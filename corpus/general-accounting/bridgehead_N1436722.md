---
id: "bridgehead_N1436722"
type: "bridgehead"
title: "Revaluation of Advanced Intercompany Journal Entry"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Revaluation Examples > Revaluation of Advanced Intercompany Journal Entry"
parent: "section_N1431203"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1436722.html"
anchors: []
sha256: "ef04ac3d251eb252bd5d6caab0764f5e6150ba113b4bc1c75e6a1067b53d7d32"
---

In this example, you revalue open balances for January to account for an expense report for a U.K. subsidiary employee with a line for a U.S. subsidiary expense.

**Advanced Intercompany Journal Entry**

In this example, the intercompany transaction has been recorded by the U.S. subsidiary using an advanced intercompany journal in January. The currency used for the journal is British pounds. The lines of the journal include the following additional information:

| Subsidiary | Account | Debit | Credit | Due To/From Subsidiary | Exchange Rate | Base Currency | Total Amount (Base Currency) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| U.S. | Expense | 100.00 |  |  | 2.0 | US dollar | 200.00 |
| U.S. | Intercompany Payables |  | 100.00 | U.K. | 2.0 | US dollar | 200.00 |
| U.K. | Intercompany Receivables | 100.00 |  | U.S. | 1.0 | British pound | 100.00 |
| U.K. | Expense |  | 100.00 |  | 1.0 | British pound | 100.00 |

The exchange rate of 2.0 to convert pounds to dollars is shown in the lines for the U.S. subsidiary with the base currency total.

For the U.K. subsidiary, the exchange rate is 1.0 because the transaction currency and base currency are the same.

**January Month End Revaluation**

At the end of January, the exchange rate to convert from the transaction currency to the base currency for the U.S. subsidiary has changed to 2.5. For the U.K. subsidiary, the transaction currency is the same as the base currency. A currency revaluation transaction is created for the U.S. subsidiary, but not the U.K. subsidiary.

The January currency revaluation details are in the Open Payables subtab and include the following information. The -50.00 is posted as a debit to Unrealized Gain/Loss for the U.S. subsidiary.

| Type | Currency | Transaction Exchange Rate | Ending Exchange Rate | Balance | Gain/Loss | Prior Gain/Loss | Net Gain/Loss |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Journal | British pound | 2.00 | 2.50 | £-100.00 | $-50.00 | 0.00 | $-50.00 |

### Related Topics

-   [Revaluation Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1431203.html)
-   [Revaluation of Invoice with No Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431303.html)
-   [Revaluation of Invoice with Partial Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431690.html)
-   [Revaluation in Reopened Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1432098.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
