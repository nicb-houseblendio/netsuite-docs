---
id: "chapter_N2092547"
type: "chapter"
title: "Financial Statements Overview"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Statements Overview"
parent: "book_N2092473"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html"
anchors: ["bridgehead_4425151234"]
sha256: "b015e8bdde659496ee2d64442295c7739aa7ae28f86c02946545e028a45254e0"
---

You can access financial statements, including income statements, balance sheets, and cash flow statements, at Reports > Financial and at Reports > Banking/Budgeting. For a list of NetSuite standard financial statements, see [Available Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092953.html).

Important:

To access Financial Report Builder training resources, see the [SuiteAnalytics: Financial Reports and Searches](http://www.netsuite.com/portal/services/training/description-suite-analytics-financial-report.shtml) page at NetSuite SuiteTraining.

Financial statements differ in the following respects from other NetSuite reports that include financial data:

-   Financial statements group data by **financial sections**.
    
    Each section is a subset of financial data for which separate filters, grouping, and sorting can be defined. The use of sections allows more fine-grained organization of data than is available for other types of reports.
    
    Standard financial statement section data is filtered and grouped by accounts. You can modify the filtering, grouping, and display formats of custom financial statement section data.
    
    Financial sections can be reused across reports. The same section filter criteria can be used in multiple layouts, while section data is grouped and displayed differently.
    
    For more information, see [Financial Statement Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html).
    
-   Financial statements store report characteristics in **layouts**.
    
    A financial statement layout is a set of definitions for financial sections and rows. This includes report rows, row order and hierarchy, section filter criteria, calculating summary amounts methods, row labels, and text, line, and background formatting options.
    
    Layouts can be shared, to provide a consistent look among related reports. Reports with shared layouts display the same rows but can have different sets of columns and different filters.
    
    A standard layout is provided for each type of standard financial statement for each country. When you customize a financial statement, its standard layout is duplicated to provide a custom layout that you can edit. Most of your customizations, other than changes to columns and filters, are stored as part of this custom layout.
    
    For more information, see [Financial Statement Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2110511.html).
    
-   Financial statements have a unique customization interface, the Financial Report Builder.
    
    The Financial Report Builder includes the column and filter customization functions of the Report Builder, as well as many other capabilities. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html).
    

If you use NetSuite OneWorld, you can run and customize separate financial statements for each subsidiary. For more information, see [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html).

The currency used for financial statements is the base currency of the company. If you use NetSuite OneWorld, it's the base currency of the subsidiary selected as the Subsidiary Context. Like other reports, values in financial statement results are rounded to the currency precision determined by the format of the company currency. In NetSuite OneWorld, values in financial statements results are rounded to the currency precision determined by the format of the subsidiary base currency. This rounding applies to currency values and non-currency values, including formula column values.

## Permissions and Roles {#bridgehead_4425151234}

You need the Financial Statements permission to run financial statement reports. Additionally, you need the Report Customization permission to customize these reports in the Financial Report Builder or to change the layouts assigned to them.

The following standard NetSuite roles include both permissions:

-   Accountant
    
-   Accountant (Reviewer)
    
-   CEO
    
-   CEO (Hands Off)
    
-   CFO
    

If you don't have necessary permissions, contact your account administrator. For more information, see [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html).

If employee information is masked and you require this information, contact your account administrator.

### Related Topics

-   [Available Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092953.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html)
-   [Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N698474.html)
-   [Accounting-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1519116.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
