---
id: "section_N1771014"
type: "section"
title: "Straight-Line Amortization Method Examples"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Amortization Template Term Reference > Straight-Line Amortization Method Examples"
parent: "section_N1768001"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1771014.html"
anchors: ["bridgehead_N1771154", "bridgehead_N1771377", "bridgehead_N1772173", "bridgehead_N1772573"]
sha256: "1a7897807c9d1ccc8d8eaa47d9453759c3aa80f957509416addde1f82037a646"
---

When a straight-line method is used, purchase expenses are amortized over the scheduled term based on the start date, end date, and method chosen. The start date and end date are included in the amortization term.

Amortization examples in this section are based on a vendor bill that shows following:

-   Amortization start date 20 August
    
-   Amortization end date 19 December of the same year
    
-   Four items purchased for $400.00 each, for a total bill of $1,600
    
-   Each item line has a different amortization template associated with it, but the start and end dates are the same.
    

Saving the vendor bill creates four amortization schedules, each to amortize $400.00 over full four periods from August through December inclusive. When you count the number of periods that have amortization amounts, the total is five periods, but two are partial periods. The method set on the amortization template for each line determines the amounts amortized during each period.

The following examples show the differences in amortization amounts per period with each recognition method:

-   [Straight-line, by even periods](#bridgehead_N1771154)
    
-   [Straight-line, prorate first & last period (with rounding)](#bridgehead_N1771377)
    
-   [Straight-line, using exact days](#bridgehead_N1772173)
    
-   [Straight-line, prorate first & last period (period-rate)](#bridgehead_N1772573)
    

## Straight-line, by even periods {#bridgehead_N1771154}

This method divides the expense from the purchase amount evenly across all periods, even partial periods. Amounts aren't prorated based on the number of days in any period.

| Period | Expense |
| --- | --- |
| August | $80.00 |
| September | $80.00 |
| October | $80.00 |
| November | $80.00 |
| December | $80.00 |
| Total | $400.00 |

## Straight-line, prorate first & last period (with rounding) {#bridgehead_N1771377}

When using the Straight-line, prorate first & last period method, if rounding is required for amounts, then the rounding difference is added to the next to the last period.

This method amortizes equal amounts for periods other than the first and the final period, regardless of the number of days in each period.

Amounts are prorated for the first period and the final period based on the number of days in each period.

-   The first period is prorated for 20 August through 31 August, or 12 days.
    
-   The final period is prorated for 1 December through 19 December, or 19 days.
    
-   The middle periods amortize the balance equally ($400 - $39.34 - 62.30 = $298.36 ÷ 3 = $99.45). However, the next to last period is rounded to $99.46.
    

| Period | Expense | Calculation |
| --- | --- | --- |
| August | $39.34 | 12 ÷122 × $400 = $39.45 |
| September | $99.45 | $298.36 ÷ 3 = $99.45 |
| October | $99.45 | $298.36 ÷ 3 = $99.45 |
| November (rounded) | $99.46 | $298.36 ÷ 3 + 0.01 = $99.46 |
| December | $62.30 | 19 ÷122 × $400 = $62.30 |
| Total | $400.00 |  |

## Straight-line, using exact days {#bridgehead_N1772173}

This method amortizes amounts individually for each period based on the number of days in each period. Because each day in the term recognizes an equal amount, each period may recognize a different amount. The full amortization period is 122 days, which is $3.278689 per day.

-   The first partial period is prorated for 20 August through 31 August, or 12 days.
    
-   The second period is prorated for the entire month of September, or 30 days.
    
-   The third period is prorated for the entire month of October, or 31 days.
    
-   The fourth period is prorated for the entire month of November, or 30 days.
    
-   The fifth partial period is prorated for 1 December through 19 December, or 19 days.
    

| Period | Expense |
| --- | --- |
| August | $39.34 |
| September | $98.36 |
| October | $101.64 |
| November | $98.36 |
| December | $62.30 |
| Total | $400.00 |

## Straight-line, prorate first & last period (period-rate) {#bridgehead_N1772573}

This method determines the full number of periods in the schedule and allocates expenses based on the proportional period amount. The example has four full periods, and the amount per period is $100.

| Period | Note | Calculation | Expense |
| --- | --- | --- | --- |
| August | 12 is the number of days from 20 August to 31 August inclusive. | 12 days ÷ 31 days × $100 | $38.71 |
| September |  |  | $100.00 |
| October |  |  | $100.00 |
| November |  |  | $100.00 |
| December | 19 is the number of days from 1 December through 19 December inclusive | 19 days ÷ 31 days × $100 | $61.29 |
| Total |  |  | $400.00 |

### Related Topics

-   [Amortization Template Term Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
