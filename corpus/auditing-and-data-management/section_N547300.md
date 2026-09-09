---
id: "section_N547300"
type: "section"
title: "Duplicate Number Warnings"
branch: "auditing-and-data-management"
category: "account-administration"
breadcrumb: "Account Administration > Auditing and Data Management > Avoiding Duplicates > Duplicate Number Warnings"
parent: "chapter_4470654298"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N547300.html"
anchors: []
sha256: "8464cbb75c8043e1a3cb20fdee6d081777f4d9dcc818516b01ab815ef5ecae63"
---

Any user with the Accounting Preferences permission can set up an account so that all users are alerted or blocked from proceeding when they attempt to save transaction records with duplicate document numbers.

If you import transactions and use the Advanced Numbering feature, NetSuite checks for duplicates based on these settings. When you import a transaction, NetSuite determines which advanced numbering rule applies to it using your rules' criteria. It then checks if a transaction with the same document numbers already exists for the same rule. If a duplicate is detected, NetSuite uses your Duplicate Number Warnings preference as described below.

To enable these warnings, go to _Setup > Accounting > Preferences > Accounting Preferences_. On the Items/Transactions subtab in the Other Transaction Preferences section, select one of the following Duplicate Number Warnings from the list:

-   **No Warnings** - Users aren't warned when the transaction they are saving will create a duplicate document number.
    
    If you import transactions and use Advanced Numbering, NetSuite doesn't warn you when the imported transactions use duplicate document numbers and imports all transactions.
    
-   **Warn (UI only)** - Users receive a message when they attempt to save a transaction record with the same document number as another record of the same type. When the warning is displayed, a user can enter a different number before attempting to save again.
    
    If you import transactions and use Advanced Numbering, NetSuite doesn't warn you when the imported transactions use duplicate document numbers and imports all transactions.
    
-   **Warn and Block** - Users receive a message when attempting to save a transaction record with the same number as another record of the same type. When the warning is displayed, the user must click Cancel and change the document number in the record. This option affects the following transaction types:
    
    -   Vendor bills
        
    -   Vendor credits
        
    -   Card charges
        
    -   Card refunds
        
    -   Custom purchase transactions
        
    
    If you import transactions and use Advanced Numbering, NetSuite warns you when imported transactions create duplicate document numbers, and doesn't import these transactions.
    

Important:

When working with transactions, don't click the Submit button multiple times. If you click Submit more than one time, multiple transactions may be created.

### Related Topics

-   [Avoiding Duplicates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4470654298.html)
-   [Avoiding Duplicate Transaction Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546911.html)
-   [Using Auto-Generated Numbering for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N547392.html)
-   [Avoiding Duplicate Processing of Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4431121865.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
