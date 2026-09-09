---
id: "section_N2095701"
type: "section"
title: "Budget Income Statement Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Income Statements > Budget Income Statement Report"
parent: "section_N2093380"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095701.html"
anchors: ["bridgehead_N2096013"]
sha256: "124ffbafa81a473fba646bb9fe5893079a091ba483fa3a04541f7cef67bd901d"
---

The Budget Income Statement lets you view a specific budget for income, cost of goods sold, and expense accounts in the same format as your income statement. This includes your projected net income per that budget.

Because budgets are set up by period, this report doesn't display budget data accurately if the Report by Period preference is set to Never. If your report's budget columns are displaying zeros, go to _Home > Set Preferences_, and on the Analytics subtab, set the Report by Period preference to All Reports, or to Financials Only.

The standard Budget Income Statement includes the following rows:

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
    

Header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. The Net Income row is a formula row that sums Net Ordinary Income with Net Other Income. Standard section data are selected based on account type and are grouped by account.

You can customize the Budget Income Statement report in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can use dynamic criteria other than account type for section data, including account name, account number, class, department, location, and if you're using NetSuite OneWorld, subsidiary. In addition to account type, you can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can set formatting options for each row. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). The Allow Web Query option isn't available for this report.

Note:

Custom segments aren't included in the Budget and Financial fields of the Financial Report Builder for budget-related reports.

Also, you can add a Percent of Expense or Percent of Income column to your Income Statement. See [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html) or [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html).

## To see the Budget Income Statement: {#bridgehead_N2096013}

Go to _Reports > Banking/Budgeting > Budget Income Statement_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from filter lists to refilter report data. You can also select from the Column list to display report amounts by an additional dimension, including time period, class, department, location, or, if you're using NetSuite OneWorld, subsidiary. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Budget Income Statement report may be run on a cash basis. The Cash Basis Reporting preference applies to all standard reports that support cash basis reporting. This preference is on the General tab under General Ledger at _Setup > Accounting > Preferences > Accounting Preferences_. If the preference is enabled, the Income Statement Detail is on a cash basis rather than an accrual basis. If this preference isn't enabled, you can create a custom cash basis Budget Income Statement by enabling the Cash Basis option on the More Options page of the Financial Report Builder. See [Setting Up Cash Basis Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html).

### Related Reports

-   [Budget Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2096390.html)
-   [Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2093552.html)
-   [Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2094110.html)
-   [Comparative Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095037.html)
-   [Multi-Book Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495034629.html)
-   [Multi-Book Income Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495115536.html)
-   [Budget vs. Actual Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2097218.html)

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
