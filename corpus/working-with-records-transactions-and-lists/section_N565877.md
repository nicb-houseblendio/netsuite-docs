---
id: "section_N565877"
type: "section"
title: "Submitting Memorized Transactions"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Memorized Transactions > Submitting Memorized Transactions"
parent: "section_N564245"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N565877.html"
anchors: ["procedure_N565898"]
sha256: "0320a61761aa3bc526f8b3b18909c0fef39b1e96880e480ef965be31d6a8c0c0"
---

After you've set up memorized transactions you can submit all transactions due to be posted at one time.

To create memorized transactions, see [Memorizing a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564637.html).

#### To submit memorized transactions: {#procedure_N565898}

1.  Go to _Transactions > Management > Enter Memorized Transactions_.
    
2.  On the Enter Memorized Transactions page, use the following filters to show transactions in the list:
    
    -   **Date**
        
        Enter or select the date you want these transactions to post.
        
        The current date defaults in this field.
        
    -   **Use Next Date**
        
        Check this box to use the date of the next scheduled occurrence of the transaction as the posting date. For transactions without a next date, the current date is used.
        
        When this box is unchecked, the current date shows in the date field and is the posting date.
        
        NetSuite remembers your preference for this box and checks or clears it the next time you use this form.
        
    -   **Has Remaining**
        
        -   Select **Yes** to show only transactions with remaining scheduled occurrences.
            
        -   Select **No** to show transactions with no remaining occurrences.
            
        -   Select **All** to show all memorized transactions.
            
    -   **Next Date**
        
        -   Select a date range to filter the list to show only transactions whose **Next Date** falls within this range.
            
        -   Select all to show all memorized transactions.
            
    -   **Action**
        
        -   Select **All** to show all memorized transactions.
            
        -   Select **None** to show no memorized transactions.
            
        -   Select **Automatic** to show memorized transactions that automatically post and don't send a reminder.
            
        -   Select **Reminder** to show memorized transactions that send a reminder for you to post them.
            
        -   Select **Template Only** to show memorized transaction templates which don't create transactions.
            
    -   **View**
        
        If you've customized list views, select a custom view in this field.
        
3.  To edit an individual transaction, click its **Edit** link.
    
4.  To process several memorized transactions at one time, check the box in the **Enter** column next to each transaction you want to process.
    
    You can also choose to click the **Enter** link next to a transaction to enter it individually.
    
5.  To change all memorized transactions from Automatic to Remind Me, or from Remind Me to Automatic at the same time, click **Switch Action**.
    
6.  Click **Submit**.
    
    A list of the new transactions shows on the Processed Transactions page.
    

Note:

There must be at least ten transactions for NetSuite to split the transactions into multiple workqueues.

To view a list of all memorized transactions, go to _Transactions > Management > Enter Memorized Transactions > List_.

Important:

When the **Allow Posting in Locked Period** option is enabled for a memorized transaction, transactions can post in locked periods even if users initiating these transactions don't have the **Override Period Restrictions** permission. Transactions can never be posted in closed periods. If the posting date for a memorized transaction is in a period that has been closed, it's posted to the next open period. For more information, see [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).

### Related Topics

-   [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html)
-   [Memorizing a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564637.html)
-   [Editing Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566256.html)
-   [Customizing the Memorized Transactions List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N564424.html)
-   [Viewing the Status of Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N564455.html)
-   [Deleting Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566525.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
