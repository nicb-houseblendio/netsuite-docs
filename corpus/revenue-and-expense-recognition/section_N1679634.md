---
id: "section_N1679634"
type: "section"
title: "Understanding Revenue Recognition Template Terms"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Creating Revenue Recognition Templates > Understanding Revenue Recognition Template Terms"
parent: "section_N1679446"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html"
anchors: ["bridgehead_N1679779", "bridgehead_N1679836", "procedure_N1679850", "procedure_N1679928", "bridgehead_N1680012", "bridgehead_N1683147", "bridgehead_N1683393", "bridgehead_N1683713"]
sha256: "05d130628fcd4041b9796d043fa0518909c56de148e79efa29328dd2771c56d6"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For the equivalent information for Advanced Revenue Management (Essentials), see [Revenue Recognition Rule Field Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4356113783.html).

Revenue recognition templates provide the basic terms used to generate revenue recognition schedules. Review the following descriptions of the terms that you use in NetSuite revenue recognition templates before you begin to define them:

-   [Revenue Recognition Template Types](#bridgehead_N1679779)
    
-   [Revenue Recognition Methods](#bridgehead_N1679836)
    
-   [Revenue Recognition Term Source](#bridgehead_N1680012)
    
-   [Revenue Recognition Period](#bridgehead_N1683147)
    
-   [Revenue Recognition Period Offset and Start Offset](#bridgehead_N1683393)
    
-   [Revenue Recognition Initial Amount](#bridgehead_N1683713)
    

These terms appear on the Revenue Recognition Template page at _Lists > Accounting > Revenue Recognition Templates > New_.

For the steps to create each revenue recognition template, see [Defining a Revenue Recognition Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1686978.html).

## Revenue Recognition Template Types {#bridgehead_N1679779}

Two types of templates are available:

-   **Standard** - Select this type for most templates. Standard templates require a recognition Method and Term Source.
    
-   **Variable** - Select this type to use this template for percent-complete revenue recognition for service items that are part of projects. A variable revenue recognition schedule recognizes revenue for its balance as time is entered against the related project, until the project is completed.
    
    This type of schedule is available if the Project Management feature is enabled. For information, see [Using Percent-Complete Revenue Recognition for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1694795.html).
    

Note:

If you select a type of Variable, you can't set the following template fields: Method, Term Source, Recognition Period, Period Offset and Start Offset.

## Revenue Recognition Methods {#bridgehead_N1679836}

You can choose from several straight-line revenue recognition methods, or define your own custom method.

## Straight-Line Revenue Recognition Methods {#procedure_N1679850}

The following straight-line methods are available:

-   **Straight-line, by even periods** - recognizes revenue evenly for each period. Amounts aren't prorated based on the number of days in any period. All periods recognize equal amounts.
    
    The term includes the start date and end date you define.
    
-   **Straight-line, prorate first & last period** - recognizes equal amounts for periods other than the first and the final period, regardless of the number of days in each period. Amounts are prorated for the first period and the final period based on the number of days in each period.
    
-   **Straight-line, using exact days** - recognizes revenue amounts individually for each period based on the number of days in each period. Because each day in the term recognizes an equal amount, each period may recognize a different amount.
    
-   **Straight-line, prorate first & last period (period-rate)** - determines the full number of periods in the schedule and allocates revenue based on the proportional period amount.
    

For examples of how revenue is recognized using straight-line methods, see [Straight-Line Revenue Recognition Method Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1684020.html).

## Custom Revenue Recognition Methods {#procedure_N1679928}

The Custom method enables you to define revenue recognition terms that include uneven periods, amounts, and multiple income accounts.

For example, you can define a custom schedule as:

-   1st period - 40% of net income posts to income account 4000, 10% to account 4001
    
-   2nd period through 6th period - 10% of net income to posts to account 4002
    

When you select Custom for the Method, you define revenue recognition terms by entering information in the columns in the lower portion of the page:

-   **Account** - the income account you want to post deferred revenue into. Make sure the currency on the account matches the intended transaction currency. Create multiple custom method templates as needed to support foreign currency transactions.
    
-   **Period Offset** - the number of periods to postpone the start of the recognition schedule for this line. The first period to recognize has an offset of zero.
    
    For example, if your recognition terms are based on 30-day periods, enter a 2 in this field to wait 60 days before you begin recognizing revenue for this line.
    
    You can recognize different amounts to different accounts within the same period when you set several lines to the same period offset value.
    
-   **Amount** - the revenue amount to recognize as a percentage or a currency value. Include the percent sign to indicate a percentage, for example, 10%.
    

## Revenue Recognition Term Source {#bridgehead_N1680012}

Term Source determines which dates to use to recognize revenue.

Select from the following:

-   **Rev Rec Dates Specified on Transaction** - Uses the invoice or cash sale as the source to determine the revenue recognition period.
    
    The revenue recognition period is determined by Rev. Rec. start and end dates entered on the invoice or cash sale.
    
    The invoice or cash sale Rev. Rec. dates can use the sales order as the original source, but subsequent changes to Rev. Rec. dates on the sales order **don't** change the Rev. Rec. dates on the invoice.
    
    When you change the Rev. Rec. start or end dates on the invoice or cash sale before the schedule is created, the revenue recognition schedule refreshes based on the new dates. After a schedule is created, the dates can't be changed.
    
    If the term source Rev Rec Dates Specified On Transaction is selected on a template that's used on a sales order, then the sales order revenue recognition dates are used because the invoice dates aren't yet known.
    
-   **Rev Rec Dates Specified on Sales Order** - Uses the sales order revenue recognition dates as the source to determine the revenue recognition period. The revenue recognition period is determined by Rev Rec start and end dates entered on the sales order. This choice appears only when you use the sales order feature.
    
    The Rev Rec dates are derived from the sales order. Subsequent changes to Rev Rec dates on the sales order **don't** change the Rev Rec dates on an invoice that was created prior to the change. Changes to sales order dates **do** change the dates on the schedule if no journal entry has posted from the schedule.
    
    If the sales order has multiple invoices, revenue recognition schedules are created for each invoice. The sales order determines the periods and amounts per period. The revenue recognition schedule for the first invoice begins with the first period and amount and includes as many periods as needed to schedule the invoice amount. Schedules for subsequent invoices begin with any remaining amount in the last period of the previous schedule and continue until the full invoice amount is scheduled.
    
    For example, create a sales order with the following values on an item line:
    
    | Field | Value |
    | --- | --- |
    | Rev. Rec. Schedule | Standard template with the following values:
    -   **Term Source** - Rev Rec Dates Specified on Sales Order
    -   **Method** - Straight-line, by even periods
    -   **Period** - 12
    
     |
    | Rev. Rec. Start Date | January 1 |
    | Rev. Rec. End Date | December 31 |
    | Quantity | 10 |
    | Unit Price | $120 |
    | Amount | $1,200 |
    
    For purposes of revenue recognition, you have $100 per month for 12 months beginning in January.
    
    If you create the first invoice for a quantity of 3.5, you get a revenue recognition schedule for $420. It has $100 per month for the first four months of January, February, March, and April, and it has $20 in May. Then when you create the next invoice, its revenue recognition schedule begins with $80 in May. If the second invoice is again for a quantity of 3.5, the $420 is divided with $80 in May, $100 each month for June, July, and August, and $40 in September. When you invoice the final $360, it's scheduled for $60 in September and $100 each month for October, November, and December. The invoice dates have no role in determining the revenue recognition schedule dates.
    
    For another example of the behavior of this term source with multiple invoices, see [Example with Rev Rec Dates Specified on Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1684020.html#bridgehead_1487719286).
    
-   **Billing Schedule, Transaction Date on Sales Order** -Uses the transaction date of the sales order to determine the revenue recognition start date.
    
    This choice appears only when the Advanced Billing feature is enabled. For more information about Advanced Billing, see [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html). This term source doesn't support the fixed bid, milestone project billing type.
    
    This term source creates a schedule to recognize revenue based on the Sales Order transaction date. NetSuite dates subsequent invoices based on the assigned billing schedule.
    
    Rev Rec start and end dates entered on the Sales Order **aren't** sourced.
    
    For example, a Sales Order is set up as follows:
    
    -   Sales Order transaction date = Mar. 25, 2006
        
    -   Billed quarterly, 4 bills total
        
    
    | Bill created on: | Rev Rec dates: |
    | --- | --- |
    | Mar. 25, 2006 | Mar. 25 through June 24, 2006 |
    | June 25, 2006 | June 25 through Sept. 24, 2006 |
    | Sept. 25, 2006 | Sept. 25 through Dec. 24, 2006 |
    | Dec. 25, 2006 | Dec. 25, 2006, through Mar. 24, 2007 |
    

-   **Billing Schedule, Rev Rec Date on Sales Order** - Uses the sales order revenue recognition dates as the source to determine the revenue recognition period.
    
    This choice appears only when the Advanced Billing feature is enabled. For more information about Advanced Billing, see [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html). This term source doesn't support the fixed bid, milestone project billing type.
    
    This term source creates a schedule to recognize revenue based on the Sales Order revenue recognition dates, not the transaction dates. NetSuite dates subsequent invoices based on the assigned billing schedule.
    
    For example, a Sales Order is set up as follows:
    
    -   Sales Order Rev Rec Start Date = Mar. 25, 2006
        
    -   Billed quarterly, 4 bills total
        
    
    | Bill created on: | Rev Rec dates: |
    | --- | --- |
    | Mar. 25, 2006 | Mar. 25 through June 24, 2006 |
    | June 25, 2006 | June 25 through Sept. 24, 2006 |
    | Sept. 25, 2006 | Sept. 25 through Dec. 24, 2006 |
    | Dec. 25, 2006 | Dec. 25, 2006, through Mar. 24, 2007 |
    

## Revenue Recognition Period {#bridgehead_N1683147}

The **Recognition Period** defines the range of time for revenue recognition by setting the number of periods over which the schedule is recognized. For example, if you enter **12**, then the schedule runs for 12 periods starting from the Rev Rec Start Date. If the Rev Rec Start Date is mid-month, the partial month counts as one of the periods in the total.

If you enter a start date in the transaction and specify a recognition period in the template, NetSuite determines the appropriate end date and generates the recognition schedule.

If you enter both a start date **and** an end date, then these dates override the recognition period set on the template.

If you enter **neither** a start date **nor** an end date, NetSuite uses the transaction date for the start date and the number of periods in the template to determine the end date. In this case, the end date is always the last day of the period, and partial periods are included in the count.

The following examples show how the recognition period field functions when you enter dates on line items in the transaction. The transaction date is mid-month, January 15, 2007. The January 1 start dates are entered in the line item as Rev. Rec. Start Date.

| **Start Date** | **End Date** | Recognition Period | Result |
| --- | --- | --- | --- |
| Jan. 1, 2007 | \[none\] | 12 | The schedule runs 12 full periods (Jan. 1, 2007 through Dec. 31, 2007.) NetSuite populates the end date as Dec. 31, 2007. |
| Jan. 1, 2007 | Nov. 1, 2007 | 12 | The schedule runs 11 full periods ((Jan. 1, 2007 through Nov. 1, 2007.) The start and end dates entered override the recognition period setting. |
| \[none\] | \[none\] | 12 | The schedule runs 12 periods. The first period is partial but counts in the total. NetSuite populates the start date as Jan. 1, 2007 and the end date as Dec. 31, 2007. |

## Revenue Recognition Period Offset and Start Offset {#bridgehead_N1683393}

You can define an Offset value for a revenue recognition template to delay the start of a schedule. Two types of Offset are available:

-   **Period Offset** moves the entire recognition period ahead by **x** number of periods, keeping the same number of periods.
    
    For example, if your amortization terms are based on 30-day periods, enter a 2 in this field to wait 60 days before you begin recognizing revenue. This can be useful for services you sell that have a probationary or trial period.
    
-   **Start Offset** delays the beginning of recognition, changing the number of periods, and keeping the same end date.
    
    To use a start offset, you specify the number of periods to postpone the start of the recognition for a schedule. Setting a start offset changes the number of periods in the schedule because it postpones the beginning, but doesn't change the final period of the schedule. You must have at least one more period in the schedule than the number of periods in the start offset.
    
    For example, you've contracted with a customer to recognize 25% of a $1200 item immediately.
    
    -   Initial amount = 25%, or $300.
        
    -   Method = Straight-line, by even periods
        
    -   Recognition period = 12 months
        
    
    The remaining $900 is recognized according to the item's schedule:
    
    | Period | Income |
    | --- | --- |
    | 1 | 0 |
    | 2 | 0 |
    | 3 | $300 (initial) |
    | 4 | $100 |
    | 5 | $100 |
    | ... | ... |
    | 12 | $100 |
    

## Revenue Recognition Initial Amount {#bridgehead_N1683713}

The initial amount is a percentage or fixed currency amount to be recognized in the first recognition period. After the initial amount, the remainder is recognized according to the revenue recognition schedule.

For example, you've contracted with a customer to recognize 25% of a $1200 item immediately.

-   Initial amount = 25%, or $300.
    
-   Method = Straight-line, by even periods
    
-   Recognition period = 12 months
    

The remaining $900 is recognized according to the item's schedule:

| Period | Income |
| --- | --- |
| 1 | $300 (initial) |
| 2 | $75 |
| 3 | $75 |
| ... | ... |
| 12 | $75 |

### Related Topics

-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Straight-Line Revenue Recognition Method Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1684020.html)
-   [Defining a Revenue Recognition Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1686978.html)
-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
