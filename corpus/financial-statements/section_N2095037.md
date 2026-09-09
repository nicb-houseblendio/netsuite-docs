---
id: "section_N2095037"
type: "section"
title: "Comparative Income Statement Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Income Statements > Comparative Income Statement Report"
parent: "section_N2093380"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095037.html"
anchors: ["bridgehead_N2095317"]
sha256: "6f9f610d98321c22fcd501185c838545c8b27dbd7ada28ba522c01c497938f6c"
---

The Comparative Income Statement report summarizes and compares income and expenses across two or more specified time periods. You can use this report to compare your company's performance with previous years. This comparison helps you to measure your company's progress and to make future projections.

This report includes an Amount column that defaults to the current date range or period and a Comparative Amount column that defaults to the last year or last fiscal year. When you change the date or period in the Date footer filter to change the date or period for Amount column data, the range for the Comparative Amount column changes accordingly because it has a relative alternate range defined. For an explanation about alternate date ranges, see [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html).

The standard Comparative Income Statement includes the following rows:

-   **Ordinary Income/Expense** (header row)
    
    -   **Income** (financial section)
        
    -   **Cost of Sales** (financial section)
        
    -   **Gross Profit** (formula row)
        
    -   **Expense** (financial section)
        
-   **Net Ordinary Income** (summary row)
    
-   **Other Income and Expenses** (header row)
    
    -   **Other Income** (financial section)
        
    -   **Other Expenses** (financial section)
        
-   **Net Other Income** (summary row)
    
-   **Net Income** (formula row)
    

Header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. The Net Income row is a formula row that sums Net Ordinary Income with Net Other Income. Standard section data are selected based on account type and are grouped by account. The date you select in the footer is used to filter the column you want to compare.

You can customize the Comparative Income Statement report in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can use dynamic criteria other than account type for section data, including account name, account number, class, department, location, and if you're using NetSuite OneWorld, subsidiary. In addition to account type, you can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can change the date range for your comparison column by editing the Date filter. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html) . Be aware that the Allow Web Query option isn't available for this report.

## To see the Comparative Income Statement report: {#bridgehead_N2095317}

Go to _Reports > Financial > Comparative Income Statement_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from filter lists to refilter report data. You can also select from the Column list to display report amounts by an additional dimension, including time period, class, department, location, or, if you're using NetSuite OneWorld, subsidiary. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Report by Period user preference determines whether report data is calculated by date range or by period. This preference is available at _Home > Set Preferences_, on the Analytics subtab. To display this report's data by date range, set this preference to Never. To display this report's date range by period, set this preference to All Reports, or to Financials Only. For more information, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).

The Comparative Income Statement report may be run on a cash basis. The Cash Basis Reporting preference applies to all standard reports that support cash basis reporting. This preference is on the General tab under General Ledger at _Setup > Accounting > Preferences > Accounting Preferences_. If the preference is enabled, the Income Statement Detail is on a cash basis rather than an accrual basis. If this preference isn't enabled, you can create a custom cash basis Comparative Income Statement by enabling the Cash Basis option on the More Options page of the Financial Report Builder. See [Setting Up Cash Basis Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html).

Note:

Click an Account Name to view General Ledger report data for the account. The data in the **General Ledger Balance** column may vary from data in the **Comparative Income Statement Amount** column. This difference occurs because the **Amount** column is the account balance from the specified report period only. The **Balance** column is a running account balance that includes the amount from the prior period as a beginning balance.

### Related Reports

-   [Generating an Insight on a Comparative Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0217065136.html)
-   [Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2093552.html)
-   [Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2094110.html)
-   [Multi-Book Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495034629.html)
-   [Multi-Book Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495115536.html)
-   [Budget Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095701.html)

### Related Topics

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html)
-   [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
