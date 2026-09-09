---
id: "section_N725800"
type: "section"
title: "Choosing a Date or Period Range for a Report"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Working with Report Results > Setting Report Footer Options > Choosing a Date or Period Range for a Report"
parent: "section_N720025"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html"
anchors: ["procedure_N725928"]
sha256: "1e3b3c80e7d44330b649af0f6f910bc037682e6f88242782626305f7f73531d9"
---

When you run a NetSuite report, you can filter its data to show only transactions that fall within a predefined date or period range, or define a custom range.

**Date, From**, and **To** dropdown lists display in the footer of most report results pages. When you make a selection from the **Date** dropdown list, **From** and **To** values are populated automatically. You can also choose (Custom) in the **Date** field and enter **From** and **To** dates manually.

![Example of choosing the date range for a report.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/date1.png)

For certain types of reports, **End Of** and **As Of** fields replace the **Date**, **From** and **To** fields, or both, to fit better in the context of reports.

For reports that use accounting periods, a **Period** field is available instead of a Date field. You can define which reports use periods by setting the **Report by Period** preference at _Home > Set Preferences_, on the Analytics subtab. The possible settings are **All Reports**, **Financials Only**, and **Never**. The **Financials Only** setting gives you the ability to display financial statement data by accounting period and at the same time enables you to set other date ranges for other types of reports.

Note:

In Trial Balance reports, you need to turn off the **Report by Period** preference to use custom date filters. For more information, see [Trial Balance Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1520986.html).

For tables of available date ranges and periods for reports, see the following:

-   [Date Range Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4083697063.html)
    
-   [Date As Of Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4125897839.html)
    
-   [Period Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4084585701.html)
    

You can customize a report to compare values across different time periods by adding multiple columns for the same field and setting a different date range for each column. See [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html).

The **Period** field contains options which indicate a specific period range. The **End of** field isn't renamed when accounting periods are used.

#### To select date options for your report: {#procedure_N725928}

1.  Click the **Reports** tab.
    
2.  On the Reports page, click the name of the report you want to view.
    
3.  When the report opens, select a date option in the **Date**, **End of**, or **Period** field.
    
4.  Click **Refresh**.
    

Note:

When you view a report filtered for a specific date or period, it might show different data depending on the time zone where the data was entered. Reports respect time zone preferences set at _Setup > Company > Preferences > General Preferences_ or _Home > Set Preferences_ > General when calculating report date fields that include timestamps. Report results for these fields are based on your company or user time zone, not the system time zone.

### Related Topics

-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720282.html)
-   [Choosing Whether to Display a Report Title](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725695.html)
-   [Behavior Descriptors for Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4125904112.html)
-   [Date Range Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4083697063.html)
-   [Date As Of Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4125897839.html)
-   [Period Selectors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4084585701.html)
-   [Using Multi-Select Options in Report Footer Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734449.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
