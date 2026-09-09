---
id: "section_N3949039"
type: "section"
title: "SuiteAnalytics"
branch: "release-notes"
category: "what-s-new"
breadcrumb: "What's New > Release Notes > NetSuite 2026.2 Release Notes > SuiteAnalytics"
parent: "article_72152418635"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3949039.html"
anchors: ["subsect_45100402416", "subsect_0603014058"]
sha256: "c08b4348ff64b2a4ef65ad38e32161b35790dec214865c3bab1e611d2e0dd6e3"
---

SuiteAnalytics is a feature area that includes NetSuite Analytics Warehouse, Connect, Workbook, Searches, Reports, and Dashboards.

NetSuite 2026.2 includes the following enhancements to SuiteAnalytics:

-   [Change to Default Sorting for SuiteQL Queries and Analytics Datasets](#subsect_45100402416)
    
-   [Export Lists, Saved Searches, and Reports to .xlsx](#subsect_0603014058)
    
-   [Transfer Saved Searches to NetSuite Analytics Warehouse](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1140446525.html#subsect_0601020515)
    
-   [Transfer Data from Salesforce Data Source](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1140446525.html#subsect_0616021340)
    

## Change to Default Sorting for SuiteQL Queries and Analytics Datasets {#subsect_45100402416}

With the NetSuite 2026.2 release, SuiteQL queries and Analytics datasets based on generic transactions use `Transaction.tranDate` as the default sort field when no sort order is specified. This change helps prevent performance issues.

Previously, these queries and datasets used `Transaction.tranDisplayName` as the default sort field.

This change may alter the order of returned results. Queries and datasets that specify a sort order are not affected. If result order is important, specify the required sort order.

For more information, see [SuiteQL Syntax and Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156257790831.html) and [Advanced Sorting Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544128698.html).

## Export Lists, Saved Searches, and Reports to .xlsx {#subsect_0603014058}

Before, when you exported lists, saved searches, and reports to Microsoft® Excel, the default format was .xls. Now, the format is .xlsx.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
