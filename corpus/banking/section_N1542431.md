---
id: "section_N1542431"
type: "section"
title: "Making Deposits"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Deposits > Making Deposits"
parent: "chapter_N1542225"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1542431.html"
anchors: ["procedure_N1542508"]
sha256: "562563a973f17a9cbb1b0d58eb829f699712580846e0d68b3d2348c31a48a03b"
---

Make a deposit in NetSuite to record funds you add to your bank account. For a deposit, select payments for existing transactions, add funds not related to transaction payments, and record any cash you get back from the bank.

Note:

Many organizations post customer payments to the Undeposited Funds account instead of a specific bank account. This prevents a time lag between your book balance and your bank balance. When you record a deposit, NetSuite moves funds from Undeposited Funds to the bank account ledger to keep your bank balances accurate. If you record customer payments directly to a bank account instead of Undeposited Funds, you don't need to create deposits for those amounts.

Warning:

If another user deletes a payment or cash sale marked for deposit while you're creating a deposit, NetSuite displays a message that the record has changed. You can't save the deposit because the data is missing.

When making a deposit, besides the standard save options, you can also do the following from the header:

-   **Reset** - clears all input on all subtabs and in the header
    
-   On the **Payments** subtab, check or clear the box below **Customize**. Checking the box selects all payment items for the deposit. Clearing the box removes them from the deposit.
    

Add items to a deposit with payment methods other than Check or Cash. For example, add a custom payment method or a credit card. If you select **Print** on the deposit form, NetSuite warns you that the deposit has items other than Check or Cash. Continue with the deposit if this is correct, or make changes as needed.

The system doesn't track tax periods on deposits.

If you use a custom role without the permission to make deposits, add the Deposit permission to the role.

#### To add the Deposit permission:

To record a customer deposit, follow the same steps but select the Customer Deposit permission. To record a customer deposit, see [Recording a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296669.html).

1.  Log in as an administrator.
    
2.  Go to _Setup > Users/Roles > Manage Roles_.
    
3.  On the Manage Roles page, click **Edit** next to the custom role you want to modify.
    
4.  On the **Permissions** subtab of the Role page, find the Transactions sublist.
    
5.  From the dropdown list in the Permission column, select **Deposit**.
    
6.  From the dropdown list in the Level column, select the access level for the permission.
    
7.  Click **OK**.
    
8.  Click **Save**.
    

#### To make a deposit: {#procedure_N1542508}

1.  Go to _Transactions > Bank > Make Deposits_.
    
2.  In the Primary Information section:
    
    1.  Select the custom form for the deposit.
        
        The system-generated deposit number appears.
        
    2.  Select the bank account for the deposit.
        
        The currency and exchange rate display for the account. For information about exchange rates, see [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html).
        
        If the bank account's currency matches the subsidiary's base currency, the **Exchange Rate** field is read-only.
        
        Note:
        
        If you use NetSuite OneWorld, the bank account determines the subsidiary and the selectable payments at the line level in step 4a. For other deposits, the bank account determines the subsidiary and the currency. If you change the bank account, class, department, location, and all line items are cleared.
        
    3.  The **Amount** field displays the total amount of payments, other deposits, and cash back selected or entered on the **Deposits** subtab.
        
    4.  Accept today's date or enter the date of the deposit.
        
    5.  Select a posting period if you use the **Accounting Periods** feature.
        
    6.  Enter a memo if needed.
        
    7.  To enter multiple deposits before printing deposit slips, check the **To Be Printed** box. For more information, see [Printing Multiple Deposit Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1543179.html#bridgehead_N1543222).
        
3.  In the Classification section, select a department, class, and location for the deposit if needed.
    
    If you use NetSuite OneWorld, the subsidiary defaults to the one linked to the selected bank account.
    
4.  On the **Deposits** subtab, enter the items for the deposit.
    
    1.  The **Payments** subtab lists all payments posted to the **Undeposited Funds** account. Check the box next to each item to include it in this deposit.
        
        Filter the items by date, date range, or payment processing profile.
        
        The **Amount** column displays the payment amount in the bank account currency, entered when received for a cash sale, invoice, or other transaction. To change the amount, click the link in the **Date** column to open the source transaction.
        
        If the field is empty, enter the amount manually. NetSuite leaves the field blank if the payment currency and bank account currency differ, and the bank and subsidiary currencies are also different.
        
        If the payment currency is different from the bank's, but the bank and subsidiary currencies match, NetSuite uses the stored exchange rate to calculate the amount.
        
        Note:
        
        You can't modify a zero payment amount.
        
        Warning:
        
        If you move a cleared cash sale transaction to **Undeposited Funds**, NetSuite returns it to an uncleared status.
        
    2.  On the **Other Deposits** subtab, enter items not received as payments to **Undeposited** Funds.
        
        Enter the name, amount (positive), account, payment method, and payment number for each item. Optionally enter a classification and memo. Click **Add**.
        
        Note:
        
        You can select an entity in the **Name** field. The available entities are filtered by the selected bank account.
        
        If you use NetSuite OneWorld with shared records, this field displays all vendors and customers assigned to the subsidiary for the selected bank account. For more information about shared records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    3.  On the **Cash Back** subtab, enter the cash back amount, account, classification, and memo. Click **Add**.
        
5.  On the **Communication** subtab, attach files and notes to this transaction if needed.
    
    1.  On the **User Notes** subtab, enter a title and note for any comments. Click **Add** after each note
        
    2.  On the **Files** subtab, attach files from the File Cabinet. To upload a new file, select **New** from the dropdown list in the **Attach Files** column.
        
    3.  Use the **Events**, **Tasks**, and **Phone Calls** subtabs to attach activities like events, phone calls, and tasks to the transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
        
6.  If you use NetSuite OneWorld and have Multi-Book Accounting, the **Accounting Books** subtab appears. This subtab displays secondary books for the deposit and their base currencies and exchange rates. For information about Multi-Book Accounting, see [Using Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3831569045.html).
    
7.  After you enter all the items for the deposit, verify the total is correct and click **Save**.
    

#### To edit a saved deposit in the Deposits list:

1.  Go to _Transactions > Bank > Make Deposits > List_.
    
2.  From the Deposits list, click **Edit** next to the deposit you want to modify.
    
3.  On the Deposit page, make the needed changes.
    
4.  Click **Save**.
    
    If you change the deposit amount, a prompt to unreconcile the transaction appears. Click **OK**, and then open the correct statement period and reconcile the transaction again.
    
    Note:
    
    If you change the account, no prompt appears and the transaction stays reconciled.
    

#### To delete an existing deposit from the Deposits list:

1.  Go to _Transactions > Bank > Make Deposits > List_.
    
2.  From the Deposits list, click **Edit** next to the deposit you want to delete.
    
3.  On the Deposit page, under **Actions**, click **Delete**.
    
4.  At the prompt, click **OK** to confirm.
    

### Additional Information

-   [Removing Undeposited Funds Lines from Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1543026.html)
-   [Handling Returned/NSF Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295030.html)

### Related Topics

-   [Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1542225.html)
-   [Viewing the Deposits List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1542818.html)
-   [Printing Deposit Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1543179.html)
-   [Recording Cash Back from a Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1543413.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
