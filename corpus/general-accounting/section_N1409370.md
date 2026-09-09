---
id: "section_N1409370"
type: "section"
title: "Foreign Currency Revaluation"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation"
parent: "chapter_N1395057"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409370.html"
anchors: []
sha256: "91fc96b809429d4f51907b4074fd94fed7e5c37499588e34f7d1632a52528623"
---

Changes in exchange rates between a company or subsidiary's base currency and the foreign currencies used in transactions can cause these transactions' base currency valuations to change over time. This impacts your general ledger accounts. As a foreign currency value changes relative to a company's base currency, so does the base currency value of transactions recorded in a company's general ledger accounts.

When you enable the Multiple Currencies feature, the following accounts are added to your chart of accounts after qualifying transactions:

| Account | Source |
| --- | --- |
| Realized Gain/Loss | Realized gains and losses resulting from payment application |
| Unrealized Gain/Loss | Unrealized gains and losses resulting from month-end open balance revaluation |
| Unrealized Matching Gain/Loss | 
-   Matching unrealized gains and losses from funds deposited This type of gain or loss is shown on the GL Impact subtab of certain foreign currency transactions, such as the bank deposit for a customer payment. NetSuite creates a gain or loss as part of the bank deposit, regardless of the dates of the customer payment and bank deposit.
-   Base currency adjustments For information about base currency adjustments, see [Residual Base Currency Balances and Base Currency Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1429248.html).

 |
| Rounding Gain/Loss | Gains and losses resulting from rounding differences This type of gain or loss is initiated when a payment transaction is applied to a source document transaction and a difference occurs due to the rounding of amounts. |

These accounts track the values for exchange rate fluctuations separately from the values of initial transactions. Use the account registers to see how fluctuations in exchange rates affect the financial position of your business. To view the account register for any of these accounts, click the account name link on the Chart of Accounts page at _Lists > Accounting > Accounts_. You also can obtain this data from the Realized Exchange Rate Gains and Losses and Unrealized Exchange Rate Gains and Loss reports.

Note:

After qualifying revaluation transactions, the system generates the Realized Gain/Loss, Unrealized Gain/Loss, Unrealized Matching Gain/Loss, Rounding Gain/Loss accounts. Depending on the year in which your NetSuite account was established, you may also have the Exchange Rate Variance account.

NetSuite automatically calculates and posts exchange rate gain or loss when users apply a payment or credit memo to an invoice. Gain or loss amounts are posted if the exchange rate has changed between the initial transaction (invoice) and the current transaction (payment or credit memo). The gain or loss resulting from changes to the exchange rate posts by default to the Realized Gain/Loss account. For more information about this type of revaluation, see [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html).

Revaluation for transactions that remain open and balances in foreign currency accounts is a separate process. The process is usually run at the end of the period as part of the period close checklist and requires the Currency Revaluation permission. For more information about this type of revaluation and instructions for running the process, see [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html).

You can define rules to specify which accounts the different types of foreign currency variances post to. If your NetSuite account has no variance posting rules, NetSuite posts the gains and losses from fluctuations in foreign exchange rates to the default system-generated accounts described earlier. For more information, see [Foreign Currency Variance Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4818126540.html).

If you use the Currency Exchange Rate Types feature, your currency revaluations use the default currency exchange rate type. For more information, see [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html).

### Related Topics

-   [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html)
-   [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html)
-   [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html)
-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
