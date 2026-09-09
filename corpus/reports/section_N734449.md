---
id: "section_N734449"
type: "section"
title: "Using Multi-Select Options in Report Footer Filters"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Working with Report Results > Setting Report Footer Options > Using Multi-Select Options in Report Footer Filters"
parent: "section_N720025"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734449.html"
anchors: ["bridgehead_N734479", "bridgehead_N734531"]
sha256: "77afcfdc328085198fd7738ce1b7d64afc065f00f2b0640a5fa6947e5d61c38a"
---

Some filter options in report footers offer the possibility to select multiple values.

![Filter options in the report filters.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/classany1.png)

## Selecting Values for a Multi-Select Option {#bridgehead_N734479}

-   Select multiple values by pressing and holding the Ctrl key, as you are selecting individual values from the list.
    
-   Select multiple consecutive values by pressing and holding the Shift key, as you are selecting the first and last values in a range from the list.
    
-   Select all values by checking the All box. (see the note below about the difference between checking All and manually selecting all values).
    

Note:

Checking the All box isn't the same as clicking each value one at a time. For example, if you check All when there are 5 options and a new value is later added, your report will include all 6 values. But if you picked the 5 values one by one, the new value wouldn't be in your report.

-   Unchecking the All box will result in the first item in the list being selected.
    

## Displaying Multi-Select Option Values in a Report Footer {#bridgehead_N734531}

Each multi-select option displays one of the following values in the report footer:

1.  **All** - the All box is checked and all possible values in the list will be included in the report (the default setting).
    
2.  **Multiple** - This means you've picked more than one value (maybe even all). (See the note above about the difference between checking the All box and picking all values by hand.) You can hover over the box to see a list of everything you selected.
    
3.  **Selected value** - if only 1 value has been selected then it will be displayed in the option box.
    
    ![Choosing multiple classes in the report footer.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/multiple1.png)

In the previous screenshot only the Legal, New Business, and New Business: Medium classes will appear in the report.

All multi-select options in standard reports have the operator 'any of' after the field name. This means any record matching any of the selected values will be included in the report. In custom reports, you can create multi-select options with different operators.

### Related Topics

-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720282.html)
-   [Choosing Whether to Display a Report Title](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725695.html)
-   [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html)
-   [Behavior Descriptors for Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4125904112.html)
-   [Date Range Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4083697063.html)
-   [Date As Of Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4125897839.html)
-   [Period Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4084585701.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
