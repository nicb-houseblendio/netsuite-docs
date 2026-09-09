---
id: "bridgehead_N1431303"
type: "bridgehead"
title: "Revaluation of Invoice with No Payments"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Revaluation Examples > Revaluation of Invoice with No Payments"
parent: "section_N1431203"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431303.html"
anchors: []
sha256: "5f0f85666a5f2a2fa37b1facc2590be4d0298677b7a39ff8c609b73af39e51ba"
---

In this example, you're revaluing open balances for January. The Open Receivables list includes the following transactions between your U.S. based subsidiary and a British customer:

-   Invoice 1 = 100 British Pounds (GBP)
    
-   Invoice 2 = 50 British Pounds (GBP)
    

The currency revaluation transaction includes the following columns in the Details subtab under Open Receivables. These columns follow Type, Date, Payee, and Currency. Currency symbols don't appear in the transaction record but are included here to distinguish the transaction currency from the base currency.

| Transaction Exchange Rate | Ending Exchange Rate | Balance | Gain/Loss | Prior Gain/Loss | Net Gain/Loss |
| --- | --- | --- | --- | --- | --- |
| 2.00 | 2.50 | £100.00 | $50.00 | 0.00 | $50.00 |
| 2.00 | 2.50 | £50.00 | $25.00 | 0.00 | $25.00 |

On the GL Impact subtab, you see a credit of $75 is posted to the Unrealized Gain/Loss account. This amount is the total of the Net Gain/Loss variance for the two invoices.

The Balance column lists the transaction currency balances as of the last day of the period, January 31. These amounts remain the same even if payments are applied to invoices in a later period, regardless of the date of the payment. Any amounts related to future payments are posted in the period when the payments are made.

### Related Topics

-   [Revaluation Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1431203.html)
-   [Revaluation of Invoice with Partial Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431690.html)
-   [Revaluation in Reopened Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1432098.html)
-   [Revaluation of Advanced Intercompany Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1436722.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
