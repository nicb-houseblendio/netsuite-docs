---
id: "bridgehead_N1431690"
type: "bridgehead"
title: "Revaluation of Invoice with Partial Payment"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Revaluation Examples > Revaluation of Invoice with Partial Payment"
parent: "section_N1431203"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431690.html"
anchors: []
sha256: "79489a32d804e5ddb041a48557884c2f04e3469ea85116005b8b422b3c161c04"
---

In this example, you're revaluing open balances for January between your U.S. based subsidiary and a British customer. Transactions include the following:

-   January 7 Invoice for 100 GBP
    
    -   Rate is 2 USD to 1 GBP
        
    -   Base currency value = 200 USD
        
-   January 9 Payment for 40 GBP
    
    -   Rate is 2.5 USD to 1 GBP
        
    -   Base currency value = 100 USD
        
        -   100 USD credited to Accounts Receivable account
            
        -   20 USD credited to Realized Gain/Loss account
            
-   February 15 Payment for 60 GBP
    
    -   Rate is 3 USD to 1 GBP
        
    -   Base currency value = 180 USD
        
        -   180 USD credited to Accounts Receivable account
            
        -   60 USD credited to Realized Gain/Loss account
            
-   January Period Close Revaluation
    
    -   Revalues the open balance amount of the invoice (60 GBP) at the end of the month
        
    -   Rate on January 31 is 2.5 USD to 1 GBP
        
    -   Variance = (Ending Rate - Transaction Rate) × Balance
        
    -   30 USD posts to Unrealized Gain/Loss account
        

The currency revaluation transaction includes the following columns in the Details subtab under Open Receivables. These columns follow Type, Date, Payee, and Currency. Currency symbols don't appear in the transaction record but are included here to distinguish the transaction currency from the base currency.

| Transaction Exchange Rate | Ending Exchange Rate | Balance | Gain/Loss | Prior Gain/Loss | Net Gain/Loss |
| --- | --- | --- | --- | --- | --- |
| 2.00 | 2.50 | £60.00 | $30.00 | 0.00 | $30.00 |

When you run revaluation in February, this transaction is closed by the payment of the balance on February 15 and not subject to revaluation.

### Related Topics

-   [Revaluation Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1431203.html)
-   [Revaluation of Invoice with No Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431303.html)
-   [Revaluation in Reopened Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1432098.html)
-   [Revaluation of Advanced Intercompany Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1436722.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
