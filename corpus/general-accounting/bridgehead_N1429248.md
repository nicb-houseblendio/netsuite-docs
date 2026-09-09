---
id: "bridgehead_N1429248"
type: "bridgehead"
title: "Residual Base Currency Balances and Base Currency Adjustments"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Types of Accounts That Can Be Revalued > Residual Base Currency Balances and Base Currency Adjustments"
parent: "section_N1428933"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1429248.html"
anchors: []
sha256: "884379263264d8846e5074ae85516738b5976fd9e547f381e10b93724569d0ed"
---

Running currency revaluation can produce residual base currency amounts in balance sheet accounts. Residual base currency account balances occur when the exchange rate at the time of payment (or zeroing the account) differs from the exchange rate of the initial transaction. Non-equity balance sheet accounts with base currency balances are subject to currency revaluation at the end of the period.

Base currency adjustments, a type of currency revaluation transaction, equalize foreign currency and base currency account balances and eliminate the continuous revaluation and reversal of residual amounts. Base currency adjustments apply to non-equity balance sheet accounts other than Accounts Receivable and Accounts Payable.

When you run currency revaluation at the end of a period, the steps of the revaluation process are as follows:

-   The process first checks account balances subject to revaluation, comparing the foreign currency (transaction currency) balances with their base currency balances.
    
    If the transaction currency balance for an account is 0 but the base currency balance isn't 0 (residual base currency balance):
    
    -   If this is the first time in the period that you've run revaluation, the process creates a base currency adjustment to clear the residual base currency amount. The base currency adjustment posts to the base currency account and to the Unrealized Matching Gain/Loss account.
        
        A base currency adjustment is created during revaluation whenever the process finds a residual base currency balance and no previous unrealized gain/loss in the period.
        
    -   If you're rerunning revaluation and the account already has unrealized gain/loss posted in the period, the process creates another unrealized gain/loss transaction to clear the residual base currency balance.
        
-   Next, the revaluation process creates currency revaluation transactions for all selected accounts if needed. Because the transaction currency balance and base currency balance are both 0 for accounts with the new base currency adjustments, currency revaluation isn't triggered again for those accounts.
    

If you rerun currency revaluation in the same period, the base currency adjustments created earlier in the period are deleted and then re-created if appropriate. If additional transactions have caused accounts to have a non-zero transaction currency balance, unrealized gain/loss is posted instead of a base currency adjustment.

**Key points for base currency adjustments:**

-   Base currency adjustments apply to non-equity balance sheet accounts subject to revaluation. Base currency adjustments aren't required for Accounts Receivable and Accounts Payable accounts.
    
-   Base currency adjustment is a separate currency revaluation transaction record called Currency Revaluation (Base Currency Adjustment). Values used to calculate the adjustment are shown on the Details subtab of the record.
    
-   The revaluation process checks account balances as of the end of an accounting period.
    
-   Base currency adjustments are created based on account balances. They aren't tied to individual transactions.
    
-   Base currency adjustments are created only if no unrealized gain or loss has been posted in the period for the account/currency pair. Additional unrealized gain or loss is posted if needed.
    
-   You can't change the posting period for a base currency adjustment.
    
-   If you rerun currency revaluation in the period, any base currency adjustments for the period are deleted. Depending on new account balances, base currency adjustments or unrealized gain/loss transactions are created.
    
-   Base currency adjustments are shown on the Unrealized Exchange Rate Gains and Losses report.
    

For information about running currency revaluation, see [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html).

### Related Topics

-   [Types of Accounts That Can Be Revalued](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428933.html)
-   [Base Currency Adjustment Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1429362.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
