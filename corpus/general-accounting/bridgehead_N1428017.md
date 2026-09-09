---
id: "bridgehead_N1428017"
type: "bridgehead"
title: "Example of Credit Memo in a Different Period with a Different Rate"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Accounting for Fluctuation in Exchange Rates for Closed Transactions > Examples for the Realized Exchange Rate Gains and Losses Report > Example of Credit Memo in a Different Period with a Different Rate"
parent: "section_N1425819"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1428017.html"
anchors: []
sha256: "a14a649721fbb1f57e6c5f19b2975b0aa40a3fbeb33f5214397e05ceda2fa212"
---

In this example of the Realized Exchange Rate Gains and Losses Report, a credit memo is issued to a customer and applied to an open invoice. The transactions are in different periods with different exchange rates.

Note:

When you create a credit memo from an invoice, the credit memo inherits the exchange rate from the invoice. No gain or loss is generated. If you create a standalone credit memo and apply it to an invoice with a different exchange rate, realized gain or loss is generated as described in the example below.

The U.K. subsidiary records a customer invoice dated January 15 for $800 U.S. dollars (USD). The U.S. dollar to pound sterling exchange rate on January 15 is 0.6140, and dollars are converted to pounds as follows: $800 × 0.6140 = £491.20.

The invoice remains open until March 16, when a standalone credit memo is issued for $800 U.S. dollars, and the credit memo is applied to the invoice. The exchange rate on March 16 is 0.6617375.

**General Ledger Impact for Invoice on January 15**

| Rate = 0.6140 | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Accounts Receivable | $800 |  | £491.20 |  |
| Revenue |  | $800 |  | £491.20 |

**General Ledger Impact for Credit Memo on March 16**

| Rate = 0.6617375 | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Revenue | $800 |  | £529.39 |  |
| Accounts Receivable |  | $800 |  | £529.39 |

**General Ledger Impact for Applying the Credit Memo on March 16**

|  | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Accounts Receivable | $0 |  | £38.19 |  |
| Realized Gain/Loss |  | $0 |  | £38.19 |

**March Report**

A portion of the Realized Exchange Rate Gains and Losses report for March is shown in the following table. Transaction numbers and type, source account, transaction currency, and transaction dates are omitted here. The transactions and associated realized gain/loss are in the Accounts Receivable section of the report, and the source account is Accounts Receivable. Although the transaction currency is U.S. dollars, the currency symbol for the British pound (£), the base currency, appears in the report because the U.K. subsidiary has been selected in the Subsidiary Context footer.

| Name | Subsidiary | Source Accounting Period | Source Exchange Rate | Pmt Accounting Period | Pmt Exchange Rate | Applied Amount | Applied Amount (Base) | Realized Gain/Loss |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| UK Cust USD | U.K. | Jan | 0.61 | Mar | 0.66 | 800.00 | £529.39 | £38.19 |

Note:

The exchange rates shown in the Realized Exchange Rate Gains and Losses report are rounded to 2 decimal places. To view the complete exchange rate used to calculate the base currency amounts, you must drill down to the source transaction.

### Related Topics

-   [Examples for the Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425819.html)
-   [Example with Same Period but Different Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1425933.html)
-   [Example with Different Periods and Different Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1427520.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
