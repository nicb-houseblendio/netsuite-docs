---
id: "section_N1684020"
type: "section"
title: "Straight-Line Revenue Recognition Method Examples"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Creating Revenue Recognition Templates > Understanding Revenue Recognition Template Terms > Straight-Line Revenue Recognition Method Examples"
parent: "section_N1679634"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1684020.html"
anchors: ["bridgehead_N1684177", "bridgehead_N1684400", "bridgehead_N1685744", "bridgehead_1487719286", "bridgehead_N1686006", "bridgehead_N1686358"]
sha256: "8f101bc3dd021fcea1c273f14e7e117c912d44340c0cf3c1c6cebf98d8783f8c"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For the equivalent information for Advanced Revenue Management (Essentials), see [Straight-Line Revenue Recognition Examples in Advanced Revenue Management (Essentials)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4362249596.html).

When a straight-line method is used, revenue from a sale is recognized over the revenue recognition term based on the start and end dates and recognition method chosen. The mid-month start date and end dates are included in the revenue recognition term.

Example amounts are based on an invoice that shows following:

-   Revenue recognition start date: August 20
    
-   Revenue recognition end date: December 19
    
-   1 item sold for $400 with a revenue recognition template chosen
    

Saving the invoice creates a revenue recognition schedule to recognize revenue of $400.00 over four months. Since each partial month counts as a period, the schedule shows five periods. The recognition method set on the revenue recognition template affects the amounts recognized during each period.

The following examples illustrate the differences in amortization amounts per period with each recognition method:

-   [Straight-line, by even periods](#bridgehead_N1684177)
    
-   [Straight-line, prorate first & last period (with rounding)](#bridgehead_N1684400)
    
-   [Straight-line, using exact days](#bridgehead_N1685744)
    
-   [Straight-line, prorate first & last period (period-rate)](#bridgehead_N1686006)
    
-   [Straight-line, prorate first & last period vs. Straight-line, prorate first & last period (period-rate)](#bridgehead_N1686358)
    

## Straight-line, by even periods {#bridgehead_N1684177}

This method divides the income from the net sales amount evenly across all periods. Currency amounts aren't prorated based on the number of days in any period.

| Period | Income |
| --- | --- |
| August | $80.00 |
| September | $80.00 |
| October | $80.00 |
| November | $80.00 |
| December | $80.00 |
| **Total** | $400.00 |

## Straight-line, prorate first & last period (with rounding) {#bridgehead_N1684400}

When using the Straight-line, prorate first & last period method, if rounding is required for amounts, the rounding difference is added to the last period.

This method recognizes revenue in equal amounts for periods other than the first and the final period regardless of the number of days in those periods.

Currency amounts are prorated for the first period and the final period based on the number of days in those periods divided by the total number of days between the Rev. Rec. Start and End dates. There are 122 days between August 20 and December 19, inclusive.

-   The first period is prorated for August 20 through August 31, or 12 days, inclusive of the 20th.
    
-   The final period is prorated for December 1 through December 19, or 19 days, inclusive of the 19th.
    
-   The middle periods recognize the balance equally.
    
-   The last period is rounded to $62.31.
    

| Period | Income | Calculation |
| --- | --- | --- |
| August | $39.34 | (12 ÷ 122) × $400 = $39.34 |
| September | $99.45 | 298.36 ÷ 3 = $99.45 |
| October | $99.45 | 298.36 ÷ 3 = $99.45 |
| November | $99.45 | 298.36 ÷ 3 = $99.45 |
| December (rounded) | $62.31 | (19 ÷ 122) × 400 + 0.01 = $62.31 |
| **Total** | $400.00 |  |

## Straight-line, using exact days {#bridgehead_N1685744}

This method recognizes revenue amounts individually for each period based on the number of days in each period. Because each day in the term recognizes an equal amount, each period may recognize a different amount.

-   The first period is prorated for August 20 through August 31, or 12 days.
    
-   The second period is prorated for the entire month of September, or 30 days.
    
-   The third period is prorated for the entire month of October, or 31 days.
    
-   The fourth period is prorated for the entire month of November, or 30 days.
    
-   The fifth period is prorated for December 1 through December 19, or 19 days.
    
-   The total number of days is 122.
    
-   The amount per day is $3.2787 when rounded to four decimal places.
    

| Period | Income |
| --- | --- |
| August | $39.34 |
| September | $98.36 |
| October | $101.64 |
| November | $98.36 |
| December | $62.30 |
| **Total** | $400.00 |

## Example with Rev Rec Dates Specified on Sales Order {#bridgehead_1487719286}

When you use the term source Rev Rec Dates Specified on Sales Order, the same number of days and amount per day are used. When the sales order is later billed, the sales order remains the reference. In this example, the sales order uses the same dates and amounts as the invoice example. However, it's billed in three invoices. One item is billed in the first invoice, two in the second, and the fourth in the third to complete the billing.

| Period | Sales Order | Inv. 1 | Inv. 2 | Inv. 3 | Total from Invoices |
| --- | --- | --- | --- | --- | --- |
|  | $400.00 | $100.00 | $200.00 | $100.00 | $400.00 |
| August | 39.34 | 39.34 |  |  | 39.34 |
| September | 98.36 | 60.66 (100-39.34) | 37.70 (98.36-60.66) |  | 98.36 |
| October | 101.64 |  | 101.64 |  | 101.64 |
| November | 98.36 |  | 60.66 (200-37.70-101.64) | 37.70 | 98.36 |
| December | 62.30 |  |  | 62.30 | 62.30 |

## Straight-line, prorate first & last period (period-rate) {#bridgehead_N1686006}

This method determines the total number of periods in the schedule, then prorates the period amount allocated to the first and final periods based on the number of days in each of those periods. An even amount is allocated to all other periods.

For example, when recognizing $400 of revenue across the year from August 20 through December 19, the revenue allocation is calculated as follows:

| Period | Income | Calculation |
| --- | --- | --- |
| August | $38.71 | (12 ÷ 31) × $100 = $38.71 |
| September | $100.00 |  |
| October | $100.00 |  |
| November | $100.00 |  |
| December | $61.29 | (19 ÷ 31) × $100 = $61.29 |
| **Total** | $400.00 |  |

1.  First, the number of total periods is calculated. This example has exactly 4 periods. When the Rev. Rec. Start date is in the middle of a period, and the End date is equal to the Start date minus one period, the first and final periods constitute one full period, as in the case of August 20 and December 19.
    
2.  The amount for each period is calculated by taking the total amount ($400) and dividing that by the number of periods (4).
    
    400 ÷ 4 = $100 per period
    
3.  The first period is prorated for August 20 through August 31, or 12 days divided by the total number of days in the first and last periods (12 + 19 = 31).
    
    (12 ÷ 31) × 100 = $38.71
    
4.  The final period is prorated for December 1st through December 19th, or 19 days including the 19th.
    
    (19 ÷ 31) × 100 = $61.29
    
5.  The middle periods recognize the period amount of $100
    

## Straight-line, prorate first & last period vs. Straight-line, prorate first & last period (period-rate) {#bridgehead_N1686358}

On an invoice, you sell one line-item for $1200. The Rev. Rec. Start date is January 17, 2024 and the End date is January 16, 2025. The revenue is recognized as follows using each method:

| Period | Straight-line, prorate first & last period | Straight-line, prorate first & last period (period-rate) |
| --- | --- | --- |
| January 2024 | $49.18 | $54.84 |
| February 2024 | $99.85 | $100.00 |
| March 2024 | $99.85 | $100.00 |
| April 2024 | $99.85 | $100.00 |
| May 2024 | $99.85 | $100.00 |
| June 2024 | $99.85 | $100.00 |
| July 2024 | $99.85 | $100.00 |
| August 2024 | $99.85 | $100.00 |
| September 2024 | $99.85 | $100.00 |
| October 2024 | $99.85 | $100.00 |
| November 2024 | $99.85 | $100.00 |
| December 2024 | $99.85 | $100.00 |
| January 2025 | $52.47 | $45.16 |

### Related Topics

-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Understanding Revenue Recognition Template Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html)
-   [Defining a Revenue Recognition Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1686978.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
