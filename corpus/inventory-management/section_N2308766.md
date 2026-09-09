---
id: "section_N2308766"
type: "section"
title: "Inventory Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Inventory Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html"
anchors: ["bridgehead_N2309039", "bridgehead_4660893916", "bridgehead_N2309112", "bridgehead_N2309140", "bridgehead_N2309159", "bridgehead_N2309232", "bridgehead_N2309252", "bridgehead_N2309273", "bridgehead_4813057068"]
sha256: "5245a2649c00d176ce9c4a3dff2da0ce22d7eda49d88fbdfb2d036aec21cbc32"
---

When you transfer inventory from one location to another, you can enter inventory transfer orders to schedule and track the movement of items.

Transfer orders are different than basic inventory transfers because you can track each stage of the transfer process and know when items are in transit. In contrast, a basic inventory transfer changes the item count in both locations in one step. For details about basic transfers, read [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html).

Transfer orders help you manage items that are moved from one location to another over a period of time.

The transfer order workflow is as follows:

1.  A transfer order is entered to schedule the movement of items and can go through an approval process.
    
2.  When a transfer order is approved, the following occurs:
    
    -   Items are committed out of the source location's inventory
        
    -   The On Order quantity of the items at the destination location increases.
        
3.  Transfers are then fulfilled out of the source location and you know when the items are in transit.
    
    -   Fulfilled items are removed from the On Hand count at the source location.
        
    -   The value of items in transit are removed from the Inventory Asset account and added to the Inventory in Transit account for the source location.
        
4.  Finally, the destination location enters a receipt for the items.
    
    -   The items are added to the destination location's inventory and increase the On Hand count.
        
    -   The items' value is added to the Inventory Asset account for the destination location.
        
    -   The On Order quantity of the item in the destination location decreases.
        

For example, your Location A sells an order for 100 widgets, but only has 20 in stock. It normally takes two weeks to receive an order from your regular widget vendor, but your customer cannot wait that long. After checking stock at all locations, you see that your Location B has 200 widgets in stock. You enter an inventory transfer order to move 80 widgets from Location B to Location A so you can fill the customer's order quickly.

The shipping manager at Location B sees that a new inventory transfer order has been entered for the location. Turnover of widgets is low at this location recently, so the transfer order is approved. After it is approved, the items are committed to the transfer and cannot be sold when in transit.

The warehouse manager at Location A sees that the transfer order was approved and knows the widgets are in transit. He can estimate when the widgets will arrive and when he can fulfill the customer's order.

The approved inventory transfer order now shows in the queue at Location B to be fulfilled and shipped to Location A. The warehouse at Location B prints a picking ticket and then picks, packs and ships the items out using their preferred shipping company.

When the shipment of widgets arrives at Location A, the manager marks the transfer order as received and the items are added to inventory. The items can then be used to fulfill the order and prepared to ship out to the customer.

Inventory transfer orders can detail the following:

-   Items and quantities intended to be transferred
    
-   When items are fulfilled and shipped out of the source location, which may include picking and packing
    
-   The status of transfers and when items remain in transit
    
-   When items are received in the receiving location
    
-   Outstanding items yet to be transferred
    
-   Transfer price of items
    

Lines on transfer orders cannot be partially fulfilled or partially received, the entire line must be processed at one time. Only available stock can be committed to transfer orders.

Transfer orders you create and process are linked to any related item fulfillments and to item receipts.

Use of transfer orders requires that you have enabled the Multi-Location Inventory feature. For details about enabling features, read [Items and Inventory Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N235482.html) or [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html).

## View Transfer Data on Item Records {#bridgehead_N2309039}

You can view transfer details on item records, as follows:

-   On the **Inventory** subtab, the **Quantity on Order** for an item includes the quantities on approved transfer orders.
    
-   On the **Inventory** subtab, the **Transfer Price** field allows entry of a transfer price for declared values when shipping.
    
    -   The transfer price is not a charge for the destination location.
        
    -   The transfer price is a shipping amount for reference only, such as for insurance or international shipping and does not affect inventory costing.
        
    -   The transfer price defaults to show a value of zero.
        
-   On the **Locations** subtab, the **Qty in Transit** column displays the amount transferred out of a location.
    
-   On the **Lot Numbers** subtab, the **Qty in Transit** column displays the amount transferred out of a location.
    

For information about other item quantities, see [Assessing Stock Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2262573.html).

## Item Costing and General Ledger {#bridgehead_4660893916}

Transfer orders do not post to a Cost of Goods Sold (COGS) account. They post to remove the item value from the source location's asset account and add the value to the Inventory in Transit account. Individual transfer orders include a setting to Use Item Cost as Transfer Cost. When a new transfer order is created, this setting defaults to the accounting preference setting. By putting this setting on the transfer order, users have more flexibility on in managing the inventory GL.

Note:

You can change this setting if the transfer order is not approved. After the transfer order is approved, this setting cannot be changed.

## Preferences for Transfer Orders {#bridgehead_N2309112}

You can set preferences that determine handling for transfer orders that you enter. Preferences are available for the default order status and handling fulfillments based on commitments.

When you require approval for processing transfer orders, after a transfer order is entered, the order must be approved by someone with permission before it can be fulfilled.

For details on these preferences, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

## Transfer Serialized and Lot Inventory {#bridgehead_N2309140}

When you enter a transfer order, you may enter the serial numbers for items you are transferring, but you must enter a serial number for each item on the order. You cannot enter serial numbers for only some of the items. After you have entered serial numbers on a transfer order, the **Serial/Lot Numbers** field is disabled on the fulfillment form.

If you do not enter serial numbers on the transfer order, then the **Serial/Lot Numbers** field is enabled on the fulfillment form and you must enter serial numbers there.

The **Serial/Lot Numbers** field is always disabled when you receive a transfer order. For more information, see [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html).

## Location Restrictions for Transfer Orders {#bridgehead_N2309159}

Users who have access that is restricted by location have the following limitations when working with transfer orders.

-   **Create/Edit/Copy**: If you are restricted to access only one location, you can create a transfer order, but it will require approval because the source location list shows only one location. The source location will need to be entered to approve the order.
    
    You can only edit or make a copy of a transfer order if you have access to both the source and destination locations.
    
-   **Fulfill**: The Fulfill Orders page and Print Picking Ticket page show only transfer orders for which for which you have access to the source location.
    
-   **Receive**: The Receive Order page shows only transfer orders for which for which you have access to the destination location.
    
-   **Reminders**: The Orders to Fulfill reminder shows only transfer orders for which you have access to the source location. The Orders to Receive reminder shows only transfer orders for which you have access to the destination location.
    
-   **Reports**: The Transfer Order Register report displays only orders for which have access to either the source or destination location on the order.
    

## View Searches, Reports, and Reminders {#bridgehead_N2309232}

You can use transaction searches, saved searches, reports, and reminders to find information about inventory you are transferring. For details, read [Searches, Reports, and Reminders for Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2309511.html).

## Customize Transfer Order Forms {#bridgehead_N2309252}

You can specify linked forms to be used when processing transfer orders, or add custom fields to transfer order forms. For details, read [Customizing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313259.html).

## Intercompany Transfers for NetSuite OneWorld Accounts {#bridgehead_N2309273}

In NetSuite OneWorld accounts, you can enter an Intercompany Transfer Order to move inventory between locations in two different subsidiaries within your company.

Enter an Intercompany Transfer Order to schedule items to be shipped out of one subsidiary location and received into the inventory at another subsidiary location. Intercompany transfer orders enable you to track items in transit between the two subsidiary locations.

To use intercompany transfer orders, go to _Transactions > Inventory > Enter Intercompany Transfer Orders._.

This form is available only in NetSuite OneWorld accounts.

Read the [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html) topic.

## Use Multi-Book and Transfer Orders {#bridgehead_4813057068}

If you use the Multi-Book Accounting feature in a NetSuite OneWorld account, the following applies for transfer orders:

-   If a secondary book exists in the source subsidiary but does not exist in the destination subsidiary, then the destination subsidiary does not post a cost at the time of the transfer.
    
-   If a secondary book exists in the destination subsidiary but does not exist in source subsidiary, then the transfer cost in the primary book is used as the transfer cost when posting in the secondary book.
    

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)
-   [In-Transit Ownership](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4813066512.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
