---
id: "section_N1520986"
type: "section"
title: "Trial Balance Report"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting-Related Reports > Financial Reports > Trial Balance Report"
parent: "section_N1520496"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1520986.html"
anchors: ["procedure_N1521800"]
sha256: "1bb69722f32c817db5e3e46e5614aa40bf3bfe644674f481c67eb190b3efb1cf"
---

The Trial Balance is a report that shows the balance of each active account as of a specified date, usually the end of the month. Account balances are shown in debit and credit columns. An accountant runs this report before preparing financial statements to make sure the debits and credits are equal. When the trial balance is in balance, the financial statements can be prepared.

The table below shows the account types on the trial balance report and whether they represent a credit or debit on the report.

| **Account Type** | **Debit** | **Credit** |
| --- | --- | --- |
| Bank | X |  |
| Accounts Receivable | X |  |
| Other Current Asset | X |  |
| Fixed Asset | X |  |
| Other Asset | X |  |
| Accounts Payable |  | X |
| Credit Card |  | X |
| Other Current Liability |  | X |
| Long Term Liability |  | X |
| Equity |  | X |
| Income |  | X |
| Cost of Goods Sold | X |  |
| Expense | X |  |
| Other Income |  | X |
| Other Expense | X |  |
| Deferred Revenue |  | X |
| Deferred Expense | X |  |
| Unbilled Receivable |  | X |
| Non-posting |  |  |

Important:

Some user roles such as Finance Manager are restricted by location to Own, Unassigned, and Subordinate. The Trial Balance report isn't restricted by location, but users with location-restricted roles may see an imbalance in the report. The reason for an imbalance is that within a single transaction some transaction lines may be set to an accessible/non-accessible location. Any resulting credit/debit imbalance is reported in the Cumulative Translation Adjustment line. Users should run reports using and unrestricted role.

## To see the Trial Balance report: {#procedure_N1521800}

Go to _Reports > Financial > Trial Balance_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

If employee information is masked and you require this information, contact your account administrator.

In the report, you can click an account name to see details about the account. You can click the dollar amount listed for an account to view an account detail report of recent transactions. See [Account Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1522428.html).

Some differences between amounts in the Trial Balance and in the account detail reports may occur as follows:

-   For income statement accounts (Income, Expense, Other Income, Other Expense, and Cost of Goods Sold), the Trial Balance report includes only transactions posted from the beginning of the calendar year up to the As of date for these types of accounts. The account detail reports for these account types also include the balance for transactions posted prior to the beginning of the calendar year.
    
-   Retained earnings are reported in the Trial Balance report as the sum of cumulative net income and amounts posted directly to the retained earnings account through journal entries. The cumulative net income is a calculated reporting value that's not recorded in the account register detail report.
    

The following filters are available in the report footer. Select from these filters, and then click Refresh to modify report results.

-   **Column** - you can switch the columns displayed in the report.
    
    -   Debit/Credit - to display two columns, with debit and credit balances, for each account
        
    -   Total - to display one column with balance of debits and credits for each account
        
-   **Date or Period** - you can change the date or period for report data.
    
    Whether Date or Period is used depends on your **Report by Period** preference at _Home > Set Preferences_, on the Analytics tab.
    
    For more information about this preference, see [Analytics Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N481482.html).
    
    Note:
    
    If you've enabled the **Report by Period** preference, you can't apply custom date filters. To filter by date, you need to disable the **Report by Period** preference first.
    
    For information about setting dates or periods for reports, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).
    
-   **As of** - displays the date corresponding to your selection in the Date or Period filter. You also can enter a date directly into this field to set a custom Date or Period.
    
    Be aware that this report handles the reporting of posted transaction data differently for different types of accounts. For example, if the **As of** date for a Trial Balance report is **12/31/2009**:
    
    -   For Income, Expense, Other Income, Other Expense, and Cost of Goods Sold (COGS) type accounts, the report includes only transactions posted from 1/1/2009 to 12/31/2009. It doesn't include transactions posted prior to 1/1/2009.
        
    -   For the Retained Earnings account, the report includes all transactions posted on or before 12/31/2009, plus Net Income posted on or before 12/31/2008.
        
    -   For all other types of accounts, the report includes all transactions posted on or before 12/31/2009.
        
-   **Subsidiary Context** - (OneWorld only) You can filter the report to show only data from the subsidiary you select, or for consolidated subsidiaries, to show data for all child subsidiaries of the consolidated parent subsidiary.
    
    Note:
    
    The Subsidiary Context list includes active subsidiaries and inactive subsidiaries with posted transactions. Inactive subsidiaries without posted transactions are hidden.
    
    When the **Subsidiary Context** is a consolidated subsidiary, a line Cumulative Translation Adjustment (CTA) account may appear at the end of the account listing. For more information about this account, see [Cumulative Translation Adjustment (CTA) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124272.html).
    
    If you've posted manual journal entries to the CTA account, a separate Cumulative Translation Adjustment account line displays the balance from manual journal entries. This line appears with other equity account type lines within the report.
    
    The primary CTA account line at the end of the account listing includes both the manual journal entries and the calculated CTA. Only the primary CTA line is counted in the total. See [Cumulative Translation Adjustment (CTA) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124272.html).
    
    If the **Subsidiary Context** is **not** a consolidated subsidiary, the transaction exchange rate used to convert from the transaction currency to the subsidiary base currency.
    

### Related Reports

-   [Generating an Insight on a Trial Balance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0217075051.html)
-   [General Ledger Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1520771.html)
-   [Account Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1522428.html)
-   [GL Audit Numbering Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739913944.html)

### Related Topics

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N698474.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
