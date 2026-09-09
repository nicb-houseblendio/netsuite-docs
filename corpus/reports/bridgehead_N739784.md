---
id: "bridgehead_N739784"
type: "bridgehead"
title: "Standard Report Alternate Ranges Are Relative to Report Date"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Adding, Removing, or Reordering Report Columns > Adding Time-Based Comparison Columns to Reports > Standard Report Alternate Ranges Are Relative to Report Date"
parent: "section_N739328"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N739784.html"
anchors: []
sha256: "2393fcd6f9fe4f2f6d708141d20a83631c256148eb0b7fd337fd92bb655f04a4"
---

Any standard report column with an alternate date range uses the of **Relative to report date** type, so that when you change the main report date or period range, the alternate range for the comparison column updates automatically.

The following standard report columns have columns with alternate ranges defined:

| Report | Column | Notes |
| --- | --- | --- |
| Comparative Balance Sheet | Comparison Amount | \- |
| Comparative Income Statement | Comparative Amount | \- |
| Comparative Sales | Revenue Comparison | This report is available from the related report snapshot. |
| Comparative Sales (Orders) | Amount Comparison | This report is available from the related report snapshot. |
| Comparative Sales (Orders Alt. Sales) | Alt. Sales Amount Comparison | This report is available from the related report snapshot. |

Important:

Any custom report column with an alternate date or period range defined before 2010.1 keeps its previous behavior and now has an alternate range type of **Relative to today's date**. This range uses the current date when the report runs, and doesn't change if you adjust the report range. If you want a custom report column to use the new relative alternate date range functionality, edit the customized report. On the Edit Columns page, select the column, set the Alternate Range Type to **Relative to report date**, and edit the Alternate Range field as needed.

### Related Topics

-   [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
