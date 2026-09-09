---
id: "section_N609351"
type: "section"
title: "Selecting an Existing Search to be a Custom KPI"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Key Performance Indicators > Custom KPIs > Selecting an Existing Search to be a Custom KPI"
parent: "section_N609047"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609351.html"
anchors: ["procedure_N609360"]
sha256: "69de6ceac8c1af7d1fc5a337ef71ee0c0b2f1a80cf24510045f8f3cd3bacb62d"
---

To better understand the requirements that your saved search must meet to be used as a custom KPI, see [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).

You can edit an existing saved search to be used as a custom KPI by completing the following steps:

#### To select an existing saved search to be used as a custom KPI: {#procedure_N609360}

1.  Choose _Reports > Saved Searches > All Saved Searches_.
    
2.  In the Saved Searches list, click **Edit** next to the search you want to use as a custom KPI. Make sure the search is set up to show KPI data the way you want.
    
3.  On the **Criteria** subtab, make sure you're not using any date filters as search criteria.
    
    Note:
    
    KPIs can't enforce summary criteria filters because KPI calculations don't include groupings. If a saved search used as a custom KPI has any summary criteria filters, the KPI result might be different from the saved search results.
    
4.  On the **Results** subtab, make sure you have exactly one field that uses a summary type.
    
    -   If you want to display a count of the number of search results for a KPI, select a number or ID field (such as **Number**) and set a **Count** summary type for this field.
        
    -   If you want to display summary data such as sum (total), average, minimum, or maximum, select a field and set the appropriate summary type for it.
        
5.  On the **Available Filters** subtab, add a date field to be able to compare saved search results over different date ranges in a Key Performance Indicators portlet, a trend graph, a KPI meter, or a KPI scorecard.
    
    -   If the type of search you have selected does not offer a date column as a filter, you may be able to use a different type of search, for example, a transaction search.
        
    -   If you want to use a saved search as a custom KPI in a scorecard and you have enabled the **Use Periods** option for a scorecard, only saved searches with a **Period** filter defined as an **Available Filter** can be defined as custom KPIs for the scorecard.
        
6.  Edit the search to meet your requirements and resave it.
    
    -   If you do not have the ability to edit and resave this search, you can ask the owner to edit it, or you can create another, similar search yourself.
        
    -   Choose **Save & Run** to verify the search results are what you expect.
        
7.  Note the title of the search. It will appear in the custom KPI lists in the Set Up Key Performance Indicators popup and the KPI scorecard.
    
8.  Now you can use the search as a custom KPI and add it to the Key Performance Indicators portlet, add it to a KPI scorecard, or display it in a trend graph portlet. See [Adding a Custom KPI to the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609834.html) , or [Using a Custom KPI in a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N610062.html).
    

For more information about editing saved searches, see [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html).

### Related Topics

-   [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html)
-   [Creating a New Search to be a Custom KPI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609600.html)
-   [Adding a Custom KPI to the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609834.html)
-   [Using a Custom KPI in a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N610062.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
