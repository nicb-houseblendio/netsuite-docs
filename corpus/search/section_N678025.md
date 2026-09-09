---
id: "section_N678025"
type: "section"
title: "Selecting Available Filters for Saved Searches"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Defining a Saved Search > Selecting Available Filters for Saved Searches"
parent: "section_N676039"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html"
anchors: ["procedure_N678056"]
sha256: "a0f9bceadda60bae6e40f3664a443ab35f79890c63ac0274d07aaaad5d902012"
---

The filters you set on the **Criteria** subtab exclude certain records from results. On the **Available Filters** subtab, you can define additional, optional filters that viewers can use to narrow results or that system functions like KPI scorecards use for summaries and comparisons.

These filters can appear as dropdown menus or multi-select boxes in the filter area, and viewers can select values to dynamically apply them. You can set a custom label for each filter's dropdown list or multi-select box.

Note:

To use a saved search as a custom KPI that displays results for multiple date ranges, you must define a date field as an available filter. You don't need to check the **Show in Filter Region** box. For additional requirements for this type of custom KPI, see [Notes on Using Saved Searches as Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html#procedure_N676064).

#### To define available filters for a saved search: {#procedure_N678056}

1.  To define a field as a filter for search results, select the field from the **Filter** dropdown list.
    
    Fields from the selected record type and join fields from related record types are listed in the **Filter** dropdown list.
    
2.  For each filter that has non-numeric values, you can check the **Show in Filter Region** box to show choices of field values in the filter region of search results, so that search viewers can dynamically filter results.
    
    By default, field values are displayed in a dropdown menu where viewers can select one value at a time.
    
    Some filters in the filter area may have limits. For more information, see [Limitations for Filters Displayed in the Filter Region](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4504549997.html).
    
3.  If you check the **Show in Filter Region** box, you can also check **Show as Multi-Select** to show values in a multi-select dropdown list, letting you choose more than one to filter results.
    
    -   By default, search results page filters use a single-select dropdown list.
        
    -   **Show as Multi-Select** doesn't apply to filters on search forms, they always show as a multi-select dropdown list there.
        
4.  You can also add a custom label for each filter.
    

If you add the **Type** field as an available filter in a transaction search and check the **Show in Filter Region** box, you see a **Type** dropdown list on the results page where viewers can choose one type of transaction at a time to filter the results.

![Saved Transaction Search example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/trans1.png)

If you check the **Show as Multi-Select** box, the filter area shows a multi-select box so you can choose more than one **Type** value to filter results.

![Show as Multi-Select box](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/transaction1.png)

### Related Topics

-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Defining Audiences for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678294.html)
-   [Highlighting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678573.html)
-   [Editing or Deleting a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679137.html)
-   [Limitations for Filters Displayed in the Filter Region](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4504549997.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
