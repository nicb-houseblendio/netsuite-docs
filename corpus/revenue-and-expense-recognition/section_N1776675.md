---
id: "section_N1776675"
type: "section"
title: "Viewing an Amortization Schedule"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Schedules > Viewing an Amortization Schedule"
parent: "section_N1776086"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776675.html"
anchors: ["procedure_N1776703"]
sha256: "500d30b0d3ad1a7b0281a6e3a70f582012568c1a7c64e1bb4d26b188c4ce6434"
---

You can view detailed information for each amortization schedule.

The Lists permission Amortization Schedules controls access to amortization schedules. For more information, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).

#### To view an amortization schedule: {#procedure_N1776703}

1.  Go to _Lists > Accounting > Amortization Schedules_.
    
2.  Click **View** next to a schedule.
    

Note:

You can also view an amortization schedule from the purchase transaction that created it. On the transaction, on the **Expenses** or **Items** subtab, in the **Amort. Schedule** column, click **View** to open the schedule.

When you view an individual schedule, this header information applies to all lines:

-   **Name** - Shows the name of the schedule. This is the same as the template name by default, but it can be changed.
    
-   **Created From** - Shows the transaction type that the schedule was created from.
    
    If you click this link to open the transaction, the line that generated the schedule is highlighted.
    
-   **Template** - Shows the name of the template that created the schedule.
    
-   **Type** - Identifies whether the schedule is Standard or Variable.
    
-   **Method** - Identifies the method used to set amortization terms for the expense.
    
-   **Term Source** - Shows how the recognition period is determined, from either the transaction date or the receipt date.
    
-   **Start Date** - Shows the date expense recognition begins for this schedule.
    
    The starting period is specified by the recognition start date on bills. If no recognition start date is specified, the posting date of the bill is the recognition start date.
    
-   **End Date** - The end date entered for this schedule appears here.
    
-   **Status** - The amortization status can be one of the following:
    
    -   **Not Started** - No expense has yet been recognized.
        
    -   **In Progress** - Some expense has been recognized, but not all.
        
    -   **Complete** - All expense is recognized for this schedule.
        
-   **Period Offset** - Specifies the number of periods to postpone the start of recognition for the entire schedule.
    
-   **Start Offset** - Specifies the number of periods to postpone the start of the recognition for a schedule.
    
-   **Residual** - Shows the amount or percentage to remain in the deferral account and not be amortized.
    
-   **Initial Amount** - The percentage or amount to be recognized in the first recognition period.
    
-   **Remaining Deferred Balance** - Shows the amount on the schedule that hasn't yet been recognized.
    
-   **Total Amortized** - Shows the amount on the schedule that's already been recognized to date.
    
-   **Amount** - Shows the total amortization amount for the schedule, including amounts already recognized and amounts yet to be recognized.
    
-   **Eliminate** - If this box is checked, the transaction from which the schedule was created is an intercompany transaction.
    

The following information shows for each line:

-   **Account** - The expense account that this line's expense amount is recognized to.
    
    This defaults to show the item's expense account.
    
-   **Posting Period** - The period this line is scheduled to be recognized in.
    
    If the Start Date of a schedule is in a closed period, the amount that would've been recognized in that period is posted to the oldest open period.
    
-   **Is Recognized** - A check box to specify that this amount has been recognized by a manual entry.
    
    If this box is checked, the schedule isn't included on the Create Amortization Journal Entry page for the certain period.
    
-   **Date Executed** - The date of the journal entry that posts the amount.
    
-   **Journal** - The number of the journal entry that posts the amount.
    
    You can click this number to view the journal entry.
    
-   **Amount** - The amount to be recognized for this line of the schedule.
    
-   **Total Amortized** - Shows the cumulative amount already recognized on the schedule to date.
    

Variable schedules, which are linked to Projects, also show the following information:

-   **Project** - Shows a link to the associated project record.
    
-   **% Amort. In Period** - Shows the amount of the schedule that's been amortized in that period.
    
-   **% Total Amort** - Shows the percentage of the schedule already recognized for all periods.
    

### Related Topics

-   [Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776086.html)
-   [Reviewing the Amortization Schedules List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776296.html)
-   [Editing an Amortization Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777207.html)
-   [Mass Updating Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777416.html)
-   [Creating an Amortization Schedule Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0822030054.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
