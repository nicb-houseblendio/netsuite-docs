---
id: "section_N2309511"
type: "section"
title: "Searches, Reports, and Reminders for Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Searches, Reports, and Reminders for Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2309511.html"
anchors: ["bridgehead_N2309535", "bridgehead_N2309570", "procedure_N2309644", "bridgehead_N2309809"]
sha256: "a127375cc2aed334096b6631a4c7794da6193fd10ee015560e0fff06ea9cd33a"
---

You can use searches, reports, and reminders to find information about inventory you are transferring.

## Reminders {#bridgehead_N2309535}

The Transfer Orders to Approve reminder shows you transfer orders due to be processed. All transfer orders that are pending approval or pending fulfillment show in the reminder.

To set up the reminder, click the Home tab and in the Settings section, click Customize this Page. In the Reminders section, click Set Up. Check the Transfer Orders to Approve box and click Save.

## Search {#bridgehead_N2309570}

Transaction searches show the status, source and destination locations, quantities in-transit, quantities shipped, and quantities received for a transfer order.

If you customize an item search to show the Location in Transit column in results, the list shows the in-transit quantity for each location. For any quantity of items that is in transit, that quantity is reduced from the On Hand count for the item at the source location. The quantity is not added to the receiving location until the transfer order is marked received.

#### To customize a search:

1.  Go to Reports > New Search.
    
2.  Click **Item**.
    
3.  On the **Item Search** form, click **Personalize Search**.
    

When you run a transaction search, you can set the following criteria to search for transfer orders:

-   Transfer Location (To Location)
    
-   Location (where the transaction is processed)
    
-   Order Status
    
-   Order Number
    

## Saved Searches {#procedure_N2309644}

You can create a Saved Transaction Search to find detailed information about transfer orders.

#### To create a saved search:

1.  Go to _Reports > Saved Searches > All Saved Searches._.
    
2.  Click **New**.
    
3.  Click **Transaction**.
    
4.  On the **Saved Transaction Search** page, **Criteria** subtab Sin the **Filter** field, you can choose to add the following:
    
    -   Transfer Order Line Type
        
    -   Transfer Order Quantity Committed
        
    -   Transfer Order Quantity Fulfilled
        
    -   Transfer Order Quantity Packed
        
    -   Transfer Order Quantity Picked
        
    -   Transfer Order Quantity Received
        
5.  On the **Results** subtab on the **Columns** subtab, you can choose to add the following:
    
    -   Transfer Location
        
    -   Transfer Order Item Line ID
        
    -   Transfer Order Line Type
        
    -   Transfer Order Quantity Committed
        
    -   Transfer Order Quantity Packed
        
    -   Transfer Order Quantity Picked
        
    -   Transfer Order Quantity Received
        
    -   Transfer Order Quantity Shipped
        

For example, you can select as a search criterion a Transfer Order Line Type that is Any Of Item, Shipping and Receiving. Select in Results to show the Transfer Order Item Line ID and Transfer Order Line Type. Then, when you run the search, for each transfer order line, Item Shipping and Receiving data is displayed for each line on each order.

## Reporting {#bridgehead_N2309809}

The Transfer Order Register shows all transfer orders with their number, status, and amount.

To view the Transfer Order Register, go to _Reports > Inventory/Items > Transfer Order Register._.

The following reports also include transfer order data:

-   Inventory Backorder Report
    
-   Inventory Pending Fulfillment Report
    
-   Shipping Report
    

Also, when viewing the Current Inventory Snapshot Report, the In Transit column displays quantities in transit.

### Related Topics

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

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
