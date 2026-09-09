---
id: "section_N1692238"
type: "section"
title: "Generating Revenue Recognition Journal Entries"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Working with Revenue Recognition Journal Entries > Generating Revenue Recognition Journal Entries"
parent: "section_N1691981"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1692238.html"
anchors: ["procedure_N1692268"]
sha256: "288e98bf2a7cd1d1519d81ca6f5e9a6524727c23f50da5fd9b490c0c612b5c8d"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4357047027.html).

To recognize deferred revenue that's due to post, you create revenue recognition journal entries.

Use the Create Revenue Recognition Journal Entries page to identify and select the transactions that require a journal entry for a posting period. This page retrieves a list of transactions based on the existing revenue recognition schedules generated for sales transactions. You can filter the list of transactions displayed. Schedules whose status is On Hold aren't included in the list.

NetSuite creates revenue recognition journal entries when you click the Create Journal Entries button on this page. Up to 50,000 revenue recognition schedules may be included in a single summarized journal entry. Multiple journal entries are created if you process more than 50,000 schedules or exceed the 1,000 line limit for detailed journal entries.

For example, if 50,000 revenue schedules use the same accounts and have the same classifications (class, department, location, and custom segments):

-   If the accounting preference Create Revenue Journals in GL is set to Detail, the process creates 100 journal entries. Each journal entry has 1,000 lines with two lines per revenue schedule.
    
-   If the accounting preference Create Revenue Journals in GL is set to Summary, the process creates one journal entry with two lines. The Details column in the journal entry includes a link that says 50,000 rows. The link opens a popup page that displays lines for the 50,000 revenue schedules.
    

For more information about line limitations in NetSuite, see [Line Limitations for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159361099314.html).

The journal entries post immediately upon clicking the button or are routed for approval, if required.

Note:

The time required to complete processing the schedules varies depending on the number of schedules. Completion may require several hours if you're processing thousands of schedules.

If you void or delete a revenue recognition journal entry, the link to the journal is removed from the revenue recognition schedule. The revenue schedule becomes available for recognition in the same period as the journal you voided or deleted.

#### To generate revenue recognition journal entries: {#procedure_N1692268}

1.  Go to _Transactions > Financial > Create Revenue Recognition Journal Entries_.
    
    You can also access the Create Revenue Recognition Journal Entries page directly from your dashboard by setting up the Revenue Recognition Entries Pending reminder. See [Setting Up a Reminder for Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1693505.html).
    
2.  Select a posting period.
    
    Note:
    
    You can't post revenue recognition journal entries in closed periods or in periods that are locked for A/R as part of the Period Close Checklist.
    
3.  In the **Journal Entry Date** field, set the transaction date of the revenue recognition journal entry you're creating.
    
    You can set the default date that shows in this field by setting a preference at _Setup > Accounting > Accounting Preferences_. Select a date in the **Default Revenue Recognition Journal Date To** field.
    
4.  If your role has permission to enter journal entries that are approved, check the **Approve Journal** box to approve the journal entry when you save it. Clear this box to submit this journal entry for approval after it's entered. For another way to approve journal entries, see [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html).
    
5.  If you use NetSuite OneWorld, select the **Subsidiary** to associate with this journal entry.
    
    When a journal entry is associated with a subsidiary, the journal posts to that subsidiary and the schedule is restricted to be viewed only by entities associated with the subsidiary.
    
6.  Use the filters at the top of the page to limit the list of source transactions scheduled to recognize revenue for this period.
    
    For information about the filter fields available, see [Filtering the Revenue Recognition Source Transaction List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1692710.html).
    
    The page shows a list of revenue recognition journal entries due to post, subject to the filters you select. The following information is shown on each line:
    
    -   **Source Transaction** - A link to the related transaction.
        
    -   **Customer** - A link to the related customer.
        
    -   **Project** - A link to the related project.
        
    -   **Type** - Shows if the schedule is Standard or Variable.
        
    -   **% Recog.** - The total percentage of a variable schedule recognized prior to this journal entry.
        
    -   **% Complete** - The total percentage completed of a project that's related to a variable schedule.
        
        The difference between the % Recognized and the % Complete is the Amount that's recognized in the current period on this journal entry.
        
    -   **Schedule Name** - A link to the related revenue recognition schedule.
        
    -   **Template Name** - A link to the related revenue recognition template.
        
    -   **Transaction Type** - The type of originating transaction.
        
    -   **Amount** - The amount to be recognized on the journal entry for this line.
        
7.  Check or clear the **Select Individual Schedules** box:
    
    -   When you check the box, journal entries are created only for schedules you select. After you filter the list to show particular schedules, check the box in the Select column next to each schedule you want to generate journal entries.
        
        If there are multiple pages of transactions shown when selecting schedules, the following is true:
        
        -   If you click **Mark All** or **Unmark All**, only boxes on the current page are affected.
            
        -   You must click **Create Journal Entries** to create an entry for each page of schedules.
            
    -   When you clear the box, the list of schedules displayed is limited to a sample of 100 schedules. An **Estimate** button appears at the top of the page.
        
        -   Click **Estimate** to count the number of schedules and calculate the amount for all of the schedules included with your current filter settings.
            
        -   Adjust the filters as needed and click **Estimate** again.
            
8.  Click **Create Journal Entries**.
    
9.  On the Process Status page, use the link in the **Submission Status** column to view the journal entry for the submission and verify that it's correct.
    

### Related Topics

-   [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html)
-   [Filtering the Revenue Recognition Source Transaction List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1692710.html)
-   [Editing a Revenue Recognition Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1693121.html)
-   [Setting Up a Reminder for Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1693505.html)
-   [Journal Entries Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1468996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
