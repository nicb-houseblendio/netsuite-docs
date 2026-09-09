---
id: "section_N1779279"
type: "section"
title: "Generating Amortization Journal Entries"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Journal Entries > Generating Amortization Journal Entries"
parent: "section_N1777836"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1779279.html"
anchors: ["procedure_N1779306"]
sha256: "1b10e6646f340036029fb3f1d16a2f93f86548c215a9a53ddac6ae71741354d3"
---

After expense and item amounts from bills and bill credits have posted to deferred expense accounts, these amounts need to be recognized and moved to expense accounts at appropriate intervals.

Amortization schedules provide a basis for the generation of journal entries to post this impact to the general ledger. You can use the Create Amortization Journal Entries page to create journal entries that post deferred expenses. This page lists amounts from all schedules that are due to post. Amortization journal entries for vendor bills typically debit expense accounts and credit deferred expense accounts.

Note:

User event scripts run when creating amortization journal entries only if Approval Routing for journal entries is enabled. If Approval Routing for journal entries is disabled, user event scripts aren't triggered. For more information about Approval Routing, [Use Journal Entry Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4643680489.html). For more information about user event scripts, see [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html).

#### To recognize a deferred expense: {#procedure_N1779306}

1.  Go to _Transactions > Financial > Create Amortization Journal Entries_.
    
    You can also get to this page directly from your dashboard. This navigation is available when you set up the Amortization Entries Pending reminder. See [Setting Up a Reminder for Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780492.html).
    
2.  Select a posting period to display the schedules with unposted amortization journal entries for that period.
    
3.  In the **Journal Entry Date** field, set the transaction date of amortization journal entries you're creating.
    
    You can set the default date that shows in this field by setting a preference at _Setup > Accounting > Accounting Preferences_. Select a date in the **Default Revenue Recognition Journal Date to** field.
    
4.  If your role has permission to enter journal entries that are approved, check the **Approve Journal** box to approve the journal entry when you save it. Clear this box to submit this journal entry for approval after it's entered.
    
5.  Select values for the following required filters if they appear in your account:
    
    -   **Subsidiary** - This required filter appears only on NetSuite OneWorld implementations.
        
    -   **Accounting Book** - This required filter appears only when the Multi-Book Accounting feature is enabled.
        
6.  Use the other filters at the top of the page to limit the list of amortization schedules displayed for this period. The filters you select become your default for this page.
    
    -   **Transaction Type** - The type of source transaction.
        
    -   **Name** - Name of the entity associated with the schedule.
        
    -   **Type** - The type of amortization schedule.
        
    -   **Item Type** - The type of item.
        
    -   **Original Account** - On this page, the original account is the same as the deferral account.
        
    -   **Target Account** - The expense account used to record amortized expenses over time.
        
    -   **Deferral Account** - The Deferred Expense type account used to post the prepaid expense or the initial cost of an asset to be depreciated.
        
    -   **Transaction Date**, **From** and **To** - When you select a date range in the **Transaction Date** field, the **From** and **To** fields are automatically populated. If you enter or select dates directly in the **From** and **To** fields, the **Transaction Date** field displays **(Custom)**.
        
7.  In the **Select Individual Schedules** field:
    
    -   Check the **Select Individual Schedules** box to create only one journal entry. After you've filtered the list to show specific schedules, you can check the box in the **Select** column next to each schedule you want to include in the journal entry. When you click **Create Journal Entries**, you create **one** journal entry for all schedules that you marked.
        
        If there are multiple segment or pages of schedules, when selecting schedules the following is true:
        
        -   If you click **Mark All** or **Unmark All**, only boxes on the current segment or page are affected.
            
        -   You must click **Create Journal Entries** to create an entry for each segment or page of schedules.
            
    -   Clear the **Select Individual Schedules** box to create one or more journal entries. The number of amortization schedules and expense amortization plans previewed is limited to 100. After you've filtered the list to show particular schedules, when you click **Create Journal Entries**, you create multiple journal entries for all schedules that show in the list including all segments or pages of the list. You don't have to submit each page individually.
        
        -   When you clear the box, the **Estimate** button appears. Clicking **Estimate** calculates the number of expense amortization sources and the amortized amount based on your current filter settings. You can adjust the filters as needed and click **Estimate** again.
            
            Note:
            
            If the Revenue and Expense Amortization feature is disabled, clicking **Estimate** shows the total number of amortization schedules rather than the total number of amortization sources.
            
        -   If you don't filter the list of schedules, a journal entry is created for every schedule for the period selected, even if there are hundreds of schedules, or more. The maximum number of entries for schedules that can be created at one time 10,000.
            
8.  Click **Create Journal Entries**.
    
9.  On the Create Journal Entries Status page, do the following:
    
    1.  Click **Refresh** to update the status.
        
    2.  When **Percent Complete** is 100.0%, in the **Status** column, click **Complete**.
        
    3.  On the Processed Schedules page, in the **Journal** column, click the links to view individual journals.
        

### Related Topics

-   [Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777836.html)
-   [Editing an Amortization Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780127.html)
-   [Approving an Amortization Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780313.html)
-   [Setting Up a Reminder for Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780492.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
