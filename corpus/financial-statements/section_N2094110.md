---
id: "section_N2094110"
type: "section"
title: "Income Statement Detail Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Income Statements > Income Statement Detail Report"
parent: "section_N2093380"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2094110.html"
anchors: ["bridgehead_N2094419"]
sha256: "212a875b88eb0cc5731f28584ee3b2042cc75c968cba25fcd0516057d11f5dd9"
---

The Income Statement Detail report shows individual transactions for a specified time period for each income and expense account and the totals for each account and category.

The standard Income Statement Detail report includes the following rows:

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

The Income Statement Detail report may display a **Split** column. The **Split** column displays the other account involved in the double-entry bookkeeping notation. If more than one account was used to offset this distribution, you see the notation **\-Split-** in the **Split** column.

The account you see in the **Split** column depends on how you view the reports:

-   If the main line account is in the Financial Row column, you'll see the other account used in the transaction.
    
-   If the main line account isn't in the Financial Row column, you'll see the main line account used in the transaction.
    

Note:

The main line refers to the **Primary Information** field group in a transaction.

NetSuite doesn't write foreign currency amounts for cost of goods lines. Item Fulfillment and Item Receipt are noted in base currency only.

You can customize the Income Statement Detail report in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can use dynamic criteria other than account type for section data, including account name, account number, class, department, location, and if you're using NetSuite OneWorld, subsidiary. In addition to account type, you can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can set formatting options for each row. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). Be aware that the Allow Web Query option isn't available for this report.

Also, you can add a Percent of Expense or Percent of Income column to your Income Statement. See [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html) or [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html).

## To see the Income Statement Detail report: {#bridgehead_N2094419}

Go to _Reports > Financial > Income Statement > Detail_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. Click Cancel Report next to the status bar to stop the report from loading.

If employee information is masked and you require this information, contact your account administrator.

In the footer of the report, you can select from filter lists to refilter report data. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Report by Period user preference determines whether report data is calculated by date range or by period. This preference is available at _Home > Set Preferences_ on the Analytics subtab. To display this report's data by date range, set this preference to Never. To display this report's date range by period, set this preference to All Reports, or to Financials Only. For more information, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).

The Income Statement Detail report may be run on a cash basis. The Cash Basis Reporting preference applies to all standard reports that support cash basis reporting. This preference is on the General tab under General Ledger at _Setup > Accounting > Preferences > Accounting Preferences_. If the preference is enabled, the Income Statement Detail is on a cash basis rather than an accrual basis. If this preference isn't enabled, you can create a custom cash basis Income Statement Detail by enabling the Cash Basis option on the More Options page of the Financial Report Builder. See [Setting Up Cash Basis Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html).

Note:

Click an Account Name to view General Ledger report data for the account. The data in the **General Ledger Balance** column may vary from data in the Income Statement Detail Amount column. This difference occurs because the **Amount** column is the account balance from the specified report period only. The **Balance** column is a running account balance that includes the amount from the prior period as a beginning balance.

### Related Reports

-   [Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2093552.html)
-   [Comparative Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095037.html)
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
