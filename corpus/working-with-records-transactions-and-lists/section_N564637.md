---
id: "section_N564637"
type: "section"
title: "Memorizing a Transaction"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Memorized Transactions > Memorizing a Transaction"
parent: "section_N564245"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564637.html"
anchors: ["procedure_N564658", "bridgehead_N565640"]
sha256: "637cf66a5d744061d570d48ed50f8d14011951df221686e85e702c522fb556e4"
---

For a list of the types of transactions you can memorize, see [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html).

When you create a memorized transaction, you can view this action in the system notes of the memorized transaction.

-   [To memorize a transaction:](#procedure_N564658)
    
-   [Automatic Memorized Transactions](#bridgehead_N565640)
    

#### To memorize a transaction: {#procedure_N564658}

1.  Edit the transaction you want to memorize, and make sure the appropriate information is filled in.
    
    -   Posting transactions that contain serial or lot numbers can't be memorized. This includes creating invoices, entering cash sales, and fulfilling sales orders.
        
    -   Non-posting transactions with serialized or lot items can be memorized, if the serial or lot numbers aren't entered on the transaction. This includes preparing estimates and entering sales orders.
        
        Memorized non-posting transactions with serialized items require serial numbers to be entered at item receipt or fulfillment time. For example, you create a sales order that includes a serialized item but don't enter the serial number for that item. Later, when you fulfill that sales order, you'll be required to enter the serial number for the serialized item.
        
    -   If you select to email or fax your customer, your customer automatically receives an email or fax each time the memorized transaction occurs.
        
    -   If you enter credit card payment information, this credit card is automatically charged each time the memorized transaction occurs.
        
2.  From the **Actions** list, select **Memorize**.
    
    When the Memorized Transaction page opens, the payee, vendor, customer, or project name you selected when entering your memorized transaction appears in the **Name** field.
    
3.  If you want to change the name of the memorized transaction, enter a new **Name**.
    
    The name you enter appears in the list of memorized transactions but doesn't affect the name you entered on the original transaction.
    
4.  Choose one of three options in the **Action** dropdown list in the Primary Information section:
    
    -   Choose **Template Only** if you want to create a memorized transaction that will be used as a template, but won't create any transactions.
        
    -   Choose **Reminder** if you want to be reminded when this transaction is due so that you can view and edit it before you save it.
        
    -   Choose **Automatic** if you want this transaction to automatically post. For information about this option, see [Automatic Memorized Transactions](#bridgehead_N565640).
        
5.  Check the following optional boxes as needed:
    
    1.  Check the **Inactive** box to prevent the memorized transaction from creating any more transactions.
        
    2.  Check the **Override Transaction Date** box if you don't want the transaction to post on the creation date. Then you must do the following:
        
        -   In the **Next Date** field in the **Recurring** subtab, enter the next date you want the transaction to be generated.
            
            If you want this transaction to automatically occur, you must enter a next date here. If you don't enter a next date, the transaction won't automatically post.
            
        -   In the **Next Transaction Date** field beside Next Date, enter the date you want the transaction to post.
            
            For example, today's date is 7/15. You want the first transaction to be generated on 7/16 and to post on 7/20. Check the **Override Transaction Date** box and enter 7/16 in the **Next Date** field and 7/20 in the **Next Transaction Date** field beside **Next Date**.
            
    3.  Check the **Allow Posting in Locked Period** box to enable the transaction to post to an accounting period for which transactions are locked. You must have the **Override Period Restrictions** permission to check this box.
        
        When this box is checked, memorized transactions can post in locked periods even if the user who initiates the transaction doesn't have the **Override Period Restrictions** permission. Transactions can never be posted in closed periods. If the posting date for a memorized transaction is in a period that has been closed, it's posted to the next open period. For more information, see [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).
        
    4.  Check the **Update Addresses** box to have the memorized transaction use the customer email, fax, and address information that is current as of the date the transaction is created. This option applies only to addresses on the customer record. Any other addresses, such as those included in the To Be Emailed list, must be updated manually.
        
    5.  Check the **Update Prices** box to have the memorized transaction use sales pricing that is current as of the date the transaction is created.
        
6.  To set the frequency of the memorized transaction, choose one of the following options:
    
    Note:
    
    You can't set a frequency if you selected **Template Only** in the Action list in the Primary Information section.
    
    1.  To create recurring transactions based on the number of occurrences within a time period, enter the following in the **Recurring** subtab:
        
        -   Select the **Next Date** on which the memorized transaction will create a new transaction.
            
        -   Select the number of times in a time period a transaction will be created in the **Repeat Every** field.
            
        -   Select the **Time Period** over which transactions will be created.
            
        -   Enter the total number of transactions which should be created in the Number Remaining field. If you don't want to set a limit on the number of transactions created, clear the field and check the **Indefinite** box.
            
        -   If you checked the **Override Transaction Date** box in the **Primary Information** subtab, enter the **Next Transaction Date** on which you want the transaction to post.
            
    2.  To create transactions on specific dates, enter the **Next Date** to generate a transaction in the Custom Dates subtab and click **Add**. If you checked the **Override Transaction Date** box in the **Primary Information** subtab, enter the **Next Transaction Date** on which you want the transaction to post.
        
    
    The frequency determines how often you receive the reminder if you choose **Remind Me**. If you choose **Automatic**, it determines how often the transaction occurs.
    
    Note:
    
    If **Monthly** is selected, and the **Next Date** selected is the last day of a month, NetSuite will schedule all following transactions for this memorized transaction for the last day of each month. For example, if you select a Monthly frequency and set the Next Date as 2/28/2019, subsequent transactions will occur on 3/31/2019 and 4/30/2019.
    
    If you want your transactions to occur on the 28th, 29th, 30th, or 31st of every month, set up a custom frequency in the Custom Dates subtab.
    
7.  When you've finished, click **Save**.
    
8.  If you clicked **Automatic** for this memorized transaction, you'll be prompted to continue.
    
9.  Click **OK**. Your memorized transaction is saved.
    

After you create a memorized transaction, you can review it in the following ways:

-   Go to _Transactions > Management > Enter Memorized Transactions > List_. Select it from the list.
    
-   Go to _Transactions > Management > Enter Memorized Transactions_. Click **View** or **Edit** next to the transaction.
    
-   Go to your NetSuite Home page and click the reminder you set up.
    
    Clicking the reminder takes you to a list showing memorized transactions that are currently due. To see all your memorized transactions, check the **Show All** box and click **Refresh**.
    

To view a list of memorized transactions due to be entered, go to _Transactions > Management > Enter Memorized Transactions_.

## Automatic Memorized Transactions {#bridgehead_N565640}

If an error occurs when automatically executing a transaction, NetSuite generates an alert message and changes the memorized transaction from **Automatic** to **Remind Me**. In this case, the transaction will no longer be automatically generated. You must determine the cause of the error, then update the transaction to correct the problem. After you update the memorized transaction, you can again select the Automatic option on the memorized transaction. The memorized transaction will run automatically on the next scheduled date.

For example, an account used in a memorized journal entry has become inactive. You receive an alert that the transaction can't be run. Update the journal entry with an active account number. Then select the Automatic radio button on the memorized transaction to reset the journal entry to run as scheduled.

### Related Topics

-   [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html)
-   [Submitting Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N565877.html)
-   [Editing Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566256.html)
-   [Customizing the Memorized Transactions List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N564424.html)
-   [Viewing the Status of Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N564455.html)
-   [Deleting Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566525.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
