---
id: "section_N2204939"
type: "section"
title: "Standard Cost Rollup"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Standard Cost Rollup"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html"
anchors: ["procedure_N2205054"]
sha256: "8934d6c3b0cc138d4879226137a041d50c14ffed41ca96897976a085e14e91ea"
---

The standard cost rollup helps maintain accurate costing data for assembly items by calculating the standard cost of assemblies. The cost of an assembly depends on current costs of its components.

The cost rollup process calculates the fixed cost based on data entered on the planned standard cost record. This allows the most accurate cost of each assembly component to be used in costing calculations.

For example, you want to know the cost of Assembly Item D. Assembly Item D is comprised of one each of Item A, Item B and Item C. The cost of each component is multiplied by the number used in the assembly. The total gives you the current cost of the assembly.

When a cost rollup is performed, NetSuite examines planned standard cost records to find the following:

-   Item A = $5
    
-   Item B = $6
    
-   Item C = $7
    

Using this data, NetSuite calculates the cost of Item D as (5 + 6 + 7) = $18, and stores it, so you can track your expected cost for Assembly Item D.

Note:

Calculations use a decimal precision to seven places. For example, 9.87654321 is calculated as 9.8765432.

In addition, cost calculations run for all parent component items. If an assembly has a component that has an assembly item itself, NetSuite does the same calculation for the sub-assembly members. Costs are calculated down to the lowest sub-assembly level and then rolled up to find the cost of the parent assembly item.

-   A cost rollup runs for an item **only if that assembly has a cost category selected** on the item record. Then, the calculated costs are broken out by components and cost categories.
    
-   NetSuite calculates the standard cost of all assemblies regardless of whether its components items use actual, average, or standard costing.
    

#### To run a cost rollup: {#procedure_N2205054}

1.  Go to _Lists > Accounting > Planned Standard Cost Rollup_.
    
2.  Select one or more **Standard Cost Versions**. Click the icon to open a multi-select popup window.
    
    A list of items corresponding to the cost versions shows.
    
3.  In the **Effective Date** field, enter the date you want the new standard cost to take effect. This defaults to the current date.
    
4.  Check the **Update Inventory Cost** box to set the standard cost of all planned standard cost records of inventory items.
    
    The planned standard cost records of inventory items are created or updated based on the inventory costing method set on the cost version. When the default item record selection is used on the cost version, the cost rollup process shows the cost in the **Standard Cost** field. This field is on the item record for each item selected. In addition, the planned standard cost of inventory items is automatically generated as part of the rollup process.
    
    The next time you open this page, NetSuite checks or clears the box based on the previous use.
    
5.  The **Rollup Assemblies Based on Components** preference lets you select only the component. NetSuite creates inventory revaluation entries for all the higher-level assemblies. For example, you can introduce a new component for several existing assemblies, as follows:
    
    Assembly A, Sub-assembly B, Component C (new)
    
    Check the **Rollup Assemblies Based on Components** box and select component C on the page. When you submit, NetSuite finds all the associated assemblies within the entire bill of materials (BOM) tree. Then, creates inventory revaluation transactions for the component and for the assemblies (A,B,C).
    
6.  Check the **Select** box next to an item to include it in the cost rollup calculations. Clear the box next to an item to exclude it from calculations.
    
    Check the **All Items** box to perform calculations for all items.
    
7.  Click **Submit** to perform the calculations.
    
    NetSuite performs the cost rollup calculations and creates or updates the planned standard cost record for all items and sub-items. You'll see a list of newly calculated planned standard cost records. Click **View** or **Edit** next to a planned standard cost records for details on that record. For more information, see [Entering Planned Standard Cost Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html).
    

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
-   [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html)
-   [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html)
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
