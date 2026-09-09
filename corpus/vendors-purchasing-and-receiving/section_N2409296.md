---
id: "section_N2409296"
type: "section"
title: "Drop Shipment and Special Order Purchases"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Drop Shipment and Special Order Purchases"
parent: "chapter_N2399286"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2409296.html"
anchors: ["bridgehead_N2409490"]
sha256: "68acb96475894fbb32296a62792cccc178e9428a5b2594dc363d46c00e7442b7"
---

You can use the Drop Shipments and Special Orders feature to create purchase orders for items. When a sales order is approved that contains drop ship or special order item, a purchase order is automatically created for the item.

Drop shipments and special order items are purchases that are not processed the same way as other items that you purchase:

-   When you drop ship an item, the item is sent directly from your vendor to your customer. The item is not processed in your inventory.
    
-   Use special orders to purchase and track items that might not follow regular inventory processing, such as immediate-need orders or orders for customized items. For example, you sell items that are customized by your vendor. You can track custom item orders as special order items. The sales order is not fulfilled with regular stock. It is fulfilled only when the linked order for the special item is received from the vendor.
    

Items are identified as a drop shipment or a special order when the sales order is created. For more information, see [Marking an Item for Drop Shipment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239986.html) and [Identifying Special Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244641.html).

You can also manually set an item to drop ship or be special ordered when entering, editing or viewing sales orders:

-   When entering a sales order, select **Drop Ship** or **Special Order** in the **Create PO** column next to the item.
    
-   When editing an existing sales order:
    
    In **View** mode, click **Drop Ship** or **Spec. Ord.** in the **Create PO** column next to the item.
    
    In **Edit** mode, click the line-item. In the **Create PO** field, select **Drop Ship** or **Special Order**.
    

When a sales order that contains an item set to drop ship or special order is saved or approved, a purchase order is automatically initiated.

-   Drop-ship purchase orders show the preferred vendor for the item and the customer's shipping address.
    
-   Special order purchase orders show the preferred vendor for the item and your company's shipping address.
    
-   The Administrator permission is used to create the work order or purchase order if either of the following conditions apply:
    
    -   The drop-ship order is created from the web store, or
        
    -   The user doesn't have permission to create the work order or purchase order.
        
        If the Administrator permission is required to create the work order or purchase order, the preferred form for the administrator role is used.
        

Note:

If you use NetSuite OneWorld and have vendors shared with multiple subsidiaries, note the following. If a sales order for a secondary subsidiary includes an item marked for drop ship, NetSuite automatically creates a purchase order. This purchase order is based on the preferred vendor for that drop shipped item.

If the subsidiary on the sales order is not the subsidiary of the preferred vendor for the item, you must manually create the purchase order.

For more information about shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

If you use Multiple Currencies, drop shipments and special orders use the primary currency of the preferred vendor. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).

If you use Multiple Units of Measure and have enabled the Update Special Order Quantities Automatically Prior to Shipment preference, note the following. You should use the same unit of measure on both the purchase order and sales order for an item. If you use different units of measure, it can cause errors due to rounding for differences greater than five decimal places.

To create the purchase orders that are initiated by drop shipments and special orders, go to _Transactions > Inventory > Order Items._.

After you have placed orders, you can view them by going _to Transactions > Purchases > Enter Purchase Orders > List._. On the Purchase Orders page, you can click View or Edit next to an order to open it. The Status column shows the status of the order.

Note:

You shouldn't delete an existing purchase order that contains a serial-numbered or lot-numbered item. Doing so can place your inventory in an invalid state.

You can set preferences so the purchase order is automatically emailed, faxed or set to print when it is generated. You can also select which purchase order transaction form you want to use. To set purchase order preferences, go to _Setup > Accounting > Preferences > Accounting Preferences_. Click the Order Management subtab.

## Marking the Purchase Order Fulfilled {#bridgehead_N2409490}

If you use Advanced Shipping, Advanced Receiving, both or neither, there are different ways to receive the purchase order and mark the sales order fulfilled:

-   **Advanced Shipping and Advanced Receiving**
    
    On the purchase order, click **Mark Shipped** to receive purchase orders and mark sales orders as fulfilled. Clicking **Mark Shipped** opens the sales order fulfillment page. When you submit the fulfillment, the purchase order status is set to **Pending Billing**. The purchase order and sales order are then ready to be billed.
    
    If you receive the items on the Receive Purchase Order page, the sales order is not updated to reflect that the items have shipped. You must open the sales order and click **Fulfill** to show that the items have shipped. Then, the purchase order and sales order have a **Pending Billing** status.
    
-   **Advanced Shipping**
    
    On the purchase order, click **Receive** to receive the order and bill it.
    
    On the sales order, click **Fulfill** to mark it as fulfilled and create an invoice or cash sale.
    
-   **Advanced Receiving**
    
    On the purchase order, click **Receive** to receive the order and bill it.
    
    On the sales order, click **Process** to mark it as fulfilled and create an invoice or cash sale.
    
-   **Neither**
    
    On the purchase order, click **Receive** to receive the order and bill it.
    
    On the sales order, click **Process** to mark it as fulfilled and create an invoice or cash sale.
    

### Related Topics

-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)
-   [Purchase Order Approval Workflow SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2398841.html)
-   [Accounting for Received Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408991.html)
-   [Purchase Order History Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2409777.html)
-   [Centralized Purchasing and Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161122386910.html)
-   [Purchasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2399286.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
