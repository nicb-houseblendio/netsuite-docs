---
id: "section_N1498385"
type: "section"
title: "Intercompany Elimination Overview"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Intercompany Elimination Overview"
parent: "chapter_N1486105"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html"
anchors: []
sha256: "e6db34599176a2628817f78a394a83820ebfc09650514e49a1c06d8adf6c9c2c"
---

When you enter intercompany transactions and advanced intercompany journal entries to record business activity between subsidiaries, the system identifies transaction lines that require elimination.

-   Intercompany sales and billing transaction lines are identified by default, based on the intercompany account with which the line is associated. An intercompany sales order is a nonposting transaction, a transaction that has no general ledger impact. However, when the sales order is invoiced, the system identifies the transaction lines that require elimination for posting to intercompany accounts. The same is true for intercompany purchase orders. An intercompany purchase order is a nonposting transaction. However, when the purchase order is billed, the system identifies transaction lines that require elimination for posting to intercompany accounts.
    
-   Intercompany inventory transfers and intercompany drop shipments are identified by default. They are based on the intercompany account associated with the line on related purchase orders and sales orders.
    
-   Journal lines that require elimination at period end are identified either by default. They are based on the intercompany account entered for the line, or by manually checking the line for elimination.
    

Note:

Lines with historical rates on accounts are eliminated only one time because historical rates do not change.

At the end of the accounting period, complete the tasks in your Period Close Checklist. The last task on the checklist is Eliminate Intercompany Transactions. You can complete this task only after completing the Revalue Open Foreign Currency Balances and Calculate Consolidated Balances tasks. You must complete these two tasks first to ensure that foreign currency adjustment amounts have been calculated for transactions in the period. See [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html).

When you run intercompany elimination, NetSuite creates elimination journal entries for all intercompany transaction journal lines that have the Elimination box checked. Adjustments that result from the difference in the foreign currency exchange rates post to the Cumulative Translation Adjustment-Elimination (CTA-E) account. These differences occur from the originating intercompany journal entry and the elimination journal entry. NetSuite also creates a reversing journal entry for all intercompany journal lines that post to Intercompany Receivables and Intercompany Payables. See [Cumulative Translation Adjustment-Elimination (CTA-E)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1498539.html).

If you use Multi-Book Accounting, you can run intercompany elimination on any accounting book.

Important:

The intercompany elimination process takes into account the unrealized gain and loss effect on Accounts Payable and Accounts Receivable accounts. During the auto-elimination process, lines related to currency revaluation of intercompany transactions are marked for elimination and considered accordingly.

To illustrate this, consider an example of an advanced intercompany journal. Suppose one of the lines posts 1000 CAD to the Intercompany Accounts Receivable account. Using an exchange rate of 0.9 USD/CAD, this amount is translated to the subsidiary's base currency (USD) as 900 USD.

However, by the time the currency revaluation process is run at month-end, the exchange rate has changed to 0.95 USD/CAD. Consequently, a currency revaluation transaction is posted, debiting 50 USD from the Intercompany Accounts Receivable account and crediting the Unrealized Gain and Loss account. This currency revaluation transaction is linked to the original intercompany transaction.

When the auto-elimination process runs, it considers both the original intercompany transaction (900 USD) and the linked currency revaluation transaction (50 USD) for elimination. Consequently, the auto-elimination process credits the Intercompany Accounts Receivable account for 950 USD. This takes into account the impact of both the intercompany transaction and the associated currency revaluation for that period.

### Related Topics:

-   [Key Points for Running Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1498454.html)
-   [Summarized Intercompany Elimination Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4813074258.html)
-   [Intercompany Elimination Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498982.html)
-   [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)
-   [Intercompany Sales and Billing Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492389.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)
-   [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html)
-   [Working with Elimination Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502129.html)
-   [Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1486105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
