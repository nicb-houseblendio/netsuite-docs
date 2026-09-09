---
id: "section_N647835"
type: "section"
title: "Summary Search Filters"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Defining an Advanced Search > Advanced Search Criteria Filters > Summary Search Filters"
parent: "section_N646477"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647835.html"
anchors: []
sha256: "b39b0c52b6502ba6056b5e9a90bb92e31a2b2a8dbcaa2213bb4a8c4e8071ef3c"
---

If you've set summary types for any search results columns, you can add additional filters to the summary results page. For more information about summary types for results fields, see [Defining Summary Types to Roll Up Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648820.html).

Note:

For more details about summary types, see [Summary Type Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659383.html) and [Summary Type Example Screenshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659760.html).

The summary search results page shows only fields with a summary type. The other results fields are in the detailed view when you click an item on the summary page.

You can apply additional filters only to the fields shown on the summary search results page.

#### To apply additional filtering to summary search results:

1.  On the **Criteria** subtab of the search definition page, click the **Summary** subtab.
    
    To learn more about the search definition page, see [Defining an Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646177.html) and [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
    
2.  In the **Summary Type** and **Field** columns, choose the options that match the field and summary type you set on the **Results** tab.
    
    Warning:
    
    If you use a multi-select related record type or a multi-select field from a related record type to define your summary search filter, your results may show duplicate data. Related record types with join fields that you can use as filters are listed at the end and have '...' after their name, for example, **Account Fields...**. There's currently no workaround for this.
    
3.  Click **Set Description**. ![Set description button](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/filter_set_description_button.png) next to the field you selected.
    
4.  In the popup window, enter a value and search logic (if available) for the field used as a filter, and click **Set**.
    
5.  The filter value appears in the **Description** column.
    
    ![Search Summary filter](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/SearchSummaryFilter.png)

Warning:

KPIs can't use summary search filters because KPI calculations don't include groupings. If a saved search used as a custom KPI has summary search filters, the KPI result may be different from the saved search result.

### Related Topics

-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Defining Standard Search Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646693.html)
-   [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html)
-   [Main Line in Transaction Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4459563851.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
