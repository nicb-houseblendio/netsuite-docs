---
id: "section_N1475891"
type: "section"
title: "Making Intercompany Journal Entries"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries in OneWorld > Making Intercompany Journal Entries"
parent: "section_N1475513"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html"
anchors: ["procedure_N1476014", "bridgehead_N1476350"]
sha256: "37eafac4ed61b3c17a51dc7269bc2efdee00b3d50c999619ab97b27113b9b4a3"
---

Note:

As of 2018.1, advanced intercompany journal entries replace legacy intercompany journal entries in new OneWorld accounts.

Intercompany journal entries are a specialized type of journal available specifically for OneWorld. An intercompany journal entry records debits and credits to be posted to ledger accounts for transactions between two subsidiaries. Intercompany journal entries adjust the value of any set of accounts without entering transactions such as invoices or bills.

An advanced version of intercompany journal entries is now available. You can define multiple receiving subsidiaries, change the base currency to any currency set up in your system, and use the Auto Balance functionality. For information, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html).

The Automated Intercompany Management feature automatically generates intercompany elimination journal entries during the period close process. If you use this feature, the intercompany journal form includes an Eliminate box to identify lines to be eliminated. For more information, see [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html).

If you enable the Intercompany Time and Expense feature, you can create intercompany time entries and expense transactions. You can create intercompany adjustment journal entries to transfer time, expense, or both charges from one subsidiary to another. For these journals, you have the option of using the intercompany clearing account that is automatically created when this feature is enabled and their associated transactions such as journal entries. For expense charges, you can generate automated adjustments instead of creating intercompany journal entries. See [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In 2013.1, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. In 2014.1, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that aren't currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

You also have the option of importing intercompany journal entry data from a CSV file. For more information, see [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html).

For general information about making journal entries in OneWorld, see [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html). For examples, see [Example of Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476520.html). For information about automatically creating journal entries from allocation schedules, see [Creating Intercompany Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484654.html).

#### To make an intercompany journal entry: {#procedure_N1476014}

1.  Go to _Transactions > Financial > Make Intercompany Journal Entries_.
    
2.  In the Classification section, select the subsidiary initiating the ledger transaction. You must select the subsidiary before you can accept or select the currency.
    
    The first line of this journal entry must post to the selected subsidiary.
    
    Important:
    
    All lines of this journal entry must post to either the **Subsidiary** or the **To Subsidiary**. No other subsidiaries can be associated with lines on this journal entry.
    
3.  In the Primary Information section:
    
    1.  In the **Entry No.** field, accept the default or enter a different number.
        
        Note:
        
        If journal entries are assigned autogenerated numbers in your account, you can't change the default number unless the override permission is enabled for Journal. Go to _Setup >Company > Auto-Generated Numbers_ > Document Numbers subtab. Check the **Allow Override** box on the **Journal** line. For more information, see [Set Auto-Generated Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252198.html).
        
    2.  Review the **Out of Balance By** fields as you enter journal lines. They indicate whether the debits and credits in the journal entry balance.
        
    3.  In the **To Subsidiary** field, choose the second subsidiary for this ledger transaction.
        
        Note:
        
        If one or both of the subsidiaries selected in the **Subsidiary** or **To Subsidiary** field is assigned to vendor or customer records, you can make intercompany journal entries for any of these vendors or customers. To do this, on the **Lines** subtab, select the shared vendor or customer from the **Name** field. For more information about shared records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    4.  By default, the **Currency** field displays the base currency of the subsidiary selected in the **Subsidiary** field.
        
        You can change this value to the base currency of the subsidiary selected in the **To Subsidiary** field.
        
        If one of the subsidiaries uses a base currency different from the selected currency, the journal entry is translated into that subsidiary's base currency before it posts to that subsidiary's ledger. This translation is based on the exchange rate entered on the intercompany journal form.
        
    5.  The **Exchange Rate** field is the current exchange rate between the selected currency and the base currency of the other subsidiary in the transaction.
        
        You can edit the exchange rate on this form for only this transaction. To affect additional future transactions, you can also update the currency record with the entered exchange rate.
        
    6.  If you have journal approval permission, check the **Approved** box to approve your journal entry.
        
        If you don't check this box, this entry doesn't post until it's approved.
        
        Important:
        
        The **Approved** box displays only if the **Require Approvals on Journal Entries** preference is enabled. Go to _Setup > Accounting > Accounting Preferences_ > **General** subtab. See [Require Approvals on Journal Entries Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469586.html).
        
        The **Approved** box doesn't display if you've enabled the **Journal Entries** approval routing preference to use SuiteFlow to create a custom journal entry approval routing. See [Use Journal Entry Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4643680489.html).
        
    7.  In the **Date** field, accept today's date or enter a new date for the journal entry.
        
    8.  If you use fiscal periods, you see a **Posting Period** field.
        
        In the Posting Period field, select the period for the journal entry. You can't select a closed period. You can select an open and locked period only if your role includes the Override Period Restrictions permission. If the journal entry is pending approval, NetSuite keeps the selected Posting Period when you edit the journal entry and doesn't update it to match the transaction date. NetSuite may recalculate the Posting Period if the selected period is locked or closed.
        
    9.  Leave the **Reversal Date** field blank and **Defer Entry** box blank, unless you want to create a reversing entry at the same time.
        
        If you check the **Defer Entry** box, the **Reversal Date** field is required.
        
        For information about reversing entries, see [Reversing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471552.html).
        
    10.  In the **Memo** field, enter information to help you identify this journal entry in a list of other journal entries.
         
         The value in this field displays on the List page.
         
4.  If you've enabled **Departments**, **Classes**, or both on the **Company** subtab of the Enable Features page, select the appropriate classification to associate with this journal entry.
    
    For information about Departments and Classes, see [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html).
    
5.  On the **Lines** subtab, enter the detail information for the journal lines.
    
    The columns that appear are based on the permissions set for your user role.
    
    Tip:
    
    You can go down the lines by pressing the **Enter** key on your keyboard. You can't go up the lines.
    
    1.  In the **Subsidiary** field, select the subsidiary to associate with this journal line. Only the **Subsidiary** or **To Subsidiary** can be selected.
        
        The first line of this journal entry must post to the subsidiary selected in the **Subsidiary** field. Lines subsequent to the first may post to either the **Subsidiary** or **To Subsidiary**.
        
        Note:
        
        If the subsidiary you select is assigned to vendor or customer records, you can make journal entries for any of these vendors or customers. To do this, on the **Lines** subtab, select the vendor or customer from the **Name** field. For more information about shared records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    2.  In the **Account** field, select the ledger account to be affected by this journal line.
        
        If you use the **Automated Intercompany Management** feature, you can select an intercompany account. The **Eliminate** box is checked to flag the line for elimination at period end. See [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html).
        
        If you enabled the **Intercompany Time and Expense** feature, you can use the subsidiaries' intercompany clearing account for entries that transfer charges for time or expenses. See [Intercompany Clearing Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html).
        
        The list of available accounts is filtered according to any class/department/location restrictions set for your role. Accounts that are associated with classes, departments, and locations to which your role doesn't have access aren't available in the **Account** list.
        
    3.  In the **Debit** or **Credit** field as appropriate, enter the amount of the line item.
        
    4.  Optionally, enter a memo to help you recognize this entry in a register for this account.
        
    5.  Optionally, in the **Name** field, select a customer, employee, project, or vendor to associate with this entry.
        
        If you use the [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html) feature, you can create a journal entry for an entity in any of that entity's currencies.
        
        If you use **Automated Intercompany Management**, select an intercompany customer or intercompany vendor, as appropriate.
        
        Note:
        
        NetSuite filters the list of options in this field and includes only entities that support the selected base currency. If the subsidiary you select is assigned to vendor or customer records, you can make journal entries for any of these vendors or customers. To do this, on the **Lines** subtab, select the vendor or customer from the **Name** field. For more information about shared records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    6.  If you've enabled **Locations** on the **Company** subtab of the Enable Features page and you specify classifications at the line-level, select the appropriate location to associate with this line.
        
        For information about Locations, see [Locations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263024.html).
        
    7.  If you use the Revenue Recognition or Amortization features:
        
        1.  In the **Schedule** column list, select the appropriate template.
            
            Revenue recognition templates display when the **Revenue Recognition** feature is enabled. Amortization templates display when the **Amortization** feature is enabled.
            
        2.  If you select a variable template, you must also select the associated project in the **Customer** column list.
            
        3.  Enter a start and end date, if needed.
            
        4.  Enter the residual amount not to be recognized, if needed.
            
    8.  NetSuite automatically marks the intercompany journal lines as elimination if the following three conditions are true:
        
        -   The journal entry was created by an intercompany allocation schedule and the selected subsidiary was an elimination subsidiary.
            
        -   The intercompany elimination accounts used the same elimination algorithm.
            
        -   The accounts were in balance.
            
        
        You can manually unmark the lines as elimination by clearing the **Eliminate** box.
        
    9.  If required, select a tax code to default the tax rate for the line.
        
        Only tax codes with VAT and GST appear in the **Tax code** list.
        
    10.  Enter the VAT or GST tax amount for the line, if any.
         
    11.  In the **Tax Account** field, select the account for the tax.
         
    12.  Click **Add**.
         
         Tip:
         
         When line details are similar, click **Copy Previous** and then make modifications as required.
         
    13.  Repeat these steps for each line item.
         
         When you finish entering line items, the **Debit** and **Credit** out of balance fields at the top of the page should be blank. If either field contains an amount, your line items are out of balance and you can't save this entry.
         
         To post an intercompany journal entry, the total debits and credits must balance by subsidiary for every transaction. Debit and credit amounts between subsidiaries can be different. Upon saving the intercompany journal entry in this case, NetSuite alerts you that the journal entry doesn't balance between subsidiaries. To save the journal entry, click **OK**.
         
6.  On the **Communication** subtab, you can attach files and notes to this transaction.
    
    1.  On the **User Notes** subtab, enter a title and note for any comments you want to add to this transaction. Click **Add** after each note.
        
    2.  On the **Files** subtab, select and attach files from the File Cabinet related to this transaction. To upload a new file to the File Cabinet, select **New** from the list in the **Attach Files** column.
        
    3.  Use the **Events**, **Tasks**, and **Phone Calls** subtabs to add activities, such as events, phone calls, and tasks to this transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
        
7.  If the Multi-Book Accounting feature is provisioned in your account, the **Accounting Books** subtab appears. This subtab shows the secondary books, if any, and their respective base currencies and exchange rates. For information about Multi-Book Accounting, see [Using Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3831569045.html).
    
8.  Click **Save**.
    

Important:

When you create an intercompany journal entry for two subsidiaries with different base currencies, the general ledger impact may be different for each subsidiary. This is due to revaluation.

## VAT/GST for Intercompany Journal Entries {#bridgehead_N1476350}

When you create an intercompany journal entry, include VAT/GST information in the VAT and VAT Amt fields on the Lines subtab. These fields are available for subsidiaries with a tax nexus set up and a reporting requirement for VAT or GST.

### Related Topics

-   [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html)
-   [System-Generated Journals for Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1528216938.html)
-   [Elimination Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475762.html)
-   [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html)
-   [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
