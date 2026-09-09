---
id: "section_N2202327"
type: "section"
title: "Defining Cost Versions"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Defining Cost Versions"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html"
anchors: ["procedure_N2202405"]
sha256: "8a15f150364cac4f6e940d427a38c7d287a59cd5d49a6644b523c49e40966f2c"
---

After you create cost category records and set up item records for standard costing, you need to create standard cost version records for your items.

A standard cost version is a label to identify a time period or other identifying characteristic that you use to identify costs for items. Having different cost version records allow you to record the cost you expect to incur for an item at a particular time.

Knowing the expense you expect to pay for an item helps you track cost variations. It gives you a point of comparison after you have a cost or bill for an item. For example, you record that you expect to pay $5 each for Item A this month. Later you get a vendor bill for Item A at $8 each. You know that your costs for that month are higher than you anticipated.

Creating standard cost version records helps you track these variances. Each cost version stores a standard cost to be used on different occasions. You can use multiple cost versions per item to track expected costs over time.

For example, if the cost of an item is expected to change each quarter, you can create a cost version for each quarter:

-   Q3 2020
    
-   Q4 2020
    
-   Q1 2021
    
-   Q2 2021
    

When you have a cost version for each quarter, you can track the expected cost for each one.

Cost versions aren't limited to being based on quarters or time periods, they can identify any specifying information that you choose.

#### To define a cost version: {#procedure_N2202405}

1.  Go to _Lists > Accounting > Standard Cost Versions > New_.
    
2.  Enter a name for this cost version. For example, enter **Q1 2021**.
    
    Note:
    
    If you use NetSuite OneWorld, the cost version name should be unique per subsidiary. For example, Subsidiary US has a cost version named Version 1 US Q1 2021. The Subsidiary UK has a cost version named Version 1 UK Q1 2021.
    
3.  In the **Location** field, select one or more locations that this costing version is applicable to.
    
4.  In the **Inventory Standard Cost** field, select one of the following to define how the standard cost of inventory items is automatically calculated:
    
    -   **Average Cost** - The average cost of the inventory
        
    -   **Item Default** - The cost set in the **Standard Cost** field on the Inventory subtab on the item record. NetSuite generates planned standard cost records based on this field.
        
    -   **Last Purchase Price** - The calculated last purchase price. For more information, see [Sales and Shipping Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2171993.html).
        
5.  Click **Save**.
    

After you create cost version records, you can set up a planned standard cost record for your cost versions. The planned standard cost record let you specify the expected standard cost related to each cost version. For more information, see [Entering Planned Standard Cost Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html).

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
-   [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html)
-   [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html)
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
