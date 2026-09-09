---
id: "section_N1704597"
type: "section"
title: "Calculating Foreign Currency Adjustment for Revenue Commitments"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Advanced Revenue Commitments Overview > Calculating Foreign Currency Adjustment for Revenue Commitments"
parent: "section_N1703735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1704597.html"
anchors: ["bridgehead_N1704663", "bridgehead_N1705077"]
sha256: "7252d934dcc87489a55de426162f275296d6b4dc9090cd17864ffaa67dc0df2b"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

The revenue reclassification for the foreign currency variance related to a sales order with a revenue commitment is automatically generated when you create revenue reclassification journal entries. The amount is calculated by determining the overlapping foreign currency amounts for billing and revenue recognition and the effective billing foreign currency rate.

-   **Effective Billing FX Rate** - The effective billing exchange rate is the total base currency amount billed divided by the total foreign currency amount billed.
    
-   **Overlap** - The overlap is the overlapping amount between the amount of income recognized and the amount billed for an order. Overlap amounts are always in transaction (foreign) currency and based on cumulative order amounts. For example, if the total foreign currency recognized revenue amount at the end of a month for an order is 200 and the total foreign currency billed amount is 300, the overlap amount is 200. If the total foreign currency recognized revenue is 200 and the total foreign currency billed amount is 150, the overlap amount is 150.
    
    When accumulated billing is greater than accumulated revenue for an order, the revenue adjustment is calculated as follows:
    
    **(Overlap x Effective Billing FX Rate) - Recognized Revenue in Base Currency**
    
    When accumulated billing is less than accumulated revenue for an order, the revenue adjustment is calculated as follows:
    
    **Billed Amount in Base Currency - (Overlap x Revenue Commitment FX Rate)**
    

The foreign currency gain/loss adjustment posts to the revenue account for the sales order when you reclassify revenue.

## Billing Greater Than Revenue Recognition Example {#bridgehead_N1704663}

A sales order with revenue commitment has 2 items. The first item is recognized and billed in full. The second item has a 12 month revenue recognition schedule and 12 month billing schedule. The transaction currency is GBP and base currency is USD. The currency exchange rate when the revenue commitment is generated is 1.5 USD/GBP. The exchange rate when the first item is billed is 2.0 USD/GBP. The second item is billed when the rate is 1.25 USD/GBP.

The order has the following details at the end of the first month:

| Sales Order | Total Amount | Revenue Recognition | Billing |
| --- | --- | --- | --- |
| Line 1 | GBP 100 | GBP 100 | USD 150 | GBP 200 | USD 400 |
| Line 2 | GBP 1200 | GBP 100 | USD 150 | GBP 100 | USD 125 |

The revenue reclassification is calculated as follows:

-   Effective billing FX rate = (400 +125) / (200 +100) = 1.75 USD/GBP
    
-   Overlap = GBP 200
    
-   FX adjustment = (200/300 x (125+ 400) - (150 + 150) or
    
    (200 x 1.75) -300 = USD 50
    

The G/L impact for the revenue reclassification for the foreign currency adjustment is:

| Account | Debit | Credit |
| --- | --- | --- |
| Deferred Revenue | USD 50 |  |
| Revenue |  | USD 50 |

## Billing Less Than Revenue Recognition Example {#bridgehead_N1705077}

A sales order with revenue commitment has 2 items. The first item is recognized in full in the first month. It has a 2 month billing schedule. The second item has a 12 month revenue recognition schedule and 12 month billing schedule. The transaction currency is GBP and base currency is USD. The currency exchange rate when the revenue commitment is generated is 1.5 USD/GBP. The exchange rate when the first item is billed is 2.0 USD/GBP. The second item is billed when the rate 2.5 USD/GBP.

The order has the following details at the end of the first month:

| Sales Order | Total Amount | Revenue Recognition | Billing |
| --- | --- | --- | --- |
| Line 1 | GBP 100 | GBP 100 | USD 150 | GBP 50 | USD 100 |
| Line 2 | GBP 1200 | GBP 100 | USD 150 | GBP 100 | USD 250 |

The revenue reclassification is calculated as follows:

-   Effective billing FX rate = (100 + 250) / (50 +100) = 2.33333 USD/GBP
    
-   Overlap = GBP 150
    
-   FX adjustment = (100 + 250) - (150 x 1.5) - or
    
    350 - (350/2.3333) x 1.5 = USD 125
    

The G/L impact for the revenue reclassification for the foreign currency adjustment is:

| Account | Debit | Credit |
| --- | --- | --- |
| Deferred Revenue | USD 125 |  |
| Revenue |  | USD 125 |

For information about creating reclassification journal entries, see [Reclassifying Deferred Revenue for Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707946.html).

### Related Topics

-   [Advanced Revenue Commitments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703735.html)
-   [Life Cycle for Sales Order with Revenue Commitment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703982.html)
-   [Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3752066884.html)
-   [Adopting Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3758129615.html)
-   [Billing Additional Items on Orders with Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1706812.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
