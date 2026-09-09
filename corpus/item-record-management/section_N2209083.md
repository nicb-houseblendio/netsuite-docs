---
id: "section_N2209083"
type: "section"
title: "Assembly Build Production Cost Variances"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Assembly Build Production Cost Variances"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html"
anchors: ["bridgehead_N2209226", "bridgehead_N2209256", "bridgehead_N2210072", "bridgehead_N2210102"]
sha256: "f82afcc6fd668ca5d525663a610f80df9ff7f2f32672fbfe12a94abc5c1ca42f"
---

When you use Standard Costing to track the expected cost for your items, you can compare the expected cost to the actual cost incurred. In making this comparison, you can track variances in costs for your items.

When you enter an assembly build, the cost associated with that specific build is sometimes more or less than you normally expect. For example, you normally expect the cost of the build to be $50, but sometimes the build might cost $40 or $75.

When you enter a build transaction, NetSuite compares the stored standard cost of the assembly to the actual cost incurred. The build transaction does the following:

1.  Examines the expected, standard cost and material usage for the assembly.
    
2.  Examines the actual cost and material usage for this build.
    
3.  Compares the expected cost and material usage to the actual cost and usage.
    
4.  Variances are posted that track cost fluctuations when there's a difference between either:
    
    -   Quantity of component items required was more or fewer than usual.
        
    -   Component item costs were higher or lower than usual.
        

For example, Assembly Item D is comprised of one each of Item A, Item B and Item C. Each component has a standard cost of $6, and NetSuite has calculated the expected cost of Assembly Item D to be $18. When you run an assembly production for Item D, you enter the build and mark that you used two of Item A instead of one.

Because you used more of Item A than usual, there's a difference in the expected cost and the actual cost of the assembly. NetSuite calculates the actual production cost for that run as $24 and posts a variance to the general ledger to track this $6 cost fluctuation. Posting these variance amounts maintains more accurate costing data for your items.

Build cost variances post to accounts based on the variance type and can specify different cost categories.

-   [Production Price Variances](#bridgehead_N2209226) - Variances post to this account when the cost of materials for the build is higher or lower than expected. Variances also post to this account when there are foreign exchange differences
    
-   [Production Quantity Variances](#bridgehead_N2210072) - Variances post to this account when the amount of materials used for the build is higher or lower than expected.
    
    You can set up the accounts used for both of these variances. For more information, see [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html).
    
    On assembly builds, variances are generated based on a comparison between the actual and standard cost at a per component, cost category basis. The total production variance is calculated as follows:
    
    Total Production Variance = (Actual Cost x Actual Quantity Consumed) - (Standard Cost x Standard Quantity Consumed)
    

## Production Price Variances {#bridgehead_N2209226}

A production price variance identifies cost differences between the planned expense and actual expense of assembly components.

For example, the build had a planned usage of components that cost $100. The actual cost of components used was $50. The actual cost for the build is lower than the planned cost, so NetSuite generates a variance.

This variance is calculated as follows:

Production Price Variance =

Actual Quantity Used \* (Standard Cost of Components - Actual Cost of Components)

### Example {#bridgehead_N2209256}

The following table details an example of a production price variance. It shows the bill of materials for the item Assembly A. It shows each member component of the assembly, how many are expected to be used, and the expected cost for each member.

| Bill of Materials for Assembly A |
| --- |
| Component | Quantity Per Assembly | Expected Unit Cost | Expected Total Cost |
| --- | --- | --- | --- |
| B | 2 | $17 | $34 |
| C | 3 | $19 | $57 |
| D | 5 | $23 | $115 |
| F | 7 | $29 | $203 |
|  |  | TOTAL | $409 |

The following table shows the actual build entered to assemble the item Assembly A. Notice that the actual price for component items is higher than expected. This causes the actual total cost of the assembly to increase for this build.

| Assembly Build for Assembly A |
| --- |
| Component | Quantity Used | Actual Unit Cost | Actual Total Cost |
| --- | --- | --- | --- |
| B | 2 | $119 | $238 |
| C | 3 | $171 | $513 |
| D | 5 | $345 | $1035 |
| F | 7 | $222 | $1554 |
|  |  | TOTAL | $3340 |

Because the actual cost for the build is higher than the expected cost, NetSuite generates the following variance.

| Assembly Build Variance |
| --- |
| Expected Total Cost | Actual Total Cost | Cost Difference | Variance Generated |
| --- | --- | --- | --- |
| $409 | $3340 | $2931 | $2931 |

## Production Quantity Variances {#bridgehead_N2210072}

A production quantity variance identifies quantity difference between what is planned and actual in component consumption.

For example, the build had a planned usage of four units. The actual quantity used was three. The actual cost for the build is lower than the planned cost, so NetSuite generates a variance.

This variance is calculated as follows:

Production Quantity Variance = Standard Cost of Component \* (Standard Quantity Used - Actual Quantity Used)

### Example {#bridgehead_N2210102}

The following table details an example of a production quantity variance. It shows the bill of materials for the item Assembly A. It shows each member component of the assembly, how many are expected to be used, and the expected cost for each member.

| Bill of Materials for Assembly A |
| --- |
| Component | Quantity Per Assembly | Expected Unit Cost | Expected Total Cost |
| --- | --- | --- | --- |
| B | 2 | $17 | $34 |
| C | 3 | $19 | $57 |
| D | 5 | $23 | $115 |
| F | 7 | $29 | $203 |
|  |  | TOTAL | $409 |

The following table shows the actual build entered to assemble the item Assembly A. Notice that the quantity used for all component items is higher than expected. This causes the actual total cost of the assembly to increase for this build.

| Assembly Build for Assembly A |
| --- |
| Component | Actual Quantity Used | Unit Cost | Actual Total Cost |
| --- | --- | --- | --- |
| B | 7 | $17 | $119 |
| C | 9 | $19 | $171 |
| D | 9 | $23 | $207 |
| F | 13 | $29 | $377 |
|  |  | TOTAL | $874 |

Because the actual cost for the build is higher than the expected cost, NetSuite generates the following variance.

| Assembly Build Variance |
| --- |
| Expected Total Cost | Actual Total Cost | Cost Difference | Variance Generated |
| --- | --- | --- | --- |
| $409 | $874 | $465 | $465 |

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
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
