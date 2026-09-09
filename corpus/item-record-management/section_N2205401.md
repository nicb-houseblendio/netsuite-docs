---
id: "section_N2205401"
type: "section"
title: "Revalue Standard Cost Inventory"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Revalue Standard Cost Inventory"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html"
anchors: ["bridgehead_N2205444", "subsect_163274945804"]
sha256: "26c35fe607a284751c1cbeac6a499bbf185fde8d6d2313fada40fc37c6381f4b"
---

You can enter a transaction to revalue standard cost inventory for each planned standard cost record. This revaluation process does the following:

-   Sets the standard cost for items as of the specified effective date
    
-   Calculates the current inventory value based on the current standard cost
    

## Set Current Standard Cost {#bridgehead_N2205444}

1.  First, the revaluation transaction sets the standard cost of an item.
    
    This process tells NetSuite which cost and cost category to use on transactions for the item as of the effective date.
    
2.  After you run the revaluation, any new transactions use the updated standard cost for items.
    
    For example, the current cost on record for the item Assembly Widget A is $20. You previously created a planned standard cost record for Widget A that's associated with cost version Q3 2020. It shows the standard cost of Widget A at $30. Now, you want to push that cost to production so it's used in costing calculations as of July 1, 2021. To do so, enter an inventory cost revaluation.
    

## Calculate Inventory Value {#subsect_163274945804}

An inventory cost revaluation transaction sets the value of on-hand inventory, calculated as:

On-hand value = (standard cost \* current quantity on hand)

Therefore, the current standard cost of Item A is set at $30 and the on-hand count is 100 units. The current value of Item A stock on hand is ($30 \* 100) = $3000.

For assemblies, this is calculated as follows:

On-hand value per cost component = (component standard cost \* current quantity on hand)

After you run the revaluation, inventory values are current and more accurate on records.

When you enter an inventory revaluation and an item has no quantity on hand, the result shows as blank.

### Related Topics

-   [Process a Revaluation Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2205507.html)
-   [Revaluation and Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4659460723.html)
-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
-   [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html)
-   [Entering Planned Standard Cost Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html)
-   [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html)
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
