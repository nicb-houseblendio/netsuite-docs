---
id: "bridgehead_N1427520"
type: "bridgehead"
title: "Example with Different Periods and Different Rates"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Accounting for Fluctuation in Exchange Rates for Closed Transactions > Examples for the Realized Exchange Rate Gains and Losses Report > Example with Different Periods and Different Rates"
parent: "section_N1425819"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1427520.html"
anchors: []
sha256: "45a20027ffaef41819f0732661d891bbace64380242a04ae8c18d06a1f3b88c6"
---

In this example of the Realized Exchange Rate Gains and Losses Report, a customer invoice is recorded in one accounting period and paid in a subsequent accounting period when the exchange rates are different.

The U.K. subsidiary records a customer invoice dated February 15 for $400 U.S. dollars (USD). The U.S. dollar to pound sterling exchange rate on February 15 is 0.6379, and dollars are converted to pounds as follows: $400 × 0.6379 = £255.16.

When the month end currency revaluation is run for February, the exchange rate is 0.61. The unrealized gain/loss for the open receivable is recorded using that exchange rate and reversed in the subsequent period.

On March 26, when the invoice is paid, the dollar to pound exchange rate is 0.67305. The conversion to pounds is $400 × 0.67305 = £269.22.

**General Ledger Impact on February 15**

| Rate = 0.6379 | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Accounts Receivable | $400 |  | £255.16 |  |
| Revenue |  | $400 |  | £255.16 |

**General Ledger Impact on March 26**

The payment has the following general ledger impact:

| Rate = 0.67305 | Transaction Currency | Base Currency |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Bank Account | $400 |  | £269.22 |  |
| Accounts Receivable |  | $400 |  | £269.22 |
| Accounts Receivable | $0 |  | £14.06 |  |
| Realized Gain/Loss |  | $0 |  | £14.06 |

**March Report**

A portion of the Realized Exchange Rate Gains and Losses report for March is shown in the following table. Transaction numbers and type, source account, transaction currency, and transaction dates are omitted here. The transactions and associated realized gain/loss are in the Accounts Receivable section of the report, and the source account is Accounts Receivable. Although the transaction currency is U.S. dollars, the currency symbol for the British pound (£), the base currency, appears in the report because the U.K. subsidiary has been selected in the Subsidiary Context footer.

| Name | Subsidiary | Source Accounting Period | Source Exchange Rate | Pmt Accounting Period | Pmt Exchange Rate | Applied Amount | Applied Amount (Base) | Realized Gain/Loss |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| UK Cust USD | U.K. | Feb | 0.64 | Mar | 0.67 | 400.00 | £269.22 | £14.06 |

Note:

The exchange rates shown in the Realized Exchange Rate Gains and Losses report are rounded to 2 decimal places. To view the complete exchange rate used to calculate the base currency amounts, you must drill down to the source transaction.

### Related Topics

-   [Examples for the Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425819.html)
-   [Example with Same Period but Different Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1425933.html)
-   [Example of Credit Memo in a Different Period with a Different Rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1428017.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
