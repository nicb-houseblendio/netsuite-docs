---
id: "section_N1694795"
type: "section"
title: "Using Percent-Complete Revenue Recognition for Projects"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Using Percent-Complete Revenue Recognition for Projects"
parent: "chapter_N1678106"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1694795.html"
anchors: ["procedure_N1694822", "bridgehead_N1694882", "procedure_N1694894", "bridgehead_N1694960"]
sha256: "245f34db1bd91c3dccf771b622757af0c1b324f538b2b89484ff8bceffec1f32"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Advanced Revenue Management (Essentials) for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4356983516.html).

If you have a projects based business, you can recognize revenue based on the percentage of completed project work by using variable revenue recognition schedules. You can coordinate the recognition of deferred revenue with the completion of stages for your projects. This feature is available only if you use Project Management.

Set up an item to associate a variable recognition template with projects you track. Then, sales that contain the service item generate a revenue recognition schedule based on the template and the linked project completion.

As time worked is logged against the project and portions of the project are marked complete, journal entries are created to recognize the related revenue.

#### To recognize revenue based on project completion: {#procedure_N1694822}

1.  Enable the Revenue Recognition feature. See [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html).
    
2.  Create a variable type revenue recognition template. See [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html).
    
3.  Associate the variable type revenue recognition template with a service item or service items. You can do this on the item record, or on individual sales orders or invoices in the Rev Rec Schedule column. See [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html).
    
    Variable templates can be used on the same items as standard templates.
    
4.  Create an invoice or bill for the project sales order. After an invoice exists, the revenue recognition schedule is generated with forecast revenue lines.
    
5.  Create revenue recognition journal entries as needed. Running revenue recognition updates the schedule based on the changes in planned and actual time for the project.
    

For information about the variable revenue recognition schedule, see [Working with Variable Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3791187429.html).

## Additional Revenue Recognition Accounting Preferences {#bridgehead_N1694882}

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Setting Advanced Revenue Management (Essentials) Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4331941758.html).

When you use the **Use System Percentage of Completion for Schedules** preference, NetSuite automatically determines the percentage of a project that's been completed based on time logged against the project. If the Percent Complete field in the project record has a value, it's used instead of the automatic calculation. If you don't select this preference, you must enter the percent complete value on the project record.

If you use the **Adv. Billling: Use Sales Order Amount** preference, revenue is recognized based on the percent complete in relation to the sales order rather than the invoice.

For more information about these and other accounting preferences related to revenue recognition, see the [Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html#bridgehead_N1386651) section in [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

#### To set preferences for revenue recognition: {#procedure_N1694894}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  Click the **General** subtab.
    
3.  Scroll to the Revenue Recognition section, and check the preferences you want to use.
    
4.  Click **Save**.
    

## Percent-Complete Based Recognition Journal Entries {#bridgehead_N1694960}

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

The Create Revenue Recognition Journal Entries page includes revenue due to post from variable schedules based on project completion.

Important:

Always create revenue recognition journal entries in chronological order when using percent-complete revenue recognition for projects.

For the period you select, NetSuite determines the amount due to be recognized for each schedule based on project completion. It calculates project completion based on entered and approved project time entries. The Project record shows the percentage of completion for the project in that period, and NetSuite uses that percentage to determine the revenue due to post.

A variable schedule doesn't show in the list if:

-   It has a zero balance to recognize for the selected period.
    
-   Revenue recognition journal entries have been created for the period and the planned or actual time worked for the project hasn't changed since that point.
    

Revenue recognition journal entries typically debit a deferred revenue account and credit a revenue account. In some cases, however, a journal entry may decrease the revenue recognized. In these cases, the revenue recognition journal entries credit a deferred revenue account and debit a revenue account.

For example, the time estimate to complete project Alpha is 100 hours. During period One, 50 hours are logged for project Alpha. 50 hours = 50% of completion and 50% of the project revenue is recognized.

Then, during period Two, the time estimate is increased to 200 hours. The 50 hours logged against the project now equals 25% completion and the revenue recognized needs to be decreased. NetSuite generates a journal entry that credits the deferred revenue account and debits the revenue account to correct the amount of revenue recognized previously. On the Variable Revenue Recognition Schedule, the journal entry line displays a negative amount.

These schedules coordinate the recognition of deferred revenue with the stages of completion of an associated project.

As time worked is logged against the project and portions of the project are marked complete, journal entries become due to post to recognize the related revenue. For more information, see [Working with Variable Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3791187429.html).

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)
-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html)
-   [Revenue Recognition Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1695172.html)
-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
