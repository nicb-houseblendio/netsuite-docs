---
id: "section_N1425327"
type: "section"
title: "Applied Payments and Realized Gain/Loss"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Accounting for Fluctuation in Exchange Rates for Closed Transactions > Applied Payments and Realized Gain/Loss"
parent: "section_N1425038"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425327.html"
anchors: []
sha256: "60997759aa68af04550f975247cf5ef77cf2024a381e42af0dcae1d33e27fa64"
---

NetSuite calculates and posts exchange rate gain or loss (variance) when you apply a payment or credit to an invoice, vendor bill, or journal entry that functions as a bill or invoice. The invoice, vendor bill, or journal entry is the source transaction. The variance occurs when the exchange rate on the source transaction differs from the exchange rate on the payment. The payment can be a payment transaction, credit memo, customer deposit, or journal entry.

The variance resulting from changes to the exchange rate for payments applied to source transactions is posted using a currency revaluation transaction. The currency revaluation transaction and payment are linked as related records to the source transaction. For more information about this transaction type, see [Currency Revaluation Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550016096.html).

By default, the variance for closed transactions posts to the Realized Gain/Loss account. However, you can create rules to post these variances to different accounts. For information, see [Foreign Currency Variance Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4818126540.html).

When foreign currency transactions remain open or unpaid at the end of an accounting period, you need to generate revaluations for them before closing the period. You also need to revalue balances in foreign currency denominated accounts. This revaluation process is separate from realized gains and losses that are automatically calculated for paid transactions. For information, see [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html).

Foreign-currency-denominated source transactions remain open until the invoice balance equals zero in both the foreign currency and the base currency.

For details about variance calculations, posting periods for realized gain and loss, and the effecting of voiding payments, see the following subsections:

-   [Variance Calculations for Realized Gain and Loss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4279828767.html)
    
-   [Posting Periods and Transaction Dates for Realized Gain and Loss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1550020494.html)
    
-   [Effect of Voiding Applied Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556144790.html)
    

### Related Topics

-   [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html)
-   [Rounding Gain/Loss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4030214366.html)
-   [Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425486.html)
-   [Examples for the Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425819.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
