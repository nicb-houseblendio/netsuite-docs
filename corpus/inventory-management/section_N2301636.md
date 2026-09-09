---
id: "section_N2301636"
type: "section"
title: "Available to Promise Methods"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Available to Promise > Available to Promise Methods"
parent: "section_N2300269"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2301636.html"
anchors: ["bridgehead_N2301726", "bridgehead_N2302158"]
sha256: "e9be817562dfd07dd2cb7ef3166856d7fc2d8940b178d5d2ca9884ac83f47295"
---

On item records, you can choose the Available to Promise (ATP) method used to calculate the available date for the item. You can choose one of the following:

-   [Discrete ATP](#bridgehead_N2301726)
    
-   [Cumulative ATP with Look Ahead](#bridgehead_N2302158)
    

## Discrete ATP {#bridgehead_N2301726}

The Discrete ATP method reviews the item availability for each supply order and provides an available date for the specified quantity.

Non-posting purchases are fulfilled by sales orders. The quantity that is available for an item is based on the quantity available within an individual purchase.

In the following example, four supply sources are entered into NetSuite:

-   A purchase order with an expected receipt date of January.
    
-   A work order with a production end date of February 10.
    
-   A transfer order with an expected receipt date of February 15.
    
-   A purchase order with an expected receipt date of March 1.
    

Based on these sources of supply, NetSuite sets aside non-posting purchase quantities for inventory calculations. Demand sources are then counted against these purchases based on the following:

-   Expected ship date for sales orders and transfer orders
    
-   Production start date for work orders
    

The quantity that is available on a certain date is based on the supply and demand calculated for each non-posting purchase transaction.

![ATP Discrete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/InventoryManagement/ATPdiscreteBuckets.png)

|  | PO #1 January 1 | WO #1 February 10 | TO #1 February 15 | PO #2 March 1 |
| --- | --- | --- | --- | --- |
| **Supply** | 50 | 40 | 50 | 50 |
| **Demand** | (Orders dated from January 1 - February 9) 30 | (Orders dated from February 9 - February 14) 40 | (Orders dated from February 15 - February 28) 10 |  |
| **Available** | 20 | 0 | 40 | 50 |

Using Discrete ATP, NetSuite calculates the earliest date that the item is available.

-   If a quantity of 10 is requested, then the available date is 1/1.
    
-   If a quantity of 30 is requested, then the available date is 2/15.
    
-   If a quantity of 100 is requested, the available date is calculated based on the sum of the current and ATP lead time.
    

Using the Discrete ATP method, the quantity available is based on the discrete non-posting purchase quantities. If your sales order quantities are always greater than the supply quantities, you should use the Cumulative ATP with Look Ahead method.

## Cumulative ATP with Look Ahead {#bridgehead_N2302158}

Using the Cumulative ATP with Look Ahead method, supply estimates are cumulative based on all outstanding orders within a horizon. This enables you to account for future shortages.

These supply calculations are based on future-dated non-posting transactions: purchase orders, sales orders, and work orders.

For example, you can build a maximum of 50 bicycles per week based on current capacity. Bicycle Mart places an order of 200 units to be delivered a month from now. You must accumulate inventory for the next month to fulfill this Bicycle Mart order. This means that any new sales orders must have a delivery date of over one month from now.

For example, four supply sources are entered into NetSuite:

-   A purchase order with an expected receipt date of January 1.
    
-   A work order with a production end date of February 10.
    
-   A transfer order with an expected receipt date of February 15.
    
-   A purchase order with an expected receipt date of March 1.
    

On March 1, a sales order for 60 units and a purchase order for 50 units is entered.

-   The 50 units on the purchase order will be consumed by the sales order.
    
-   The sales order will also use 10 units from the transfer order on February 15.
    
-   The total amount available reflected includes this transfer amount.
    
    ![ATP Cumulative method example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/InventoryManagement/ATPcumulativeBuckets1.png)

|  | PO #1 January 1 | WO #1 February 10 | TO #1 February 15 | PO #2 March 1 |
| --- | --- | --- | --- | --- |
| **Supply** | 50 | 40 | 50 | 50 |
| **Demand** | (Orders dated from January 1 - February 9) 30 | (Orders dated from February 9 - February 14) 40 | (Orders dated from February 15 - February 28) 10 | (All orders on March 1st and beyond, within ATP lead time) 60 |
| **Projected On-hand Total** | 20 | 20 | 60 | 50 |
| **Available** | 20 | 20 | 50 | 50 |

### Related Topics

-   [Enabling Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300611.html)
-   [Checking Item Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2302738.html)
-   [Available to Promise Earliest Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159250317916.html)
-   [Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300269.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
