---
id: "section_N1428662"
type: "section"
title: "Revaluation of Open Currency Balances"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances"
parent: "section_N1409370"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html"
anchors: []
sha256: "30b319bcc3a9a26e9731a9f4bf692c6478b79f0903525e3e2d66f967cbd9caa3"
---

As exchange rates between a base currency and foreign currencies change over time, the base currency value of foreign currency denominated transactions and accounts also changes.

When a payment is applied to close a transaction, NetSuite automatically calculates and posts the realized gain or loss due to exchange rate fluctuation. See [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html).

You must run a revaluation process to calculate the unrealized gain or loss due to exchange rate fluctuation. To run this process, you must have a role with the Currency Revaluation permission at Create level or higher. Unrealized gain or loss applies to open customer and vendor transactions, foreign-currency-denominated accounts, and other non-equity balance sheet accounts. Currency revaluation should be part of your month-end close process. If you don't run revaluation at the end of the period, your monthly financial statements may be inaccurate due to missing currency revaluation transactions.

Note:

You must enable the Accounting Periods feature in your account before you attempt to generate revaluations. Accounting periods are required to properly post open balance revaluations at the end of each accounting period. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).

You can generate revaluations as part of the Period Close Checklist or at any time, and for any reason, from _Transactions > Financial > Revalue Open Currency Balances_. You should lock the period before you generate revaluations. Revaluations apply exchange rates as of the last day of the accounting period to calculate gain or loss. If you generate revaluations from the menu prior to the end of the period, the exchange rate for the current date is used.

If you use Multi-Book Accounting, you can run month-end currency revaluation in both pending and active secondary accounting books.

If you use the Currency Exchange Rate Types feature, your currency revaluations use the default currency exchange rate type. For more information, see [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html).

A revaluation calculates the effects of exchange rate fluctuations on open balances for a selected period. Only transactions whose transaction period matches the selected period are evaluated. Related transactions that occur in a period later than the selected period are ignored. An exception to this rule may occur when you void an applied payment. For more about voided payments, see [Effect of Voiding Applied Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556144790.html).

For example, an invoice recorded in January is paid in July. The variance due to exchange rate fluctuation is calculated on the open balance each period from January through June and posted as unrealized gain or loss. When the payment is made in July, the realized gain or loss is posted in that period.

The currency revaluations associated with transactions and accounts that are marked for elimination aren't eliminated. These gains and losses that are due to changes in exchanges rates need to be included in financial statements. For more information, see [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html) and its subtopics.

Important:

If you intend to match the source classification when you revalue open receivables and open payables, all source transactions must include values for all required classification. Classification includes department, class, location, and custom segment with GL impact. See [Classifications and Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430408.html).

For instructions and additional information about the revaluation of open currency balances, see the following topics:

-   [Types of Accounts That Can Be Revalued](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428933.html) - for more information about accounts that can be revalued
    
-   [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html) - for instructions for revaluing open currency balances before closing a period
    
-   [Revaluation Record Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430933.html) - for information about the Details subtab of the currency revaluation transaction
    
-   [Unrealized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1437432.html) - for information about reporting for unrealized exchange rate gains and losses
    

### Related Topics

-   [Foreign Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409370.html)
-   [Currency Revaluation Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550016096.html)
-   [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html)
-   [Foreign Currency Variance Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4818126540.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
