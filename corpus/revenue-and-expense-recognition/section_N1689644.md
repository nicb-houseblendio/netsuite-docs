---
id: "section_N1689644"
type: "section"
title: "Viewing a Revenue Recognition Schedule"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Working with Revenue Recognition Schedules > Viewing a Revenue Recognition Schedule"
parent: "section_N1689004"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689644.html"
anchors: ["procedure_N1689663"]
sha256: "90bfc6f5e5130f40df25b75db58bb352ece8a65aa799450b147ecb84cb6afcec"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Viewing Revenue Recognition Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4380140655.html).

Revenue recognition schedules determine the journal entries that need to be generated. Revenue isn't recognized until the revenue recognition journal entries for the scheduled posting period are generated. See [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html).

#### To view a revenue recognition schedule: {#procedure_N1689663}

1.  Go to _Lists > Accounting > Revenue Recognition Schedules_.
    
2.  Click **View** next to a schedule.
    

Note:

You can also view a revenue recognition schedule from the sales transaction that created it. On the sales transaction, on the **Items** subtab, in the **Rev. Rec. Schedule** column, click **View** to open the schedule.

The following information appears at the top of the page:

-   **Name** - By default, this is the same as the template name. You can edit the name if the Allow Users to Modify Revenue Recognition Schedules preference is enabled. See [Editing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689901.html).
    
-   **Created From** - Link to the source transaction for the schedule.
    
-   **Job** or **Project** - The job or project associated with the schedule. Jobs and projects can be associated only with variable revenue recognition schedules.
    
-   **Template** - Link to the revenue recognition template used to create the schedule.
    
-   **Type** - Either Standard or Variable. See [Revenue Recognition Template Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1679779).
    
-   **Method** - Eee [Revenue Recognition Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1679836).
    
-   **Term Source** - See [Revenue Recognition Term Source](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1680012).
    
-   **Recognition Period** - The number of periods over which the revenue from the schedule is recognized. This field is blank in the schedule if it's blank in the template.
    
-   **Start Date** - The date revenue recognition begins for this schedule.
    
-   **End Date** - The date the revenue recognition schedule ends.
    
-   **Status** - The schedule status can be one of the following:
    
    -   **Not Started** - No revenue has yet been recognized.
        
    -   **In Progress** - Some revenue has been recognized, but not all.
        
    -   **On Hold** - Some revenue may or may not have been recognized. No additional revenue can be recognized until the hold is removed.
        
    -   **Complete** - All revenue has been recognized for this schedule.
        
-   **Period Offset** and **Start Offset** - See [Revenue Recognition Period Offset and Start Offset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1683393)
    
-   **Initial Amount** - See [Revenue Recognition Initial Amount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1683713).
    
-   **Remaining Deferred Balance** - The amount on the schedule that hasn't yet been recognized.
    
-   **Total Recognized** - The amount on the schedule that's been recognized to date.
    
-   **Amount** - The total amount for the schedule including the amount already recognized and the remaining balance.
    
-   **Eliminate** - If this box is checked, the transaction from which the schedule was created is an intercompany transaction.
    

The following information shows for each line:

-   **Account** - Income account that this line's revenue amount posts to when it's recognized. By default, this is the item's income account.
    
-   **Posting Period** - Period in which this line is scheduled to be recognized.
    
-   **Is Recognized** - When this box is checked, it indicates that the revenue amount on the line has been recognized by a manual journal entry outside the revenue recognition journal entry process. The schedule isn't included on the Create Revenue Recognition Journal Entry page for the specified period. This box isn't checked by the system. This box appears on both Standard and Variable revenue recognition schedules.
    
-   **Date Executed** - Date of the journal entry that posts the amount on this line.
    
-   **Journal** - Number of the journal entry that posts the amount on this line. The number is a link to the journal entry record.
    
-   **Amount** - Amount to be recognized for this line of the schedule.
    
-   **Total Recognized** - Shows the cumulative amount recognized on the schedule to date.
    

Variable schedules, which are linked to Projects, also show the following information:

-   **% Amort. In Period** - Percentage of revenue recognized or to be recognized for that period.
    
-   **% Total Amortized** - Cumulative percentage of revenue recognized each period.
    

### Related Topics

-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Reviewing the Revenue Recognition Schedules List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689265.html)
-   [Editing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689901.html)
-   [Mass Updating Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690102.html)
-   [Deleting a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690402.html)
-   [Cases When a Revenue Recognition Schedule May Not Be Created](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691758.html)
-   [Creating a Revenue Recognition Schedule Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0822023107.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
