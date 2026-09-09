---
id: "section_N1543875"
type: "section"
title: "Writing Checks"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Checking > Writing Checks"
parent: "chapter_N1543613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1543875.html"
anchors: ["procedure_N1544027"]
sha256: "2b3f6b785ac6cc9aaae74c1a194355c15e1ce0f73ec9a0e0d5068ea08874607b"
---

Note:

The Write Checks option is not available for Japan Edition.

In NetSuite, use the Write Checks transaction to issue a check to pay an expense or record a non-check transaction. For example, you can:

-   reimburse employees for expenses if you do not use Direct Deposit or Accounts Payable
    
-   pay vendors if you do not use Accounts Payable
    
-   record cash transactions
    
-   enter other non-check debits, such as debit card transactions
    

If you use Accounts Payable, pay vendors at _Transactions > Payables > Pay Bills_. For more information, see [Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3694535.html).

Note:

If you need to stop payment on a check, the preferred method is to void the check in the system. When you void a check with a reversing journal entry, NetSuite records a reversing journal entry to cancel the general ledger impact of the check. If you void a check without a reversing journal entry, NetSuite sets the check amount to zero. Voiding a check doesn't remove it from the system, ensuring that you maintain the proper audit trail. For information about voiding a check, see [Voiding a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3951602420.html) and [Voiding Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html#bridgehead_4241871944).

Saving a check transaction records the expense by debiting the specified expense account and crediting the selected bank account.

When you save a check transaction, you have three options:

-   To process the information and return to the Transactions page, click **Save**.
    
    If you select **To be Printed** for the transaction, you can print it on the Print Checks page. For more information, see [Printing Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1545292.html).
    
-   To process the information and return to another blank Check page, click **Save & New**.
    
-   To save the information and immediately print the check you created, click **Save & Print**. For more information, see [Printing a Single Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1546118.html).
    

#### To write a check: {#procedure_N1544027}

1.  Go to _Transactions > Bank > Write Checks_.
    
    Note:
    
    The Write Checks option is not available for Japan Edition.
    
2.  In the Primary Information section:
    
    1.  From the **Account** list, select the bank account from which to withdraw the funds for this check.
        
        The **Balance** field is read-only.
        
    2.  Select the **Payee** for this check.
        
    3.  In the **Amount** field, enter the amount you want to write the check for.
        
        You can also leave this field blank and enter amounts from the expenses and items added for the check. **Auto Fill** displays the amount from the previous transaction for this payee.
        
        The currency and exchange rate appear in the **Currency** and **Exchange Rate fields**, if they're visible.
        
        Note:
        
        These fields only appear if the Multiple Currencies feature is enabled. If disabled, the currency and exchange rate match the base currency and exchange rate of the associated subsidiary or company.
        
        If the payee is an employee, these fields are populated based on the base currency of the associated subsidiary or company. You need to use this currency for transactions with this employee.
        
        If the payee is a vendor or customer, these fields are populated based on the primary currency on the payee's record. To add multiple currencies for the vendor or customer, see [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html).
        
        Note:
        
        The Multiple Currencies feature includes what used to be separate Multi-Currency Customers and Multi-Currency Vendors features.If those features are still in your account, you need to enable them along with Multiple Currencies. Otherwise, customer and vendor records can only contain one currency. For more information, see [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html).
        
    4.  Use today's date or enter a new one for this transaction.
        
    5.  If you use accounting periods, pick a posting period for this check.
        
    6.  Select **To Be Printed** to save this check in your print queue to print later.
        
        If you don't check this box, you can click **Save & Print** to print this check immediately.
        
    7.  The **Check #** field is populated with one of the following:
        
        -   If you checked **To Be Printed**, this box is populated with **To Print.**
            
            You choose starting numbers when you print those checks.
            
        -   If you print this check right away when you save, NetSuite increases the largest check number by one. You can enter another number, but the next number reverts to the standard pattern.
            
        
        Note:
        
        You can also use this field to record ACH, ATM, or other reference numbers or text.
        
    8.  Enter a memo for the check (optional).
        
3.  In the Classification section:
    
    1.  If you use NetSuite OneWorld, the **Subsidiary** field displays the primary subsidiary for the **Payee** by default.
        
        Note:
        
        If you share vendor and customer records with multiple subsidiaries, you can change the subsidiary from the primary to a secondary one. When you change the subsidiary, NetSuite updates the bank account to that of the selected subsidiary and updates the currency to that of the new bank. NetSuite also clears the lines on the **Expenses** and **Items** subtabs. For more information about shared vendor and customer records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    2.  If you use departments or classes, select one to associate with this check.
        
4.  On the **Expenses & Items** subtab, click the **Expenses** subtab and select any expenses for this transaction. For more information, see [Adding Expenses to a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1544419.html).
    
5.  On the **Expenses & Items** subtab, click the **Items** subtab and select any items for this transaction. For more information, see [Adding Items to a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1544711.html).
    
6.  If you use the Landed Cost feature, on the **Landed Cost** subtab, select the allocation method, enter shipping and duty costs, and select their sources. For more information, see [Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2416930.html).
    
7.  On the **Payee Address** subtab, the address from the payee record displays. If **Auto Fill** is enabled, the address from the latest transaction displays. If you haven't sent invoices or **Auto Fill** is disabled, the **Default Billing** address appears.
    
    Note:
    
    The **Auto Fill** preference takes precedence over the **Default Billing** address.
    
    To enable or disable the **Auto Fill** preference, go to _Home > Set Preferences_. On the Transactions subtab, in the Basics section, check or clear the **Auto Fill Transactions** box.
    
    To enable or disable the **Default Billing** box, go to _Lists > Relationships > Customers_ and click **Edit** next to a customer. On the customer record, in the **Address** subtab, check or clear the **Default Billing** box next to an address.
    
8.  On the **Relationships** subtab, the primary contact for the customer automatically appears. You can edit, add, or delete contact information for this transaction.
    
9.  On the **Communication** subtab, attach files and notes to this transaction.
    
    1.  On the **User Notes** subtab, enter a title and note for any comments you want to add, and then **Add** after each note
        
    2.  On the **Files** subtab, select and attach files from the File Cabinet. To upload a new file, select **New** from the dropdown list in the **Attach Files** column.
        
    3.  Use the **Events**, **Tasks**, and **Phone Calls** subtabs to add to attach activities like events, phone calls, and tasks to this transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
        
10.  If you use NetSuite OneWorld and have Multi-Book Accounting, the **Accounting Books** subtab appears. This subtab lists any secondary books for the selected check, if any, and their base currencies and exchange rates. For information about Multi-Book Accounting, see [Using Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3831569045.html).
     
11.  If you use the International Tax Reports SuiteApp, on the **Tax Reporting** subtab, select the delivery terms, region of origin, nature of transaction code, and mode of transport. Check the **Non-deductible Tax Adjusted** box if this check includes a nondeductible tax. For more information, see [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html).
     
12.  Click **Save**.
     

#### To edit a saved check in the Checks list:

1.  Go to _Transactions > Bank > Write Checks > List_.
    
2.  From the Checks list, click **Edit** next to the check you want to modify.
    
3.  On the Check page, modify the saved check as required.
    
4.  Click **Save**.
    
    If you change the check amount, a prompt appears to unreconcile the transaction. Click **OK**, open the correct statement period, and reconcile the transaction again.
    
    Note:
    
    If you change the account for the transaction, no unreconcile prompt appears and the transaction remains reconciled.
    

#### To delete an existing check from the Checks list:

1.  Go to _Transactions > Bank > Write Checks > List_.
    
2.  From the Checks list, click **Edit** next to the check you want to delete.
    
3.  To remove the check, under **Actions**, click **Delete**.
    
4.  In the confirmation prompt, click **OK**.
    

### Related Topics

-   [Checking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1543613.html)
-   [Resetting Check Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1545131.html)
-   [Printing Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1545292.html)
-   [Entering Non-Check Debits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1547301.html)
-   [Recording Cash Transactions Using Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1547571.html)
-   [Tracking Petty Cash](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1547782.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
