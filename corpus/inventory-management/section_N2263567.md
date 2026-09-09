---
id: "section_N2263567"
type: "section"
title: "Reallocating Items"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Reallocating Items"
parent: "chapter_N2250682"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263567.html"
anchors: ["procedure_N2263709"]
sha256: "6f4d3e777eee61d909ea5b6fe59ec0b5cfeb2531d3dd0332ff275e9b998f953e"
---

Depending on your order preference setting for item commitments, you can automatically allocate items from inventory to commit them to fill orders. Inventory can be automatically committed in the following cases:

-   As you enter or approve a sales order, NetSuite can automatically commit inventory from the item's available quantity.
    
-   When you receive items from your vendors, inventory can be automatically committed to fill backorders.
    
-   Inventory that you generate from assembly work orders can be automatically committed to open orders.
    

For more information about order preferences, see [Order Management Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1388149.html). For preferences if you use the Pick, Pack, and Ship feature, see [Commitment Settings for Reallocation of Picked or Packed Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0525105436.html).

You can use the Reallocate Items page to redistribute inventory items between open orders.

For example, you commit 70 out of 100 widgets from your available quantity to a sales order. However, you get an incoming order for 50 widgets from an important customer. You can reallocate the items committed to the previous order to fill the new order.

Note:

If you use the Demand Planning feature, you can automate some item commitment processes. For details, see [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html).

#### To reallocate items: {#procedure_N2263709}

1.  Go to _Transactions > Order Management > Reallocate Items_.
    
2.  On the Reallocate Items page, select the item you want to reallocate in the **Item** field.
    
3.  Select a **Location**.
    
    A list of open orders for the item appears.
    
    The current Quantity On Hand, Quantity Committed, and Quantity Required to fulfill all orders is displayed at the top of the page.
    
    The orders pending fulfillment for this item are listed, showing the Order Number, Date, Customer, Quantity Ordered, Quantity Remaining, and the current Quantity Committed.
    
4.  To specify whether you want to commit reallocated quantities, do one of the following:
    
    -   To commit items to an order, check the box in the **Commit** column.
        
    -   Clear the box in the **Commit** column to release items from commitment to the order.
        
        Any changes update the **Uncommitted** quantity, which you can view above the **Auto Commit** button.
        
5.  In the **Quantity Committed** field, accept, increase, or reduce the number of items committed to each order.
    
    The total Quantity Committed of all orders cannot exceed the Quantity On Hand.
    
    -   To automatically commit any available items to sales orders, click the **Auto Commit** button.
        
        Items are committed to sales orders based on order of entry. For example, the oldest sales order has items committed first.
        
    -   The **Quantity Required** field displays the quantity needed for the item you select in the **Item** field. This amount is calculated as Quantity Committed + Backorders.
        
    -   If you use the Pick, Pack and Ship feature, the **Quantity Picked** displays the committed quantity that has already been picked and packed for the item. If you use the Multi-location Inventory feature, this quantity displays per location.
        
    -   If you use the Multiple Units of Measure feature, the **Units** field displays the applicable unit.
        
6.  Click **Submit**.
    

You can view the updated committed quantities on the orders. When you reallocate items and commit less than the complete quantity, NetSuite adjusts the **Commit** column setting of the order. The setting switches from **Complete Qty** to **Available Qty** for the affected order lines.

You can also view the updated inventory levels on item records.

For best practices when committing lot or serialized inventory, see [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html).

### Related Topics

-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html)
-   [Handling Backorders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263962.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
