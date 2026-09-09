---
id: "section_N557197"
type: "section"
title: "Tracking Financial Account Changes"
branch: "auditing-and-data-management"
category: "account-administration"
breadcrumb: "Account Administration > Auditing and Data Management > Managing Transactions > Reviewing Transaction History > Tracking Financial Account Changes"
parent: "section_N554247"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557197.html"
anchors: ["procedure_N557209"]
sha256: "d690702b3955b26e1609a5aa24591a92bf99275829eca9a892145a721f5dc701"
---

You can use the audit trail function to search for changes made to your financial accounts.

#### To use the Audit Trail: {#procedure_N557209}

1.  Go to _Transactions > Management > View Audit Trail ( Administrator )_.
    
2.  Select criteria to quickly find the information you need.
    
    For example, you can filter by user who performed the action, date range, or affected account. You can select more than one user, action, transaction type, account, or name by pressing the Ctrl key and selecting with your mouse.
    
3.  Click **Submit**.
    

The Audit Results page shows 8 columns with the following information:

-   **Date/Time** - This is the date and time your data was saved.
    
    All times are in Pacific Standard Time (PST). When Daylight Savings Time is in effect, all times are expressed in Pacific Daylight Time (PDT).
    
    If you import data or load sample data, all the dates and times of existing transactions appear as the date and time your data was loaded.
    
-   **Username** - This is the name of the person who created, changed, or deleted the transaction.
    
    If your company memorizes transactions, the name of the user who created these transactions appears.
    
-   **Action** - This is what was done to the transaction. This can be CREATE, CHANGE, or DELETE.
    
    If you void a transaction, CHANGE appears.
    
-   **Type** - This is the type of transaction that was created, changed, or deleted.
    
-   **Number** - This is the number specific to each transaction. For example, invoice number 18 or check number 1400.
    
-   **Post Date** - This is the date your transaction was posted to the account.
    
-   **Account** - This is the financial account that is affected by the transaction. For example, if you create an invoice, Accounts Receivable appears in the Account column.
    
    If no account was affected, the corresponding field in this column is blank.
    
-   **Amount** - This is the total amount of the transaction.
    
    Deleted and voided transactions have zero in this column. Zero also appears in this column next to changed transactions if you made a change that didn't affect the original amount.
    

Click any date in the **Date/Time** column to view the details of a transaction. When the Audit Results page appears with the particular transaction you selected, click **View** to see the details or **Edit** to make changes, and then click **Save**.

### Related Topics

-   [Reviewing Transaction History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N554247.html)
-   [Transaction System Information and Communication Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N554714.html)
-   [Granting User Access to Transaction History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555081.html)
-   [Viewing Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555355.html)
-   [Using the Transaction Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556825.html)
-   [Line-Level Audit Trail for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557476.html)
-   [Transaction Line-Level History Window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557750.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
