---
id: "section_N1407165"
type: "section"
title: "Consolidated Exchange Rate Automatic Calculation Example"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Consolidated Exchange Rates > Calculating Consolidated Exchange Rates Automatically > Consolidated Exchange Rate Automatic Calculation Example"
parent: "section_N1406908"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407165.html"
anchors: []
sha256: "d9832395f0ebd69d96929801995ecb4409a7e3dae6d0ce2ed5f68d837017b98c"
---

The following is an example of the calculation that NetSuite uses to determine the consolidated exchange rates for subsidiaries with the following hierarchy:

-   U.S. Subsidiary is parent subsidiary, base currency is USD
    
-   U.K. Subsidiary is child subsidiary, base currency is GBP
    

The transactions during the period of January for the U.K. Subsidiary are listed in the following table:

| Transaction Date | Currency Exchange Rate | Amount | Posting Account General Rate Type |
| --- | --- | --- | --- |
| January 1 | 2 | 100 GBP | Average |
| January 1 | 2 | 300 GBP | Historical |
| January 15 | 2.5 | 200 GBP | Average |
| January 15 | 2.5 | 200 GBP | Historical |
| January 31 | 3 | 300 GBP | Average |
| January 31 | 3 | 100 GBP | Historical |

When you click Calculate at the top of the Consolidated Exchange Rates page, the consolidated exchange rates from the U.K. Subsidiary to the U.S. Subsidiary are derived as follows:

-   Current rate uses the GBP to USD rate from the Currency Exchange Rates list as of the end of the period (January 31).
    
    Current rate = 3
    
-   Average rate is a weighted average based on transaction amounts posted to all accounts with a general rate type of Average. The currency exchange rate for each transaction is the GBP to USD rate in effect on the transaction date.
    
    Average rate = (2 × 100 + 2.5 × 200 + 3 × 300) ÷ 600 = 2.6666667
    
-   Historical rate is a weighted average based on transaction amounts posted to all accounts with a general rate type of Historical. As for the average rate, the currency exchange rate for each transaction is the GBP to USD rate in effect on the transaction date.
    
    Historical rate = (2 × 300 + 2.5 × 200 + 3 × 100) ÷ 600 = 2.3333333
    

The results are the same if you click the calculate icon ![Calculator icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/calculator.png) for each subsidiary pair.

Note:

In a transaction saved search that includes consolidated exchange rates values, the values may not match the general ledger impact of these same transactions. The difference is because currency exchange rates are used to determine the general ledger impact of transactions, not consolidated exchange rates. For more information, see [Consolidated Exchange Rate Types for Transaction Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html).

### Related Topics

-   [Calculating Consolidated Exchange Rates Automatically](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406908.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
