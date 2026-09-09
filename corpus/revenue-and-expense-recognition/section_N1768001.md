---
id: "section_N1768001"
type: "section"
title: "Amortization Template Term Reference"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Amortization Template Term Reference"
parent: "section_N1767815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html"
anchors: ["bridgehead_N1768166", "bridgehead_N1768215", "procedure_N1768228", "procedure_N1768306", "bridgehead_N1768391", "bridgehead_N1768466", "bridgehead_N1768528", "bridgehead_N1768558", "bridgehead_N1770243", "bridgehead_N1770687"]
sha256: "118e14df6433f9664e7cb413f8a6aadc0512c86d4076bb3e76075d2f5802ee7f"
---

Amortization templates provide the basic terms used to generate amortization schedules. You should review the following descriptions to get a good understanding of amortization terms before you begin to define them:

-   [Amortization Template Types](#bridgehead_N1768166)
    
-   [Amortization Methods](#bridgehead_N1768215)
    
-   [Amortization Term Source](#bridgehead_N1768391)
    
-   [Amortization Accounts](#bridgehead_N1768466)
    
-   [Amortization Period](#bridgehead_N1768528)
    
-   [Amortization Period Offset and Start Offset](#bridgehead_N1768558)
    
-   [Amortization Residual](#bridgehead_N1770243)
    
-   [Amortization Initial Amount](#bridgehead_N1770687)
    

You set these terms on the Amortization Template page at Lists > Accounting > Amortization Templates > New. All amortization templates are public templates.

For steps to follow to create each amortization template, see [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html).

For information about how amortization posting occurs, see [Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776086.html).

## Amortization Template Types {#bridgehead_N1768166}

Two types of templates are available:

-   **Standard** - Select this type for most templates. This type requires you to enter a recognition Method and Term Source for the template.
    
-   **Variable** - Select this type to use this template for percent-complete expense recognition for service items that are part of projects. A variable amortization schedule amortizes its balance as time is entered against the related project, until the project is completed.
    
    This type of schedule is available if the Project Management feature is enabled. For information, see [Using Percent-Complete Amortization for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780615.html).
    
    Note:
    
    If you select a type of Variable, you can't set the following template fields: Method, Term Source, Amortization Period, Period Offset, Start Offset, and Initial Amount. Variable amortization scheduled don't include forecast amounts.
    

## Amortization Methods {#bridgehead_N1768215}

You can choose from a number of straight-line amortization methods, or define your own custom method.

## Straight-Line Amortization Methods {#procedure_N1768228}

The following straight-line methods are available:

-   **Straight-line, by even periods** - amortizes expenses evenly for each period. Currency amounts aren't prorated based on the number of days in any period. All periods recognize equal amounts.
    
    The term includes the start date and end date you define.
    
-   **Straight-line, prorate first & last period** - amortizes equal amounts for periods other than the first and the final period, regardless of the number of days in each period. Amounts are prorated for the first period and the final period based on the number of days in each period.
    
-   **Straight-line, using exact days -** amortizes amounts individually for each period based on the number of days in each period. Because each day in the term recognizes an equal amount, each period may recognize a different amount.
    
-   **Straight-line, prorate first & last period (period-rate)** - determines the full number of periods in the schedule and allocates expenses based on the proportional period amount.
    

For examples of how expenses are recognized using straight-line methods, see [Straight-Line Amortization Method Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1771014.html).

## Custom Amortization Methods {#procedure_N1768306}

If you select a Method of Custom, you can define amortization terms that can include uneven periods, amounts, and multiple expense accounts.

For example, a custom schedule may be defined as:

-   1st period - 40% of expense posts to expense account 6000, 10% to account 6001
    
-   2nd period through 6th period - 10% of expense to posts to account 6002
    

When you select Custom in this field, you define amortization terms by entering information in the columns at the bottom of the page:

-   **Account** - the expense account you want to post deferred expenses into.
    
-   **Period Offset** - the number of periods to postpone the start of the amortization schedule for this line. The first period to recognize has an offset of zero.
    
    For example, if your amortization terms are based on 30-day periods, enter a 2 in this field to wait 60 days before you begin recognizing revenue for this line.
    
    You can recognize different amounts to different accounts within the same period when you set several lines to the same period offset value.
    
-   **Amount** - the expense amount to recognize as a percentage or a currency value.
    

## Amortization Term Source {#bridgehead_N1768391}

The Term Source controls how the amortization period is determined. Select from the following:

-   **Transaction Date** - sources the date specified in the originating transaction, such as a vendor bill.
    
-   **Receipt Date** - sources the receipt date on bills associated with an item receipt, using the receipt date as the amortization start date. The receipt date is used generally for fixed assets entered on vendor bills.
    
    For example, you could set up the following term source amortization:
    
    -   On 1/1/2006, you enter a bill for a $3600 computer. You set an amortization period of 36 months and a period offset of 1 month. Amortization start or end dates are ignored.
        
    -   On 2/1/2006, the computer on the purchase order is received into inventory.
        
    -   On 3/1/2006, amortization begins.
        
    
    Note:
    
    If you select Receipt Date as the term source for a template but no receipt exists, for example when billing in advance, then NetSuite uses the transaction date to determine the amortization period.
    

## Amortization Accounts {#bridgehead_N1768466}

The following types of accounts are used for amortization:

-   **Deferral Account** - the Deferred Expense type account used to post the prepaid expense to be amortized or the initial cost of an asset to be depreciated. If you leave this field blank on a template, the deferred expense account specified on the transaction is used. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).
    
    If you select a GL account, NetSuite overrides the expense account shown on the transaction and posts to the account selected on the template.
    
-   **Contra Account** - the account that accumulates amortized balances. This account is used most often for depreciated expenses.
    
-   **Target Account** - the account used to record amortized expenses over time. If you leave this field blank on a template, the expense account specified on the transaction is used. Select a specific GL account on the template to override the expense account shown on the transaction or item record.
    

## Amortization Period {#bridgehead_N1768528}

The Amortization Period is the number of periods over which the amount should be amortized. For example, you can enter 60 to amortize the amount over 60 periods starting from the amortization start date.

The starting period is specified by the amortization start date on the transaction. If no amortization start date is specified, the posting date of the transaction is the amortization start date.

If an amortization end date is indicated on the transaction, you don't need to complete this field.

## Amortization Period Offset and Start Offset {#bridgehead_N1768558}

You can define an Offset value for an amortization template to delay the start of a schedule. Two types of Offset are available:

-   **Period Offset** moves the entire amortization period ahead by the number of periods you specify, keeping the same number of periods.
    
    For example, if your amortization terms are based on 30-day periods, enter a 2 in this field to wait 60 days before you begin recognizing expenses. This can be useful for services you purchase that have a probationary or trial period.
    
-   **Start Offset** delays the beginning of amortization, changing the number of periods, and keeping the same end date.
    
    To use a start offset, you specify the number of periods to skip before the start of the amortization for a schedule. Setting a start offset changes the number of periods in the schedule because it postpones the beginning, but doesn't change the final period of the schedule.
    
    For example, to begin amortization in the third month of a 12-month schedule, enter 2 for the Start Offset. The number of periods in the schedule is reduced by the start offset value.
    

## Amortization Residual {#bridgehead_N1770243}

The residual is the amount or percentage to remain in the deferral account and not be amortized. A residual amount generally represents the salvage value of a fixed asset.

For example, you entered a $1400 bill for a new computer. The computer is set to amortize the expense as follows:

-   Method = Straight-line, by even periods
    
-   Amortization period = 12 months
    
-   Residual = $200
    

This results in the following amortization schedule:

| Period | Amortization Amount | Deferral Account Balance (Fixed Asset) | Debit Target Account Balance (Depreciation Expense) | Credit Contra Account (Accumulated Depreciation Expense) | Credit Contra Account Cumulative Balance |
| --- | --- | --- | --- | --- | --- |
| 1 |  | 1400 |  |  |  |
| 2 | 100 | 1300 | 100 | 100 | 100 |
| ... | ... | ... | ... | ... | ... |
| 12 | 100 | 200 (residual) | 100 | 100 | 1200 |

Note:

A residual amount entered on a transaction overrides a residual amount entered on an item record.

## Amortization Initial Amount {#bridgehead_N1770687}

The initial amount is a percentage or fixed currency amount to be amortized in the first amortization period. After the initial amount, the remainder to be amortized is recognized according to the amortization schedule.

For example, you've contracted with a vendor who will recognize 25% of a $1200 item immediately.

-   Initial amount = 25%, or $300.
    
-   Method = Straight-line, by even periods
    
-   Amortization period = 12 months
    

The amortization of the remaining $900 is recognized at $75 per period over the remainder of the schedule:

| Period | Expense |
| --- | --- |
| 1 | $300 (initial) |
| 2 | $75 |
| 3 | $75 |
| ... | ... |
| 12 | $75 |

### Related Topics

-   [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html)
-   [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html)
-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)
-   [Associating Amortization Templates with Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
