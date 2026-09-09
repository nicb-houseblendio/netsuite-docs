---
id: "section_N1457773"
type: "section"
title: "Year-End Closing"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Year-End Closing"
parent: "chapter_N1445226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457773.html"
anchors: ["bridgehead_4279831998", "bridgehead_N1458419", "bridgehead_N1458483"]
sha256: "5e776eb33b907e5d507dbac1fecca0e5dd8ffade0c64d2eeed41f9035c22e7e0"
---

Closing the books for a year ends the opportunity to post entries to the sub-ledgers and general ledger to transfer net income to retained earnings (for a corporation) or to owner's equity (for an individual proprietorship).

To perform year-end closing, go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.

Using NetSuite financials, you're **not required** to make journal entries to close out the income statement to retained earnings. You can choose to do one of the following:

-   **Automatic Close** - Allow NetSuite to automatically close year end so that your books reflect the correct balance in retained earnings based on the dates you select on the balance sheet. This method is **strongly** recommended. For more information, see [Automatic Close](#bridgehead_N1458419).
    
-   **Manual Close** - Manually close income statement accounts to the balance sheet by making journal entries to close accounts. For more information, see [Manual Close](#bridgehead_N1458483).
    

## Preparing for Year-End Closing {#bridgehead_4279831998}

Be aware of the following as you prepare for year-end closing:

-   Before year-end close, you should close all of the periods included in the year.
    
    -   A checklist of required tasks is provided to guide you through the closing process for each period. See [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html).
        
    -   If you use multiple currencies, you should revalue open currency balances for each period before you close it. See [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html).
        
    -   it's important to understand the difference between closing a period and locking transactions for a period.
        
        -   Closing a period prevents postings for any dates included in the period, by anyone, and should be the final step after a process of accounts review and reconciliation.
            
        -   Locking transactions for a period prevents users without override permission from posting to the period, and is a preliminary task before closing occurs.
            
            For more information, see [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html).
            
-   If you use NetSuite for payroll processing, you must complete additional payroll tasks before year-end close. See [Complete Quarterly or Yearly Payroll Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N954521.html).
    

Important:

it's recommended that you consult with your accountant to ensure that your books fulfill all legal requirements.

## Automatic Close {#bridgehead_N1458419}

When you permit NetSuite to automatically close year end, financial statement figures display as if the accounts had been closed, based on the period or periods you select for reports. **you're not required to perform a formal year-end closing. NetSuite automatically closes year-end after you close all of the periods in your year.**

To permit NetSuite to automatically perform year-end closing, go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_. Perform the required tasks noted in [Preparing for Year-End Closing](#bridgehead_4279831998), referring to the noted topics for specific details.

By using this method, your general ledger ties to financials for the same periods run for all accounts, with the exception of the retained earnings account. The system posts a placeholder entry to the retained earnings account on the balance sheet to reflect the income for the period run.

For example, if you want to see a balance sheet for the fiscal year 2013, NetSuite assesses the cumulative net income though 2013 and displays that value in the retained earnings account for reporting purposes. Similarly, if you run a balance sheet for fiscal year 2012, NetSuite assesses the cumulative net income from 2011 and 2012 to determine the retained earnings balance.

NetSuite **doesn't post** the balance to retained earnings because doing so would zero the past income statements and prevent them from being viewed.

On your balance sheet, the retained earnings account and the net income account together make up your cumulative retained earnings balance at any point in time.

Net income from **prior** fiscal year is displayed in the **retained earnings** account.

Net income from the **current** fiscal year-to-date is displayed in the **net income** account.

The retained earnings account is a system account and can't be deleted or substituted with another account. If you must adjust retained earnings or allocate the balance to other equity accounts, you can post a journal entry and it's reflected on the balance sheet.

Adjustments to the retained earnings account are combined on the balance sheet along with other account figures. For example, if your net income for 2013 was $100,000 and you made a journal entry that debited retained earnings $10,000 in 2013, your fiscal year 2013 balance sheet displays a $90,000 credit, assuming it was your first year in business.

## Manual Close {#bridgehead_N1458483}

If you want to start the new fiscal year with a zero net income, go to _Transactions > Financial >Make Journal Entries_ to create journal entries that zero out your income and expense accounts, and transfer the balance to a retained earnings account.

Warning:

Be aware that the manual close method isn't recommended. If you must record entries in the general ledger at year end, consider using the Period End Journal Entries feature. For information, see [Period End Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531269686.html).

### Related Topics

-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)
-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html)
-   [Searching by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459178.html)
-   [Locking Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560870.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
