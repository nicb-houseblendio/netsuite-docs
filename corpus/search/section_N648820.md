---
id: "section_N648820"
type: "section"
title: "Defining Summary Types to Roll Up Search Results"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Defining an Advanced Search > Search Results Display Options > Defining Summary Types to Roll Up Search Results"
parent: "section_N648053"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648820.html"
anchors: []
sha256: "59e25e7cb48e1f4b4ffd71030ef97723bd9a39867154f6a054e236af6a1d7ee4"
---

The **Results** subtab for an advanced or saved search has a summary type column where you set how to group data. When you add summary types, your search returns a summary page where you can drill down to each group of results.

-   First, set a Group summary type for the field you want to use for grouping. The summary page lists the values for this field. Click a value to drill down into each group.
    
    For example, in a customer search, set a Group summary type for the sales rep field. The summary page shows a list of all sales reps, and you can click one to see their customers.
    
-   After you set a Group, you can add another summary type to see quantities on the summary page:
    
    -   **Count** - Counts results for the field, usually on name or ID fields to see how many records are in each group.
        
    -   **Sum** - Adds up the fields' values.
        
    -   **Minimum** - Shows the lowest amount or the earliest date.
        
    -   **Maximum** - Shows the highest amount or the latest date.
        
    -   **Average** - Calculates the average of the fields' values.
        
    
    For example, in a customer search grouped by sales rep, set a **Count** for the customer name field to show how many customers each sales rep has. Or set a **Sum** on the balance field to show a total balance for each sales rep's customers.
    

Any field not listed with the same name in search criteria field listing (**Criteria** subtab > **Standard** subtab) won't be available for drilldown when grouped in the **Results** subtab > **Columns** subtab.

Drilldown pages you reach from the summary pages don't include their own subtotals. To add them, check the **Show Totals** box on the **Results** subtab. See [Showing Totals in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649366.html).

In special cases, you can use a Minimum or Maximum summary type to get a value in one field based on the lowest or highest value in another. In this case, choose this other field as the **When Ordered By Field**. See [Using When Ordered By Field for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649095.html).

For more information, see [Summary Type Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659383.html) and [Summary Type Example Screenshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659760.html).

Note:

To use a saved search as a custom KPI for multiple date ranges, you must have only one field with a summary type. For additional requirements on this type of custom KPI, see [Notes on Using Saved Searches as Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html#procedure_N676064).

### Related Topics

-   [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html)
-   [Selecting Fields to Display in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648349.html)
-   [Entering Custom Labels for Search Results Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648659.html)
-   [Using When Ordered By Field for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649095.html)
-   [Showing Totals in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649366.html)
-   [Applying Functions to Search Results Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649633.html)
-   [Defining Order and Overall Formatting for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N651604.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
