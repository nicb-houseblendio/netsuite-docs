---
id: "section_N1785562"
type: "section"
title: "Foreign Currency Amortization Examples"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Foreign Currency Amortization > Foreign Currency Amortization Examples"
parent: "section_N1784814"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1785562.html"
anchors: ["bridgehead_N1785626", "bridgehead_N1786909"]
sha256: "fb79205c1ec8c5fa8cc9b61ef0312a8d43a547bc3b94cd8dedbb9ccf62421820"
---

-   [Foreign Currency Amortization Schedule (Standard) Example](#bridgehead_N1785626) [Foreign Currency Amortization Schedule (Standard) Example](#bridgehead_N1785626)
    
-   [Foreign Currency Amortization Schedule (Variable) Example](#bridgehead_N1786909) [Foreign Currency Amortization Schedule (Variable) Example](#bridgehead_N1786909)
    

## Foreign Currency Amortization Schedule (Standard) Example {#bridgehead_N1785626}

Note:

Foreign currency amortization is available only in NetSuite U.K. editions.

The following is an example of amortizing prepaid assets denominated in a foreign currency using a foreign currency amortization schedule. This example assumes:

-   Foreign currency transactions are recorded in local currency using the exchange rate in effect on the date the transaction occurred.
    
-   The company's base currency is GBP.
    
-   The effect of hedging transactions isn't considered in the analysis.
    

**Recording the Bill and Payment**

Vendor bill (invoice) is recorded and paid at the same exchange rate in a single accounting period.

On February 1, a bill is received from a USD vendor for services to be rendered from 2/1/2010 to 4/30/2010. The bill is fully paid when it's received at the same exchange rate. The exchange rate on February 1 is 1.50 USD to 1.00 GBP (600 / 1.50 = 400).

Accounting for bill:

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Prepaid Services | USD | 600 | 400 |
| Accounts Payable | USD | (600) | (400) |

Accounting for bill payment:

| Description/Account | Transaction Currency | Amount DrR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Accounts Payable | USD | 600 | 400 |
| Cash | USD | (600) | (400) |

Since the bill is settled, there will be no revaluation of the transaction for A/P purposes at month-end.

**Amortization Schedule**

Because this prepayment represents services to be rendered evenly over three months, the straight-line amortization method is used. The prepaid asset will be amortized to the Service Expense account. (Prepaid Services is the deferral/capitalization account).

The following amortization schedule is created:

| Period | Deferral Account | Destination Account | Transaction Currency | Foreign Amount\* | Base Amount\*\* |
| --- | --- | --- | --- | --- | --- |
| Feb 2010 | Prepaid Services | Service Expense | USD | 200 | 133.33 |
| Mar 2010 | Prepaid Services | Service Expense | USD | 200 | 133.33 |
| Apr 2010 | Prepaid Services | Service Expense | USD | 200 | 133.33 |

\*The foreign amount is based on the foreign amount of the transaction.

\*\*The base amount is the foreign amount divided by the rate on the transaction (200/1.5 = 133.33)

Note:

The total amortization amount in the **Base Amount** column may be slightly different from the total base currency amount on the related transaction line due to rounding. In this example, the total transaction base currency amount is $400, but the base currency amount amortized is $399.99. You may want to journal out these rounding differences periodically

**Creation of Amortization Journal Entries**

At the end of each period, amortization journal entries are created for the period using historical rates.

Journal posted on February 28, currency rate 1.50 USD to 1.00 GBP (200/1.50 = 133.33):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Services Expense | USD | 200 | 133.33 |
| Prepaid Services | USD | (200) | (133.33) |

Journal posted on March 31, currency rate 1.50 USD to 1.00 GBP (200/1.50 = 133.33):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Service Expense | USD | 200 | 133.33 |
| Prepaid Services | USD | (200) | (133.33) |

Journal posted on April 30, currency rate 1.50 USD to 1.00 GBP (200/1.50 = 133.33):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Prepaid Services | USD | 600 | 400 |
| Accounts Payable | USD | (600) | (400) |

## Foreign Currency Amortization Schedule (Variable) Example {#bridgehead_N1786909}

In this example, the vendor bill (invoice) is recorded and paid at the same exchange rate in a single accounting period. The bill represents services that will be completed over several months and tracked as a project. Expenses are amortized based on the percentage of project completion. This example assumes:

-   Foreign currency transactions are recorded in local currency using the exchange rate in effect on the date the transaction occurred.
    
-   The company's base currency is GBP.
    
-   The effect of hedging transactions isn't considered in the analysis.
    

**Recording the Bill and Payment**

On February 1, a bill is received from a USD vendor for services to be rendered. The bill is fully paid when received at the same exchange rate. The exchange rate on February 1 is 1.50 USD to 1.00 GBP (600 / 1.50 = 400). The project associated with this bill for computer maintenance is created and associated with this line on the bill.

Accounting for bill, currency rate, 1.50 USD to 1.00 GBP (600/1.50 = 400):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Prepaid Services | USD | 600 | 400 |
| Accounts Payable | USD | (600) | (400) |

Accounting for bill payment, currency rate 1.50 USD to 1.00 GBP (600/1.50 = 400):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Accounts Payable | USD | 600 | 400 |
| Cash | USD | (600) | (400) |

Because the bill is settled, there is no revaluation of the transaction for A/P purposes at month-end.

**Amortization Schedule**

The amortization schedule is created without lines because the amount to amortize is based on the percentage of project completion and not known at this point.

The project work is completed as follows:

-   February - 25% complete (25% total)
    
-   March - 50% complete (75% total)
    
-   April - 25% complete (100% total)
    

The amortization schedule calculated the following amounts:

| Period | Deferral Account | Destination Account | Transaction Currency | % Amortized | Total Amortized | Foreign Amount\* | Base Amount\*\* |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Feb 2010 | Prepaid Services | Service Expense | USD | 25% | 25% | 150 (25% of 600) | 100 (25% of 400) |
| Mar 2010 | Prepaid Services | Service Expense | USD | 50% | 75% | 300 | 200 |
| Apr 2010 | Prepaid Services | Service Expense | USD | 25% | 100% | 150 | 100 |

\*The foreign amount is based on the foreign amount of the transaction.

\*\*The base amount is foreign amount divided by the rate on the transaction (300/1.5 = 200)

**Creation of Amortization Journal Entries**

At the end of each period, amortization journal entries are created for the period using historical rates.

Journal posted on February 28, currency rate 1.50 USD to 1.00 GBP (200/1.50 = 133.33):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Services Expense | USD | 150 | 100 |
| Prepaid Services | USD | (1500) | (100) |

Journal posted on March 31, currency rate 1.50 USD to 1.00 GBP (300/1.50 = 200.00):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Service Expense | USD | 300 | 200 |
| Prepaid Services | USD | (300) | (200) |

Journal posted on April 30, currency rate 1.50 USD to 1.00 GBP (200/1.50 = 133.33):

| Description/Account | Transaction Currency | Amount DR (CR) | GPB Home Value |
| --- | --- | --- | --- |
| Prepaid Services | USD | 150 | 100 |
| Accounts Payable | USD | (150 | (100) |

### Related Topics

-   [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html)
-   [Setting Up Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784923.html)
-   [Using Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784998.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
