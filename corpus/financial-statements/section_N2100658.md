---
id: "section_N2100658"
type: "section"
title: "Balance Sheet Detail Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Balance Sheets > Balance Sheet Detail Report"
parent: "section_N2098170"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2100658.html"
anchors: ["bridgehead_N2101090"]
sha256: "1791842f17e20b4f74dd2c696d38ca69335a4f77e67dea24e5770716a912c721"
---

The Balance Sheet Detail report shows the starting balance at the beginning of a specified time period, transactions entered in the account for the time period you select, and the ending balance as of the report end date.

The standard Balance Sheet Detail report includes the following rows:

-   **ASSETS (header row)**
    
    -   Current Assets (header row)
        
        -   Bank (financial section)
            
        -   Accounts Receivable (financial section)
            
        -   Unbilled Receivable (financial section)
            
        -   Other Current Asset (financial section)
            
    -   Total Current Assets (summary row)
        
    -   Fixed Assets (financial section)
        
    -   Other Assets (financial section)
        
-   **Total ASSETS (summary row)**
    
-   **LIABILITIES & EQUITY (header row)**
    
    -   Current Liabilities (header row)
        
        -   Accounts Payable (financial section)
            
        -   Credit Card (financial section)
            
        -   Other Current Liability (financial section)
            
    -   Total Current Liabilities (summary row)
        
    -   Long Term Liabilities (financial section)
        
    -   Equity (header row)
        
        -   Equity (financial section)
            
        -   Retained Earnings (header row)
            
        -   Total Retained Earnings (summary row)
            
        -   Net Income (referenced row from Income Statement)
            
        -   Cumulative Translation Adjustment (financial section)
            
            (OneWorld accounts with multi-currency enabled only)
            
    -   Total Equity (summary row)
        
-   **Total LIABILITIES & EQUITY (summary row)**
    

Header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. Standard section data are selected based on accounts and are grouped by accounts.

The Balance Sheet Detail report may display a **Split** column. The **Split** column displays the other account involved in the double-entry bookkeeping notation. If more than one account was used to offset this distribution, you see the notation **\-Split-** in the **Split** column.

The account you see in the **Split** column depends on how you view the reports:

-   If the main line account is in the Financial Row column, you'll see the other account used in the transaction.
    
-   If the main line account isn't in the Financial Row column, you'll see the main line account used in the transaction.
    

Note:

The main line refers to the **Primary Information** field group in a transaction.

You can customize the Balance Sheet Detail report in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can set formatting options for each row. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). Be aware that the Allow Web Query option isn't available for this report.

If employee information is masked and you require this information, contact your account administrator.

Note:

All balance sheet accounts that have the Eliminate Intercompany Transactions box checked are used exclusively for intercompany posting. Consequently, you can't post a non-intercompany balance to an Other Current Asset account if the account Eliminate Intercompany Transactions box is checked. In this case, you must have separate balance sheet accounts to post intercompany and non-intercompany transactions. The impacted balance sheet accounts include A/R, A/P, Other Current Asset (excluding inventory account), Other Current Liability, Long Term Liability, Other Asset, Deferred Expense, and Deferred Revenue. Further, the elimination Journal Entry is automatically reversed in the beginning of next period. Therefore, the month-end auto-elimination will be calculated using the latest exchange rate, and on top of the total open balance of the account.

## To see a Balance Sheet Detail report: {#bridgehead_N2101090}

Go to _Reports > Financial > Balance Sheet > Detail_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from filter lists to refilter report data. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Report by Period user preference determines whether report data is calculated by date range or by period. This preference is available at _Home > Set Preferences_ on the Analytics subtab. To display this report's data by date range, set this preference to Never. To display this report's date range by period, set this preference to All Reports, or to Financials Only. For more information, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).

### Related Reports

-   [Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2098310.html)
-   [Comparative Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2101379.html)
-   [Multi-Book Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495037141.html)
-   [Multi-Book Balance Sheet Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495119693.html)
-   [Multi-Column Balance Sheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2102164.html)

### Related Topics

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
