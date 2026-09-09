---
id: "section_N609600"
type: "section"
title: "Creating a New Search to be a Custom KPI"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Key Performance Indicators > Custom KPIs > Creating a New Search to be a Custom KPI"
parent: "section_N609047"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609600.html"
anchors: ["procedure_N609608"]
sha256: "e86afb8e04c95a97af0297dc4f5dcb572f3d5968fb7a4837ca5f2b4a744f8ded"
---

To better understand the requirements that your saved search must meet to be used as a custom KPI, see [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).

You can create an existing saved search to be used as a custom KPI by completing the following steps:

#### To create a new saved search to be used as a custom KPI: {#procedure_N609608}

1.  Choose _Reports > Saved Searches > All Saved Searches_ > New.
    
2.  In the New Saved Search list, click a search type.
    
3.  On the Saved Search form, enter a title for the search. (This title will appear in the custom KPI dropdown lists in the Set Up Key Performance Indicators popup and the KPI scorecard.)
    
4.  On the **Criteria** subtab, set up filters to narrow down your search data, but don't include date filters as criteria.
    
    Note:
    
    KPIs can't enforce summary criteria filters because KPI calculations don't include groupings. If a saved search used as a custom KPI has any summary criteria filters, the KPI result might be different from the saved search results.
    
5.  On the **Results** subtab, define which fields you want to be returned in the saved search results. Make sure you have exactly one field that uses a summary type.
    
    -   If you want to display a count of the number of search results for a KPI, select a number or ID field (such as **Number**) and set a **Count** summary type for this field.
        
    -   If you want to show summary data like sum, average, minimum, or maximum, pick a field and set the right summary type.
        
6.  On the **Available Filters** subtab, add a date field to be able to compare saved search results over different date ranges in a Key Performance Indicators portlet, a trend graph, a KPI meter, or a KPI scorecard.
    
    -   If your search type doesn't have a date column as a filter, try using a different search type, like a transaction search.
        
    -   If you want to use a saved search as a custom KPI in a scorecard and you have enabled the **Use Periods** option for a scorecard, only saved searches with a **Period** filter defined as an **Available Filter** can be defined as custom KPIs for the scorecard.
        
7.  When you're done setting up the search, click **Save**. (You can also click **Save & Run** to make sure the results look right.)
    

Now you can use the search as a custom KPI and add it to the Key Performance Indicators portlet, add it to a KPI scorecard, or display it in a trend graph portlet. See [Adding a Custom KPI to the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609834.html) , or [Using a Custom KPI in a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N610062.html).

For more information about creating saved searches, see [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html).

### Related Topics

-   [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html)
-   [Selecting an Existing Search to be a Custom KPI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609351.html)
-   [Adding a Custom KPI to the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609834.html)
-   [Using a Custom KPI in a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N610062.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
