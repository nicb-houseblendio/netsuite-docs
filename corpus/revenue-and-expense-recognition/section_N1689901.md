---
id: "section_N1689901"
type: "section"
title: "Editing a Revenue Recognition Schedule"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Working with Revenue Recognition Schedules > Editing a Revenue Recognition Schedule"
parent: "section_N1689004"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689901.html"
anchors: ["procedure_N1689928"]
sha256: "9e2666a7296a5c990e2f08b73c6cb4a2572f759a504ae23162049c00c7299746"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Editing Revenue Recognition Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4369089832.html).

Depending on your setting for the preference Allow Users to Modify Revenue Recognition Schedules, you can change schedules after they're created. For more information about this preference, read [Setting Revenue Recognition Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678834.html).

To change the start or end dates of a revenue recognition schedule, or to place the schedule on hold, use the Manage Revenue Recognition page. For instructions to access this page, see [Managing Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4029604484.html).

On the revenue recognition schedule record, you can change the name of the revenue recognition schedule and change values in schedule lines before revenue is recognized.

#### To edit a revenue recognition schedule: {#procedure_N1689928}

1.  Go to _Lists > Accounting > Revenue Recognition Schedules_.
    
    You can filter the list by **Posting Period**, **Status**, and **Transaction Type** to reduce the number of revenue recognition schedules listed.
    
2.  Click **Edit** next to the schedule you want to edit.
    
3.  Enter a new **Name** if desired.
    
4.  In the schedule lines, click in the field you want to change to begin editing, and click **OK** when you're finished with that line.
    
    The following fields appear if revenue hasn't been recognized:
    
    -   **Account** - Income account that this line's revenue amount posts to when it's recognized. By default, this is the income account specified on the item record.
        
    -   **Posting Period** - Period when revenue for this line is scheduled to be recognized.
        
        Periods that are locked for A/R are generally not available to select as posting periods. Those with the Administrator role or a custom role with the Override Period Restrictions permission may select periods that are locked.
        
    -   **Is Recognized** - Check this box to indicate that the revenue amount on the line has been recognized by a manual journal entry outside the revenue recognition journal entry process. The schedule isn't included on the Create Revenue Recognition Journal Entry page for the specified period when this box is checked.
        
        If you check this box, be sure that the manual journal entry to recognize the revenue amount has been created, or create the journal entry as the next step in your process. When the Revenue Commitments feature is enabled, lines with this box checked are considered in deferred revenue reclassification.
        
    -   **Amount** - Amount to be recognized for this line of the schedule.
        
        The total schedule amount must equal the sales amount or the VSOE allocation amount on the line in the source transaction.
        
5.  Click **Save**.
    

### Related Topics

-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Reviewing the Revenue Recognition Schedules List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689265.html)
-   [Viewing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689644.html)
-   [Mass Updating Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690102.html)
-   [Deleting a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690402.html)
-   [Cases When a Revenue Recognition Schedule May Not Be Created](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691758.html)
-   [Creating a Revenue Recognition Schedule Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0822023107.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
