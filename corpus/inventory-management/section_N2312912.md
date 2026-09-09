---
id: "section_N2312912"
type: "section"
title: "Receiving Fulfilled Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Receiving Fulfilled Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html"
anchors: ["bridgehead_4661942137", "bridgehead_N2313022", "bridgehead_N2313037", "bridgehead_N2313049"]
sha256: "4a8ed7dfebb2d7d57cfc1bd6c9eb41240f8e23e68e9f7f1a1d5b76cdcf0f9868"
---

When items being transferred between locations are received by a warehouse, the transfer order must be marked as received. Receiving a fulfilled transfer order does the following:

-   Adds the quantities received into the inventory at the receiving location.
    
-   Removes the value of the items from the Inventory In Transit account of source location.
    
-   Adds the value of the items to the inventory asset account of the destination location.
    

For example, the warehouse manager at Location A shipped 50 widgets to you at Location B. When the items are in transit between locations, the 50 widgets continue to be counted with the inventory for Location A. When you receive the package of 50 widgets from your shipper, you mark the transfer order as received. Then, the 50 widgets are added to your inventory in Location B and removed from the inventory count at Location A.

Note the following guidelines when receiving fulfilled transfer orders:

-   You cannot receive more than the quantity on the transfer order.
    
-   When you enter a receipt for a transfer order, the receipt cannot be dated prior to the shipment date of the order.
    
-   When you receive lot or serialized items, you cannot change the lot or serial numbers, including lot number quantities. The inventory numbers and lot number quantities on an item receipt must match those on the item fulfillment.
    
    Note:
    
    Changes to lot or serial numbers, including lot number quantities, must be done on the associated item fulfillment before you create a receipt. If the transfer order includes the original inventory numbers, you can update those too for consistency across transactions. Note that a transfer order may have inventory numbers that differ from those on the item fulfillment, depending on your business requirements. To update transfer orders, see [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html). To update item fulfillments, see [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html).
    
    If you want to change the inventory numbers for orders that are already received, you can process an inventory adjustment. Otherwise, you can delete the item receipts before you update the originating transactions, depending on your business requirements. To create adjustments, see [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).
    

## Full or Partial Receiving and Transfer Costs {#bridgehead_4661942137}

The item receipt quantity must match the item fulfillment quantity. If you enable the **Use Item Cost as Transfer Cost** setting on an order that is partially fulfilled, the quantity you receive must match the partial quantity on the fulfillment. This ensures accuracy when tracking item costing. For other guidelines when receiving transfer orders, [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html).

To fully or partially receive a transfer order, click **Receive** on the transfer order, and then proceed as follows:

-   If there is only one open item fulfillment, the item receipt page for that fulfillment opens and you can enter the receiving details.
    
-   If there are multiple open fulfillments, a separate page displays them in a list. Click **Receive** next to the fulfillment that corresponds to the transfer order you want to receive against. This enables NetSuite to link the item fulfillment cost to the item receipt cost.
    

To fully receive multiple transfer orders at the same time, go to _Transactions > Purchases > Receive Order_. This option submits a job to generate the item receipts, one for each transfer order.

For details on steps to receive orders, read [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html).

## Transfer Orders and Landed Cost {#bridgehead_N2313022}

If you use the Landed Cost feature, you should be aware of the way NetSuite handles transfer order receipts when you use the Cost method for landed cost allocation. If the inventory costing is recalculated on an item receipt for some line items, the landed cost of the items is not updated.

For example, an order includes two lines that have a cost of $40 for line one and $60 for line two. The landed cost is $200, so $80 applies to line one and $120 applies to line two. Later, if the cost on the transfer order fulfillment gets updated by inventory costing calculations, that cost is propagated to the item receipt. If inventory costing updates the cost of the items on the receipt to be $50 for line one and $50 for line two (instead of $40 and $60), the landed cost on the receipt is NOT updated to $100 for each line. It remains at $80 and $120.

## Departments and Classes for Received Transfers {#bridgehead_N2313037}

The receipt form defaults to show the department and class values entered on the transfer order for the destination, unless the department or class is not available at the destination subsidiary. If a department or class is required on a transaction, then you must enter an available department or class on the receipt.

## Item Value and Currency for Received Transfers {#bridgehead_N2313049}

Upon receiving the item, the value of the transferred item used on the item receipt is based on the transfer price on the transfer order.

If you use the Multiple Currencies feature, the item receipt uses an exchange rate which is the currency conversion between the source and destination locations. These can be set in the **Currency** field on the receipt.

### Related Topics

-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
