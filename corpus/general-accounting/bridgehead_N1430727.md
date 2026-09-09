---
id: "bridgehead_N1430727"
type: "bridgehead"
title: "Viewing Revaluation Results"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Generating Revaluations > Viewing Revaluation Results"
parent: "section_N1430227"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430727.html"
anchors: []
sha256: "1cf12ed4094fe52b2ab8547c98abb48e5c2fc5920595abe3bab577a5db0a3c6b"
---

Use the Task: Revalue Open Currency Balances page on the Period Close Checklist to view information about the status and results of each currency revaluation run.

The **Results** subtab displays the currency revaluations created for each run in addition to the currency and the total variance amount for the transaction. If a revaluation run produces four currency revaluation transactions, you see four lines for that run number, each with a link to the revaluation results details.

Click the **Transaction** number to open the Currency Revaluation (Unrealized Gain/Loss) page.

![Screenshot of period close task: Revalue Open Foreign Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/revalresults.png)

You can also go to _Transactions > Financial > Revalue Open Currency Balances > List_ to view currency revaluation results.

The **Status** subtab displays the status of the currency revaluation. The Percent Complete column provides how much of the process has run.

![Screenshot showing Status subtab of Task: Revalue Open Foreign Currency Balances page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/revalstatus.png)

You can also view the Foreign Currency Revaluation: Status page at _Transactions > Financial > Revalue Open Currency Balances > Status_.

The Currency Revaluation (Unrealized Gain/Loss) page displays the detailed results for each currency revaluation. You can open this page from the link in the Results subtab or from the Currency Revaluations list at _Transactions > Financial > Revalue Open Currency Balances > List_.

![Screenshot of Currency Revaluation (Unrealized Gain/Loss) page showing Open Receivables subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/currencyrevalresults.png)

-   Review the amount in the **Total Variance** field.
    
    NetSuite calculates the total impact of exchange rate fluctuations for the selected accounts and displays the amount in the **Total Variance** field.
    
    A negative number indicates that overall, open foreign currency transactions and account balances have decreased in base currency value, resulting in a debit for the posting period. A positive number indicates an overall increase in base-currency value, resulting in a credit for the posting period.
    
-   Click the available **Details** subtabs to view the details of the revaluation calculation. For unrealized gain/loss, these subtabs include **Open Receivables**, **Open Payables**, and **Other Accounts**. Drill down to view the source transactions for each revaluation amount. For more information, see [Revaluation Record Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430933.html).
    
-   The **GL Impact** subtab shows the accounts affected by the revaluation with debit and credit amounts.
    

In some cases, NetSuite creates a Currency Revaluation (Base Currency Adjustment) transaction instead of an Unrealized Gain/Loss transaction. For details, see [Residual Base Currency Balances and Base Currency Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1429248.html).

### Related Topics

-   [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html)
-   [Foreign Currency Revaluation for Multiple Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4169300609.html)
-   [Classifications and Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430408.html)
-   [Revaluation Record Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430933.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
