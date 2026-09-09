---
id: "section_N2202799"
type: "section"
title: "Entering Planned Standard Cost Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Entering Planned Standard Cost Records"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html"
anchors: ["bridgehead_N2204495", "procedure_N2204562", "bridgehead_3775406263"]
sha256: "f0acb18272bd3661cafc941e9ab0be6643802280a2324360e5d09feeff37bbff"
---

Using Standard Costing, you can compare the expected cost for an item with the cost incurred. To make this comparison, you need to define the expected cost for each cost version on planned standard cost records.

Planned standard cost records let you map out and track standard, or expected, cost of items you expect to use in the future. The standard cost is a fixed amount that you plan for as an expense.

You can create and store as many planned standard cost records as you need to anticipate different costing scenarios.

For example, you know a specific cost you expect to incur for an item on a particular date. You can enter a planned standard cost record to show the cost you expect for an item on specific future dates. You expect an item to cost $10 during January, but anticipate a rise in the cost to $20 during February. Your planned standard cost record plans for these cost fluctuations.

The planned standard cost record stores the fixed standard cost amount for an item. Each cost can be identified by a Cost Version and a Cost Category, as shown below:

| Cost Version | Item Name | Cost Category | Standard Cost |
| --- | --- | --- | --- |
| Q3 2020 | Item AB1001 | Material: Wood | $10 |
| Q4 2020 | Item AB1001 | Material: Wood | $20 |
| Q1 2021 | Item AB1001 | Material: Wood | $30 |
| Q2 2021 | Item AB1001 | Material: Wood | $50 |

You can see by the above planned standard cost record that prices for Item AB1001 are expected to rise over time. In Q3 the anticipated cost is $10, for Q4 it's $20 and further upwards over time.

When you assign a cost category, the cost is itemized in the specified category during the time that this cost version is used in production. As shown below, the parts of the assembly process for Assembly Widget A are categorized by materials and labor.

| Planned Standard Cost Record: Assembly Widget A-Q3 2011 |
| --- |
| Cost Category | Cost | Item | Quantity |
| --- | --- | --- | --- |
| Material: Metal | $90 | Metal Component 1 | 3 |
| Material: Wood | $50 | Wooden Component 2 | 2 |
| Labor: Assembly | $40 | Widget Assembly | 1 |
| Labor: Painting | $30 | Widget Painting | 1 |

This also includes the quantity of each component, which records the amount you expect to use in a build. This information is used to calculate variances by comparing expected usage to actual usage.

Note:

Amounts entered on planned standard cost records won't affect costing calculations unless you update the record into production.

## Creating New Planned Standard Cost Records {#bridgehead_N2204495}

You can create a new planned standard cost record either manually or automatically.

-   **Manual** standard cost records are created when you complete the steps below to enter costing data for an item by hand.
    
-   **Automatic** standard cost records are created for assembly items when you run a cost rollup.
    
    -   Automatic standard cost records show costing data based on NetSuite calculations of component item costs.
        
    -   When an automatic standard cost record is generated, the new calculated costs overwrite the previous manual data. This is true only if a standard cost record has previously been entered manually for the item.
        
        For more information, see [Creating Planned Cost Records Using Import and Cost Rollup](#bridgehead_3775406263) and [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html).
        

Note:

NetSuite performs calculations with a decimal precision of seven places. For example, 9.87654321 is calculated as 9.8765432.

#### To manually enter a new planned standard cost record: {#procedure_N2204562}

1.  Go to _Lists > Accounting > Standard Cost Versions > New_.
    
2.  Choose a **Standard Cost Version**.
    
3.  Select a location. The location you choose determines where you can push this version to production and use it for standard costing calculations.
    
4.  Select an item.
    
5.  Select a **Cost Category**. This category defines how NetSuite tracks cost variances.
    
6.  In the **Cost** field, enter the standard cost for the item to be associated with the selected category. This is the fixed cost you expect to pay.
    
    -   If the item you selected isn't an assembly item, this is the cost of the item selected in the header.
        
    -   If the item you selected is an assembly item, this is the cost of the component on this line.
        
7.  If the item you selected is an assembly item, complete these fields:
    
    1.  Select a component.
        
    2.  Enter a quantity. This is the number of this component you expect to use in a build.
        
    3.  Enter a unit of measure.
        
8.  Click **Add**.
    
    Non-assembly items can have only one cost category associated with them.
    
    For assembly items, you can associate multiple cost categories to track costs. If you select only one category, the entire standard cost of the item is tracked in that category.
    
9.  Repeat these steps for each cost category you need to track for this assembly item.
    
10.  Click **Save**.
     

## Creating Planned Cost Records Using Import and Cost Rollup {#bridgehead_3775406263}

You can use import functions and the Standard Cost Rollup page to create planned cost records for the inventory items. When you process the rollup, it creates the revaluation and all the planned cost records for the inventory items.

#### To create new records:

1.  Import the cost to the **standard cost** field on the item record using CSV Import or SOAP web services. For more information, see [CSV Imports Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html).
    
2.  Create a cost version with **Item Default** selected as the inventory cost. For more information, see [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html).
    
3.  Run the cost rollup.
    
    When you run the rollup, NetSuite creates all the planned standard costs for the inventory items. These are based on the item record value when you check the **Update Inventory Cost** box on the item record.
    
4.  Run a revaluation. For more information, see [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html).
    

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
-   [Manually Entering an Inventory Cost Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205923.html)
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
