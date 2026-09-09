---
id: "section_N269257"
type: "section"
title: "Multiple Currencies in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Subsidiaries in OneWorld > Multiple Currencies in OneWorld"
parent: "section_N268563"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269257.html"
anchors: ["bridgehead_156777556141", "bridgehead_156777561145", "bridgehead_156777565443", "bridgehead_156777576589", "bridgehead_156777583192"]
sha256: "ac3cec16a9d679a547169fa03406660e5db178b03a44a0080698304007832f90"
---

The Multiple Currencies feature provides support for transactions with entities that use currencies other than the currency in which your company manages its financials. The currency used to manage your company's financials is called the base currency. Other currencies used by customers and vendors are referred to as foreign currencies.

The Multiple Currencies feature is required for NetSuite OneWorld. With OneWorld, each subsidiary can have a separate base currency, which is used to manage the subsidiary's financials. You can't change a subsidiary's base currency after the subsidiary record has been saved for the first time.

## Currency Records {#bridgehead_156777556141}

As you plan your subsidiary hierarchy, you must determine the base currency of your root subsidiary. Then, the base currencies of all of your other subsidiaries. All subsidiary base currencies as well as any other currencies used in transactions should be set up in NetSuite. See [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html).

When you enter a transaction for a subsidiary, the currency defined on the customer's or vendor's record determines the currency used in the transaction amounts. If a customer or vendor has a currency different from the subsidiary, the transaction must use two currencies. The foreign currency used by the customer or vendor, and the base currency used by the subsidiary.

## Currency Exchange Rates {#bridgehead_156777561145}

NetSuite uses currency exchange rates to convert foreign currencies to base currencies. Exchange rates provide default rates for transactions in currencies other than the base currency. Exchange rates are expressed in terms of base currency units per foreign currency units. You must set up a currency exchange rates list in NetSuite. See [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html). You can enable the Currency Exchange Rate Integration feature to automatically update currency exchange rates on a nightly basis. See [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html).

## Consolidated Exchange Rates {#bridgehead_156777565443}

Consolidated reports use a separate consolidated exchange rates table to translate child subsidiaries' amounts to roll up into consolidated parent subsidiary amounts. See [Consolidated Reporting in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278654.html) and [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html).

## Budget Exchange Rates {#bridgehead_156777576589}

Reports that include budget and actual amounts, such as some financial statements, use a separate budget exchange rates table for translation of budget amounts. See [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html) and [Subsidiary-Specific Budget Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2125541.html).

## Exchange Rate Variance Amounts {#bridgehead_156777583192}

Over time, variances in exchange rates can affect the value of foreign currency transactions. NetSuite automatically calculates and posts exchange rate variance amounts for transactions that close during each accounting period. See [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html). In addition, before you close each period, you are required to revalue open balances to account for variances. See [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html).

### Related Topics

-   [Elimination Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268759.html)
-   [Subsidiary Hierarchy Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269084.html)
-   [Nexuses and Taxes in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269581.html)
-   [NetSuite Editions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N270055.html)
-   [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
