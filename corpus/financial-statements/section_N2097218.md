---
id: "section_N2097218"
type: "section"
title: "Budget vs. Actual Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Income Statements > Budget vs. Actual Report"
parent: "section_N2093380"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2097218.html"
anchors: ["bridgehead_N2097511"]
sha256: "24867112f4eaf0c4d4af7578f5540def29e0ebd3e334f92ad2d9d7ac0e7f455c"
---

The Budget vs. Actual report combines an income statement with a budget income statement for the same set of criteria including both dollar and percentage comparisons between the two. This report lets you analyze budgeted and actual financials to determine how closely your income and expenses compare to those you originally budgeted.

You can use this report to compare budgeted and final amounts associated with your statistical accounts. For example, you can enter a budget for the headcount statistical account that specifies the number of new employee requisitions for the Sales Department in the upcoming financial year. To view the comparison, customize the report by inserting a row or section for your statistical account. You can view the report for the total amount as well as by classification segments defined in your budget. For more information, see [Using Statistical Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3841945149.html) and [Budgets in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1503165.html).

Because budgets are set up by period, this report doesn't display budget data accurately if the Report by Period preference is set to Never. If your report's budget columns are displaying zeros, go to _Home > Set Preferences_, and on the Analytics subtab, set the Report by Period preference to All Reports, or to Financials Only.

The standard Budget vs. Actual report includes the following rows, with columns for amount, budget amount, dollars that the amount is over budget, and amount as a percentage of budget.

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
    

The Amount Over Budget and % of Budget columns are formulas based on the first two columns. You can review how these formulas are defined on the Edit Columns page of the Financial Report Builder.

Header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. The Net Income row is a formula row that sums Net Ordinary Income with Net Other Income. Standard section data are selected based on account type and are grouped by account. The date you select in the footer is used to filter the column you want to compare.

You can customize the Budget vs. Actual report in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can use dynamic criteria other than account type for section data, including account name, account number, class, department, location, and if you're using NetSuite OneWorld, subsidiary. In addition to account type, you can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). The Allow Web Query option isn't available for this report.

Note:

Custom segments aren't included in the Budget and Financial fields of the Financial Report Builder for budget-related reports.

## To see the Budget vs. Actual report: {#bridgehead_N2097511}

Go to _Reports > Banking/Budgeting > Budget vs. Actual_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from filter lists to refilter report data. You can also select from the Column list to display report amounts by an additional dimension, including time period, class, department, location, or, if you're using NetSuite OneWorld, subsidiary. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Budget vs. Actual report may be run on a cash basis. The Cash Basis Reporting preference applies to all standard reports that support cash basis reporting. This preference is on the General tab under General Ledger at _Setup > Accounting > Preferences > Accounting Preferences_. If the preference is enabled, the Income Statement Detail is on a cash basis rather than an accrual basis. If this preference isn't enabled, you can create a custom cash basis Budget vs. Actual by enabling the Cash Basis option on the More Options page of the Financial Report Builder. See [Setting Up Cash Basis Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html).

Note:

Click an Account Name to view General Ledger report data for the account. The data in the **General Ledger Balance** column may vary from data in the **Budget vs. Actual Amount** column. This difference occurs because the **Amount** column is the account balance from the specified report period only. The **Balance** column is a running account balance that includes the amount from the prior period as a beginning balance.

### Related Reports

-   [Generating an Insight on a Budget vs. Actual](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0217072902.html)
-   [Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2093552.html)
-   [Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2094110.html)
-   [Comparative Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095037.html)
-   [Multi-Book Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495034629.html)
-   [Multi-Book Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495115536.html)
-   [Budget Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095701.html)
-   [Budget Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2096390.html)

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
