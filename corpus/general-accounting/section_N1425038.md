---
id: "section_N1425038"
type: "section"
title: "Accounting for Fluctuation in Exchange Rates for Closed Transactions"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Accounting for Fluctuation in Exchange Rates for Closed Transactions"
parent: "section_N1409370"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html"
anchors: []
sha256: "9fd01b4aea6ff09dba32f390ab01b103d963000b1cf3755f1271dc1018a93d37"
---

Changes in exchange rates between base currencies and foreign currencies used in transactions cause foreign currency transactions' base currency valuations to change over time. As exchange rates change, a variance occurs between the initial values of transactions and their values upon closure or payment. This variance is recorded in the general ledger as a gain or loss. For a definition of base currency, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).

The currency revaluations associated with transactions and accounts that are marked for elimination aren't eliminated. These gains and losses that are due to changes in exchanges rates need to be included in financial statements. For more information, see [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html) and its subtopics.

NetSuite automatically calculates and posts the exchange rate gain or loss when a payment is applied to a source transaction. The variance posts by default to the Realized Gain/Loss account. If your company uses the Foreign Currency Variance Mapping feature, your realized gains and losses may post to different accounts.

If you use the Currency Exchange Rate Types feature, the exchange rate gain or loss calculations use the default currency exchange rate type. For more information, see [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html).

Various transactions can be applied as payments including customer payments, credit memos, vendor bill payments, vendor credits, customer deposits, and journal entries. The source transaction may be a vendor bill, customer invoice, or a journal entry. A variance (gain or loss) is posted if the exchange rate has changed between the source transaction date and the date the payment is applied.

For details about how variances are calculated and posted, see [Applied Payments and Realized Gain/Loss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425327.html).

For sample variance calculations for different types of transactions, see [Examples for the Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425819.html).

Note:

The exchange rates shown in the Realized Exchange Rate Gains and Losses report are rounded to 2 decimal places. To view the complete exchange rate used to calculate the base currency amounts, drill down to the source transaction.

When foreign currency transactions remain open or unpaid at the end of an accounting period, you must generate revaluations for them before closing the period. You must also revalue balances in foreign currency denominated accounts. This revaluation process is separate from realized gains and losses that are automatically calculated for paid transactions. See [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html).

### Related Topics

-   [Foreign Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409370.html)
-   [Currency Revaluation Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550016096.html)
-   [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html)
-   [Foreign Currency Variance Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4818126540.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
