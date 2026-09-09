---
id: "section_N2402825"
type: "section"
title: "Bulk Orders"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Management > Bulk Orders"
parent: "section_N2399585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html"
anchors: ["bridgehead_N2402858", "bridgehead_N2402942", "bridgehead_4413965570"]
sha256: "77cccd60b32af28d0d0e95a3911bf920041c3957620c239b1a0c4a88e8dd34cb"
---

You can create purchase orders in bulk for items you need to restock. The Order Items page lists items that NetSuite determines are in need of being replenished. In this way, bulk item ordering helps automate your replenishment process and keep your inventory at an optimum level.

To use bulk item ordering, you can add items to the list by using either the Demand Planning feature or the Advanced Inventory Management feature.

## Bulk Ordering with Demand Planning {#bridgehead_N2402858}

When you use the Demand Planning feature, item orders are generated using demand plans and supply plans that incorporate historical demand and expected future orders. Supply plans determine when items are ordered and in what quantity. After a supply plan is reviewed, the orders can be generated using the Order Items page.

For details about the Demand Planning feature and how it produces orders, read the following topics:

-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
    
-   [Calculating Item Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html)
    
-   [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html)
    
-   [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html)
    

## Bulk Ordering with Advanced Inventory Management {#bridgehead_N2402942}

When you use Advanced Inventory management, you set a preferred stock level and reorder point on each item record. When records indicate that an item is backordered or below its set reorder point, the item is added to the Order Items form. The Order Items page suggests a quantity to order based on your preferred stock level and the quantity of open backorders.

NetSuite checks stock levels on item records to determine if the item should be reordered.

-   Any item record that shows a backordered quantity greater than zero appears on the Order Items page.
    
    **Qty. Backordered** = quantity committed to sales for which there is no stock to fill the order
    
-   Any item record that shows an available quantity below the reorder point will appear on the Order Items page.
    
    Note:
    
    If there are inventory items with an on-order quantity equal to or greater than the backordered quantity, note the following. The item no longer appears on the Order Items page.
    
    To calculate the Quantity Available for an item, NetSuite analyzes the following:
    
    **Qty. Available** = (Qty. On Hand - Qty. Committed)
    
    **Qty. On Hand** = quantity now stocked, including the Quantity Committed
    
    **Qty. Committed** = The quantity promised to customers on approved sales orders, that are not yet fulfilled.
    

The **Qty. Available** on the Item record and Order Items page shows zero or higher, even if the actual value is negative. However, when calculating the quantity to order, NetSuite uses the true value from your records, including any negative amounts.

For example, if **Qty. On Hand** is -17, and **Qty. Committed** is 0, NetSuite shows a **Qty. Available** of 0, but calculates replenishment using -17. This process ensures that order recommendations accurately reflect your inventory position, even when the displayed value is zero.

For more information about item commitment, see [Committing Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3765928460.html).

After NetSuite determines which items need to be ordered, it determines the quantity needed. To do so, NetSuite compares the item's Quantity Available to the preferred stock level.

For example, the record for item #12345 shows the following:

-   Manual Reorder Point = 80
    
-   Manual Preferred Stock Level = 100
    
-   Quantity on Hand = 90
    
-   Quantity Committed = 20
    

NetSuite committed 20 of the 90 you have on hand, leaving a Quantity Available of 70. Because a quantity of 70 is below the reorder point of 80, NetSuite suggests that you order the item. You should order 30 of the item to bring you back up to your preferred stock level of 100.

In another example, the record for item #12345 shows backorders:

-   Manual Reorder Point = 80
    
-   Manual Preferred Stock Level = 100
    
-   Quantity on Hand = 0
    
-   Quantity Backordered = 25
    

Because you need more of the item to fill backorders and replenish stock, you should order the item. You need 25 to fill backorders and 100 to reach the preferred level. You should order 125 of the item to bring you back up to your preferred stock level of 100.

Bulk ordering items makes procurement straightforward and efficient. You can order the optimal amount of items you need without gathering information from several places to assess replenishment needs.

At any time, you can also create purchase orders manually. To do so, make your own assessment about what stock you need, how much to order and when to place the order. For more information, see [Assessing Stock Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2262573.html).

## Auto-calculated Order Quantities {#bridgehead_4413965570}

For items set to automatically calculate the reorder point and preferred stock level, the calculations to determine the quantity to order are as follows:

-   Reorder quantity = Average daily demand \* number of days (preferred stock level)
    

For example, an item has a daily demand rate of 2.77 and a number of days supply of 10. The reorder quantity is (2.77 \* 10) = 28 because the quantity is rounded to the nearest integer.

Note:

If you use the Multiple Units of Measure feature, the reorder quantity rounds to the nearest integer in purchase units.

For more information about setting inventory to auto-calculate, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).

After the quantity needed is determined for items, you should use the amount to order on the Order Items page.

To manually set preferred stock levels and reorder points on item records, go to _Lists > Accounting > Items_.

### Related Topics

-   [Setting Purchasing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400174.html)
-   [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html)
-   [Ordering Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html)
-   [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html)
-   [Editing a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2404305.html)
-   [Viewing the Status of a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408514.html)
-   [Printing a Tax ID or Resale Number on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4746558953.html)
-   [Purchase Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2407704.html)
-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
