---
id: "section_N1430227"
type: "section"
title: "Generating Revaluations"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Generating Revaluations"
parent: "section_N1428662"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html"
anchors: ["procedure_N1430522"]
sha256: "27b499beca56d4f6307b7c1cb2845f3c6d58e924e1f46db6430d88d22fd5e273"
---

At the end of each accounting period, you generate currency revaluation transactions for open customer and vendor transactions, foreign-currency-denominated accounts, and other non-equity balance sheet accounts. Revaluations apply exchange rates as of the last day of the accounting period to calculate gain or loss.

NetSuite automatically calculates and posts exchange rate gain or loss when users apply a payment or credit memo to an invoice. For more information about the automatic process, see [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html).

Generating revaluations requires the Create level for the Transaction permission Currency Revaluation. To access the revaluation task from the Period Close Checklist, you must have the Manage Accounting Periods permission. To complete this task for a locked period, you must have the Override Period Restrictions permission.

The revaluation process sometimes needs to delete previous revaluation transactions to complete the current revaluation. Deletion requires the Currency Revaluation transaction permission at the Full level. If you don't have Full level access, you receive a message that lists the revaluation transactions that need to be deleted. Another user with Full level access must delete the transactions so you can rerun the process. Alternatively, you can have a user with Full level access rerun the process for you.

The Accounting Periods feature must be enabled in your account before you generate revaluations. Accounting periods are required to properly post open balance revaluations at the end of each accounting period. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).

Important:

Running revaluation can impact the revaluation calculations in subsequent periods. If you reopen a period, post changes, and rerun its revaluation after later periods have been closed, you must rerun revaluation for all the later periods. For an example, see [Revaluation in Reopened Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1432098.html).

#### To generate period close revaluations: {#procedure_N1430522}

1.  Go to _Transactions > Financial > Revalue Open Currency Balances_.
    
    You can also access this page from the **Revalue Open Foreign Currency Balances** task on the Period Close Checklist. For information about required tasks for closing periods, see [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html).
    
2.  Select a **Posting Period**.
    
    Transactions to be revalued are determined by the transaction period. If you open this page from the Period Close checklist, you can't change the posting period. When you use the menu link, this field defaults to the current period, but you can change it to any other open period.
    
3.  If you use Multi-Book Accounting, select an **Accounting Book** from the list.
    
    Month-end currency revaluation is book specific. The accounting book you select determines which subsidiaries are available in the **Subsidiary** list.
    
4.  If you have a OneWorld account, select a **Subsidiary**.
    
    If you want to run month end currency revaluation for multiple subsidiaries at one time, check the **Include Children** box. For more information, see [Foreign Currency Revaluation for Multiple Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4169300609.html).
    
5.  Enter a **Memo** (optional).
    
6.  Use the **Class**, **Department**, **Location**, and custom segment lists to filter the list of accounts that are displayed for selection for revaluation.
    
    For example, if you select Class A in the **Class** filter, only accounts that are restricted to this class are displayed in the list. For more information about restricting accounts, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).
    
    If you check the **Include Children** box, **Class**, **Department**, **Location**, and custom segment filters are disabled.
    
7.  Check **Match Source Classification** to generate a currency revaluation for each combination of classifications (class, department, location, and custom segment with GL impact).
    
    The classification grouping applies only to Open Receivables and Open Payables revaluations. The classification values are copied to the GL Impact lines for each currency revaluation transaction. For more information, see [Classifications and Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430408.html).
    
    Note:
    
    When classifications are required and the box is checked, a missing classification value in a source transaction causes an error that ends the revaluation process.
    
8.  For **Account Type**, select the type of account you want to revalue. Select **All** to list all accounts.
    
    When the **Include Children** box is checked, **Account Type** is called **Account Category**.
    
9.  Check the box in the **Include** column for the accounts you want to revalue.
    
    Alternatively, click **Mark All** to include all accounts, or click **Unmark All** to clear the check boxes for all accounts.
    
    If you check the **Include Children** box, this step doesn't apply because individual accounts aren't listed. All the accounts in the selected **Account Category** are included.
    
10.  Click **Save** to run the revaluation process for the selected period and accounts.
     
     You must wait for the process to finish or submit a different combination of posting period, subsidiary, accounting book, and account. If you resubmit the same combination of criteria before the first process finishes, you receive an error.
     
     The maximum number of lines in a currency revaluation is 2,000. Open Receivables and Open Payables are included in a separate currency revaluation transaction from Other Accounts. For more information about line limitations in NetSuite, see [Line Limitations for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159361099314.html).
     
     The total variance amount for each currency revaluation transaction created is posted to the Unrealized Gain/Loss account.
     

To review completed revaluations, go to _Transactions > Financial > Revalue Open Currency Balances > List_. You can also review completed revaluations from the Period Close Checklist using the Results subtab of the Task: Revalue Open Currency Balances page. For more information, see [Viewing Revaluation Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430727.html).

### Related Topics

-   [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html)
-   [Types of Accounts That Can Be Revalued](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428933.html)
-   [Unrealized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1437432.html)
-   [Revaluation Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1431203.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
