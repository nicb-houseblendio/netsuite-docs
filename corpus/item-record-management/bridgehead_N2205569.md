---
id: "bridgehead_N2205569"
type: "bridgehead"
title: "Revaluing Standard Cost Inventory in Bulk"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Revalue Standard Cost Inventory > Process a Revaluation Transaction > Revaluing Standard Cost Inventory in Bulk"
parent: "bridgehead_N2205507"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2205569.html"
anchors: ["procedure_N2205586"]
sha256: "ddf49de79c002c8c40dfc7af6bc681454051697ecc0e214ccbbf849b92c55771"
---

This bulk process lets you create inventory revaluations for multiple items at one time. Standard costing data is retrieved from existing cost version records and you don't need to enter it manually.

Standard costing data for assembly components is updated or created on cost version records as necessary.

#### To revalue standard cost inventory in bulk: {#procedure_N2205586}

1.  Go to _Lists > Accounting > Revalue Standard Cost Inventory_.
    
2.  Select one or more **Standard Cost Versions**. Click the icon to open a multi-select popup window.
    
    A list of items corresponding to the cost versions shows.
    
3.  Select or enter the **effective date**. This is the date after which the price on the planned standard cost record is used for costing calculations.
    
4.  Select an **Adjustment Account**. The inventory value variance amounts post to this account.
    
5.  Check the **Revalue Assemblies based on Components** box to revalue all affected assemblies based on the component selected.
    
    After you submit the page, NetSuite remembers your selection for this box. The next time you open this page, NetSuite checks or clears the box based on the previous use.
    
6.  Check the box next to an item to include it in the cost rollup calculations. Clear the box next to an item to exclude it from calculations.
    
    Check the **All Items** box to perform calculations for all items.
    
7.  Click **Submit** to perform the calculations.
    

After you submit the page, NetSuite calculates the inventory value of all selected items. Going forward, transactions use the prices on the planned standard cost record.

### Related Topics

-   [Manually Entering an Inventory Cost Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205923.html)
-   [Deleting a Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163275017694.html)
-   [Process a Revaluation Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2205507.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
