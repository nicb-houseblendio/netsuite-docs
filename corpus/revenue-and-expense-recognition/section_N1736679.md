---
id: "section_N1736679"
type: "section"
title: "VSOE Revenue Recognition Examples"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > VSOE Revenue Recognition Examples"
parent: "chapter_N1717900"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html"
anchors: ["bridgehead_N1736745", "bridgehead_N1737920", "bridgehead_N1738668", "bridgehead_N1740182", "bridgehead_N1740871"]
sha256: "819a4a9f60f40e883254e7b0c13e0a1b6e9ee39a28e1c2d9bc99ecc897b8d571"
---

The following examples of vendor-specific objective evidence (VSOE) revenue recognition illustrate possible VSOE scenarios you may encounter in your workflows.

Each scenario includes examples of VSOE transactions with various VSOE settings, statuses, and pricing information for items, such as the following:

-   various delivery statuses
    
-   various deferral settings
    
-   matching/non-matching VSOE and invoice pricing
    
-   complete/incomplete VSOE prices
    
-   complete/incomplete invoice prices
    

In this group of examples, all items on the sale have a VSOE price indicated.

## VSOE Scenario 1 {#bridgehead_N1736745}

These transactions have the following attributes:

-   All items have a VSOE price.
    
-   The sales amount of the transaction equals the total VSOE amount.
    
-   No discount items or specified upgrades are included.
    
-   The invoice price is different from the VSOE amount, for some items.
    

| Item | Invoice price | VSOE Price | VSOE Allocation | Deferral | Delivered |
| --- | --- | --- | --- | --- | --- |
| Upgrade | $500 | $400 | $400 | Defer Bundle Until Delivered | Yes |
| Support | 300 | 200 | 200 | Defer Until Item Delivered | Yes |
| Product 301 | 800 | 1000 | 1000 | Defer Until Item Delivered | Yes |
| Total | $1600 | $1600 | $1600 |  |  |

The Example 1 bundle has known VSOE prices for all items and the VSOE allocation amount is equal to the VSOE price. Because all items are marked delivered, revenue recognition schedules are created for all items.

| Item | Invoice price | VSOE Price | VSOE Allocation | Deferral | Delivered |
| --- | --- | --- | --- | --- | --- |
| Upgrade | $500 | $400 | $400 | Defer Bundle Until Delivered | Yes |
| Support | 300 | 200 | 200 | Defer Until Item Delivered | No |
| Product 301 | 800 | 1000 | 1000 | Defer Until Item Delivered | Yes |
| Total | $1600 | $1600 | $1600 |  |  |

The Example 2 bundle has known VSOE prices for all items and the VSOE allocation is equal to the VSOE price. Since the Support item isn't delivered at the time of invoice, the $200 VSOE allocation amount for that item is deferred indefinitely and no revenue recognition schedule is created until it's marked delivered.

| Item | Invoice price | VSOE Price | Allocation Amount | Delivered | Deferral |
| --- | --- | --- | --- | --- | --- |
| Software Product 099 | $10,000 | $8,000 | unknown | Yes | Defer Until Item Delivered |
| Professional Services, 100 hours | 8,000 | 8,000 | unknown | No | Defer Bundle Until Delivered |
| Maintenance, 1 year | 2,000 | 2000 | unknown | No | Defer Until Item Delivered |
| Total | $20,000 | $18,000 | unknown |  |  |

The Example 3 bundle has known VSOE prices for all items, but the total invoice price of the bundle is $2,000 more than the VSOE total. Therefore, amounts aren't yet allocated because the item Professional Services has a deferral setting of Defer Bundle Until Delivered. This means that the VSOE allocation of all items in the bundle is deferred, or on hold, until this item is marked delivered.

## VSOE Scenario 2 {#bridgehead_N1737920}

These transactions have the following attributes:

-   All of the items have a VSOE price.
    
-   No items are marked Defer Bundle Until Delivered.
    
-   The total sales price of items is greater than the total VSOE price.
    

| Item | Invoice price | VSOE Price | Delivered | Deferral |
| --- | --- | --- | --- | --- |
| Service 202 | $1500 | $1000 | No | Defer Until Item Delivered |
| Product 101 | 1500 | 2000 | Yes | Defer Until Item Delivered |
| Product 103 | 2500 | 2500 | Yes | Defer Until Item Delivered |
| Total | $5500 | $5500 |  |  |

In Example 1 above, the VSOE price is allocated for delivered items. Allocation is deferred for items not yet delivered.

Products 101 and 103 are marked delivered and a recognition schedule is generated. The schedule recognizes the allocated VSOE price of each item, not the sales amount.

The VSOE price of Service 202 is deferred pending delivery.

| Item | Invoice price | VSOE Price | VSOE % | Calculate | VSOE Allocation |
| --- | --- | --- | --- | --- | --- |
| Service 202 | $0 | $1000 | 18.2% | (3700 x .182) = 672.73 | $672.73 |
| Product 401 | 2200 | 2000 | 36.4% | (3700 x .364) = 1345.45 | 1345.45 |
| Product 501 | 1500 | 2500 | 45.5% | (3700 x .455) = 1681.82 | 1681.82 |
| Total | $3700 | $5500 | 100% |  | $3700.00 |

In example 2 above, NetSuite allocates the percentage of the sales amount to each bundle member item based on the VSOE price of an item.

## VSOE Scenario 3 {#bridgehead_N1738668}

These transactions have the following attributes:

-   All of the items have an assigned VSOE price.
    
-   No items are marked Defer Bundle Until Delivered.
    
-   The total VSOE price of the bundle is greater than the total sales price.
    
-   All items are set to Defer Until Item Delivered and have been delivered.
    

| Item | Invoice price | VSOE Price | VSOE % | Calculate | VSOE Allocation |
| --- | --- | --- | --- | --- | --- |
| Service 202 | $0 | $1000 | .182 | 3700 x .182 | $672.73 |
| Product 401 | 2200 | 2000 | .364 | 3700 x .364 | 1345.45 |
| Product 501 | 1500 | 2500 | .455 | 3700 x .455 | 1681.82 |
| Total | $3700 | $5500 | 100% |  | $3700 |

In Example 1 above, NetSuite allocates the appropriate percentage of the sales amount for each line item based on the VSOE amount for each item.

## VSOE Scenario 4 {#bridgehead_N1740182}

These transactions have the following attributes:

-   All of the items have an assigned VSOE price.
    
-   At least one item is marked Defer Bundle Until Delivered.
    

| Item | Invoice price | VSOE Price | VSOE Allocation | Delivered? | Deferral |
| --- | --- | --- | --- | --- | --- |
| Service 202 | $1500 | $1000 | $1000 | No | Defer Bundle Until Delivered |
| Product 101 | 1500 | 2000 | 2000 | Yes | Defer Until Item Delivered |
| Product 103 | 2500 | 2500 | 2500 | Yes | Defer Until Item Delivered |
| Total | $5500 | $5500 | $5500 |  |  |

In Example 1 above, Service 202's deferral status is Defer Bundle Until Delivered. The VSOE price isn't allocated for any items until Service 202 is marked delivered.

-   Service 202 isn't allocated because it's not delivered
    
-   Products 101 and 103 aren't allocated even though they're delivered because Service 202 isn't yet delivered
    

When Service 202 is marked delivered, NetSuite allocates the VSOE price of all items.

-   Service 202 is allocated because it's delivered
    
-   Products 101 and 103 are allocated because they're delivered and service 202 is delivered
    

Note:

When an item in a bundle is marked **Defer Bundle Until Delivered** and that item's delivery status is Delivered, the revenue recognition of other items in the bundle depends on their individual delivered statuses.

If the delivery statuses of items in the above example are changed, the effect is as described below:

| Delivered? | Deferral | Allocation |
| --- | --- | --- |
| Service 202 = Yes Product 101 = No | Service 202 = Defer Bundle Until Delivered Product 101 = Defer Until Item Delivered | S202 = Revenue recognition begins based on the assigned schedule. P101 = Revenue recognition is deferred. |
| Service 202 = No Product 101 = No | Service 202 = Defer Bundle Until Delivered Product 101 = Defer Until Item Delivered | S202= Revenue recognition is deferred until S202 is marked delivered. P101 = Revenue recognition is deferred. |
| Service 202 = Yes Product 101 = Yes | Service 202 = Defer Bundle Until Delivered Product 101 = Defer Until Item Delivered | S202 = Revenue recognition begins based on the assigned schedule. P101 = Revenue recognition begins based on the assigned schedule. |

## VSOE Scenario 5 {#bridgehead_N1740871}

These transactions have the following attributes:

-   The transaction includes a bundle-level discount.
    
-   All items are delivered.
    
-   The Residual Method doesn't apply to the bundle.
    

In this case, a discount affects the VSOE allocation of each item in proportion to its VSOE price, or total VSOE amount for multiple items. This effect on the VSOE allocation, shown in example 1 below, is the same for transaction-level discounts.

| Item | VSOE Price | Delivered? | VSOE % | Invoice price | Calculations | VSOE Allocation |
| --- | --- | --- | --- | --- | --- | --- |
| Installation Service 302 | $1000 | Yes | .182 | $0 | (3300 x .182) = 605.45 | $605.45 |
| Software Product 401 | 2000 | Yes | .364 | $2200 | (3300 x .364) =1210.91 | 1210.91 |
| Software Product 501 | 2500 | Yes | .455 | 1500 | (3300 x .455) = 1513.64 | 1513.64 |
| **Subtotal** |  |  | 100% | 3700 |  |  |
| 10% transaction discount |  |  |  | (370) |  |  |
| **Total** | $5500 |  | 100% | $3330 |  | $3330.00 |

In example 2, there is an item-level discount on Software Product 401 and the Residual Method doesn't apply to the bundle. For sales or billing purposes, the discount applies to one specific item. However, for VSOE purposes, the discount is handled the same as a transaction-level or bundle-level discount. The discount affects the VSOE allocation of each item in proportion to their VSOE prices or VSOE amount.

| Item | VSOE Price | Delivered? | VSOE % | Invoice price | Calculations | VSOE Allocation |
| --- | --- | --- | --- | --- | --- | --- |
| Installation Service 302 | $1000 | Yes | .182 | $0 | (3480 x .182) = 632.73 | $632.73 |
| Software Product 401 | 2000 | Yes | .364 | $2200 | (3480 x .364) =1265.45 | 1265.45 |
| 10% item discount |  |  |  | (220) |  |  |
| Software Product 501 | 2500 | Yes | .455 | 1500 | (3480 x .455) = 1581.82 | 1581.82 |
| **Total** | $5500 |  | 100% | $3480 |  | $3480 |

Note:

VSOE allocation can't be automatically performed if a transaction contains multiple bundles and a transaction-level discount.

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Setting Up the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718515.html)
-   [Understanding VSOE Prices and Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718126.html)
-   [Creating VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719451.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
