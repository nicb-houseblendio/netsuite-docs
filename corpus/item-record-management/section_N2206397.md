---
id: "section_N2206397"
type: "section"
title: "Standard Costing and Transactions"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Standard Costing and Transactions"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html"
anchors: ["subsect_163275164575", "subsect_163275166848", "bridgehead_N2208090", "bridgehead_N2208277", "bridgehead_N2208464", "bridgehead_N2208663"]
sha256: "8e97a63b613b57ace0843710556d2667ea730fc62533bc2688f3940c0525ade9"
---

When you use the Standard Costing feature, transactions you enter in NetSuite include line-item data to process standard costing variances.

Please note the following:

-   The sum of the cost across cost categories for an item generates the total cost of an item.
    
-   Purchase price variances can post on any 'more-on-hand' transactions, including purchase receipts and transfer order receipts.
    
-   When transactions are processed using Standard Costing, the item cost is valued at a per-cost category level for non-lot numbered and non-serial numbered items.
    
    -   For lot numbered items, inventory is valued at a per cost category, lot number combination.
        
    -   For serial numbered items, inventory is valued at a per cost category, serial number combination.
        

The following details how NetSuite processes transaction data with Standard Costing enabled. The examples below refer to Item A, which has a standard cost of $3 and an actual cost of $5 on transactions. The resulting general ledger postings are shown in tables as below:

## Purchase Order Receipts {#subsect_163275164575}

-   The inventory asset value is always set at standard cost.
    
-   A variance is generated for any difference between the actual cost shown on the order and the standard cost.
    

| Account | Amount |  |
| --- | --- | --- |
| Asset | $3 | standard cost |
| Purchase Price Variance | $2 | difference in standard and actual cost |
| Accrued Purchases | $ -5 | actual cost |

## Purchase Order Receipts With Landed Cost {#subsect_163275166848}

-   The inventory asset value is always set at standard cost.
    
-   A variance is generated for any difference between the actual cost shown on the order and the standard cost.
    
    The variance isn't divided into individual cost categories.
    

## Transfer Order Receipts {#bridgehead_N2208090}

A Gain/Loss value is generated based on the difference between the transfer price and standard cost at the source location. A variance is generated for any difference between the standard cost at the origination and destination locations.

| Account | Amount |  |
| --- | --- | --- |
| Asset | $3 | standard cost |
| Purchase Price Variance | $2 | difference in standard and actual cost |
| In Transit | $ -5 | loss on the item fulfillment record Note: The source location records the Gain/Loss account that transferred the item to the destination location. This account reflects in the GL impact of Item Fulfillment because the In Transit account is established at fulfillment. |

## Inventory Transfer {#bridgehead_N2208277}

A variance is generated for any difference between the standard cost at the origination and destination locations.

| Account | Amount |  |
| --- | --- | --- |
| Asset (From Location) | $ -2 | standard cost of location B |
| Asset (To Location) | $5 | standard cost of location A |
| Purchase Price Variance | $ -3 |  |

## Assembly Build {#bridgehead_N2208464}

Cost variances are divided into different cost categories and variance types. For more information, see [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html).

| Account | Amount |  |
| --- | --- | --- |
| Asset (Assembly) | $3 | standard cost |
| Asset (Component) | $ -5 | standard |
| Variances | $2 |  |

## Assembly Unbuild {#bridgehead_N2208663}

Any difference between the standard and actual cost is posted to the Unbuild Variance account. For information about setting this account for items, see [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html).

| Account | Amount |  |
| --- | --- | --- |
| Asset (Assembly) | $ -3 | standard/actual/average cost |
| Asset (Component) | $5 | standard |
| Unbuild Variances | $ -2 |  |

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
-   [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html)
-   [Entering Planned Standard Cost Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html)
-   [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html)
-   [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
