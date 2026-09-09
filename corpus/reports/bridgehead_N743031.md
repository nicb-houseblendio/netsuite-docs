---
id: "bridgehead_N743031"
type: "bridgehead"
title: "Updating of Custom Date Range Filters"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Filtering Data on Reports > Customizing Report Date Range Filters > Updating of Custom Date Range Filters"
parent: "section_N742889"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N743031.html"
anchors: []
sha256: "1ad73c28a339f35551d84d3e7e8b6814c17d65d7ac0d72be0e354e6ea7d3f9cf"
---

Custom report date range filters that use BETWEEN and a relative date are calculated dynamically based on the current date when you run the report. This automatic updating overwrites the values you selected when you first customized the report. However, when you show the custom date range filter in the report footer and the user selects refresh, the operator changes to CUSTOM, and the values update to what you originally selected.

When you define a custom date range filter such as 'this week', the report data filters by the dates in the From and To fields. The report keeps using those dates over time. For example, if you set the following filter for 'this week', the report returns the current week's data until 8/2/2014. After that date, you need to update the filter to the following week's dates. Otherwise, the report continues to show results for 7/27/14-8/2/14.

![Example of setting the date range filter as 'this week'.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/thisweek.png)

Note:

If you filter a report for a specific date or period range, results may differ for users in other time zones. Reports follow the time zone preferences you set at _Setup > Company > Preferences > General Preferences_ or _Home > Set Preferences_ when calculating report date fields with timestamps. Report results for these fields use company or user time zone, not system time zone.

### Related Topics

-   [Customizing Report Date Range Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N742889.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
