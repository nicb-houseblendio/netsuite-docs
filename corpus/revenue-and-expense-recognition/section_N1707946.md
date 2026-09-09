---
id: "section_N1707946"
type: "section"
title: "Reclassifying Deferred Revenue for Revenue Commitments"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Reclassifying Deferred Revenue for Revenue Commitments"
parent: "chapter_N1701780"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707946.html"
anchors: ["procedure_N1708028"]
sha256: "26f186885b98875891ce74bdb4e8cd9b0195020769ed8fce86c365c8bf3eaee4"
---

Important:

This topic applies to the Revenue Commitments feature. If you're using Advanced Revenue Management (Essentials), see [Reclassification of Deferred Revenue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4363759368.html) and its subtopics.

Use the Create Reclassification Journal Entries process to reclassify deferred revenue for revenue commitments.

If line level deferred revenue reclassification **is enabled** for your account, reclassifying deferred revenue for revenue commitments automatically creates journal entries to:

-   **Allocate the gross billing amount to individual order lines (for multi-elements sales contracts only)**
    
    The G/L impact for the carve in/carve out adjustment to deferred revenue is:
    
    -   For carve out: Debit Deferred Revenue account
        
    -   For carve in: Credit Deferred Revenue account
        
-   **Adjust revenue for foreign currency variance, posting to item-specific accounts, if you use Multiple Currencies**
    
    The G/L impact for the foreign currency adjustment to revenue is:
    
    -   For a gain: Debit Deferred Revenue and Credit Revenue.
        
    -   For a loss: Debit Revenue and Credit Deferred Revenue.
        
-   **Reclassify revenue amounts for unbilled receivables and deferred revenue**
    
    The G/L impact for reclassifying revenue is:
    
    -   When billing < revenue recognition: Debit Unbilled Receivable and Credit Deferred Revenue.
        
    -   When billing > revenue recognition: Debit Deferred Revenue and Credit Unbilled Receivable. Reclassification isn't needed unless unbilled receivables exist from a prior period, so a journal entry may not be created.
        

If line level deferred revenue reclassification is disabled for your account, reclassifying deferred revenue for revenue commitments automatically creates journal entries to:

-   **Adjust revenue for foreign currency variance, if you use Multiple Currencies**
    
    The G/L impact for the foreign currency adjustment to revenue is:
    
    -   For a gain: Debit Deferred Revenue and Credit Revenue.
        
    -   For a loss: Debit Revenue and Credit Deferred Revenue.
        
-   **Reclassify revenue amounts for unbilled receivables and deferred revenue**
    
    The GL impact for reclassifying revenue is:
    
    -   When billing < revenue recognition: Debit Unbilled Receivable and Credit Deferred Revenue.
        
    -   When billing > revenue recognition: Debit Deferred Revenue and Credit Unbilled Receivable. Reclassification isn't needed unless unbilled receivables exist from a prior period, so a journal entry may not be created.
        

You must create deferred revenue reclassification journal entries each month to ensure accurate results in subsequent periods. To reclassify deferred revenue, run the Create Deferred Revenue Reclassification Journal Entries batch process. You should run revenue reclassification after each time you create revenue recognition journal entries. If you run these processes out of order, you can go back and run Create Revenue Recognition Journal Entries and then rerun Create Deferred Revenue Reclassification Journal Entries. The reclassification is cumulative.

All reclassification journal entries are approved by default.

#### To create deferred revenue reclassification entries: {#procedure_N1708028}

1.  Go to _Transactions > Financial > Create Reclassification Journal Entries_.
    
2.  In **Posting Period**, select the period to reclassify revenue for.
    
3.  For **Journal Entry Date**, enter the date for the journal entries.
    
4.  If you use NetSuite OneWorld, select the **Subsidiary** to associate with this journal entry.
    
    When a journal entry is associated with a subsidiary, the journal posts to that subsidiary and the schedule is restricted to be viewed only by entities associated with the subsidiary.
    
5.  Select a transaction type if you want to filter the list of transactions.
    
6.  Select a **Customer:Job**.
    
7.  In the **Select Individual Schedules** field:
    
    -   Check the **Select Individual Schedules** box to create only one journal entry for the transactions you select from the list of source transactions. If you filter the list to show particular schedules, you can check the box in the **Select** column next to each schedule you want to include in the journal entry. Clicking **Create Journal Entries** creates **one** journal entry for all schedules that you mark.
        
        If there are multiple segments or pages of transactions shown when selecting schedules, the following is true:
        
        -   If you click **Mark All** or **Unmark All**, only boxes on the current segment or page are affected.
            
        -   You must click **Create Journal Entries** to create an entry for each segment or page of schedules.
            
    -   Clear the **Select Individual Schedules** box to create one or more journal entries. You can filter the list to show particular transactions. When you click **Create Journal Entries**, you create multiple journal entries at one time for all schedules that show in the list, across all segments or pages. You don't need to submit each page individually.
        
        If you don't filter the list of schedules, a journal entry is created for every source transaction for the period selected, even if there are hundreds or more schedules.
        
    
    The page shows a list of revenue recognition journal entries due to post with the following information for each line:
    
    -   **Source Transaction** - links to the originating transaction
        
    -   **Customer** - links to the customer on the transaction
        
    -   **Has recognition change** - indicates whether the amount of revenue recognized has changed since the last time reclassification was run.
        
    -   **Has billing change** - indicates whether the amount billed has changed since the last time reclassification was run
        
    
    Revenue recognition schedules that have lines with **Is Recognized** checked for the selected **Posting Period** are included in the list if they have been billed.
    
8.  Click **Create Journal Entries**.
    

### Related Topics

-   [Using Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1701780.html)
-   [Setting Up the Revenue Commitments Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1702000.html)
-   [Revenue Commitments Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703512.html)
-   [Advanced Revenue Commitments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703735.html)
-   [Creating Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707026.html)
-   [Creating Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707738.html)
-   [Creating Revenue Commitment Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709562.html)
-   [Revenue Commitment Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710191.html)
-   [Revenue Reclassification Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1717186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
