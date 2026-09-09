---
id: "bridgehead_N1425933"
type: "bridgehead"
title: "Example with Same Period but Different Rates"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Accounting for Fluctuation in Exchange Rates for Closed Transactions > Examples for the Realized Exchange Rate Gains and Losses Report > Example with Same Period but Different Rates"
parent: "section_N1425819"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1425933.html"
anchors: []
sha256: "1124cad3edaa9c8bf34dfcc32c53a6c58abf191102c72002abd31f8af00f142a"
---

In this example of the Realized Exchange Rate Gains and Losses Report, a customer invoice and payment are recorded in a single accounting period. The exchange rates on the transaction dates are different.

**Scenario**

The U.K. subsidiary records a customer invoice dated February 15 for $300 U.S. dollars (USD). The U.S. dollar to pound sterling exchange rate on February 15 is 0.6379, and dollars are converted to pounds as follows: $300 × 0.6379 = £191.37.

On February 25, the invoice is paid. The dollar to pound exchange rate is 0.653733, and the conversion to pounds is $300 × 0.653733 = £196.12.

**General Ledger Impact on February 15**

| Rate = 0.6379 | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Accounts Receivable | $300 |  | £191.37 |  |
| Revenue |  | $300 |  | £191.37 |

**General Ledger Impact on February 25**

| Rate = 0.653733 | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Bank Account | $300 |  | £196.12 |  |
| Accounts Receivable |  | $300 |  | £196.12 |
| Accounts Receivable | $0 |  | £4.75 |  |
| Realized Gain/Loss |  | $0 |  | £4.75 |

**February Report**

A portion of the Realized Exchange Rate Gains and Losses report for February is shown in the following table. Transaction numbers and type, source account, transaction currency, and transaction dates are omitted here. The transactions and associated realized gain/loss are in the Accounts Receivable section of the report, and the source account is Accounts Receivable. Although the transaction currency is U.S. dollars, the currency symbol for the British pound (£), the base currency, appears in the report because the U.K. subsidiary has been selected in the Subsidiary Context footer.

| Name | Subsidiary | Source Accounting Period | Source Exchange Rate | Pmt Accounting Period | Pmt Exchange Rate | Applied Amount | Applied Amount (Base) | Realized Gain/Loss |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| UK Cust USD | U.K. | Feb | 0.64 | Feb | 0.65 | 300.00 | £196.12 | £4.75 |

Note:

The exchange rates shown in the Realized Exchange Rate Gains and Losses report are rounded to 2 decimal places. To view the complete exchange rate used to calculate the base currency amounts, you must drill down to the source transaction.

### Related Topics

-   [Examples for the Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425819.html)
-   [Example with Different Periods and Different Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1427520.html)
-   [Example of Credit Memo in a Different Period with a Different Rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1428017.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
