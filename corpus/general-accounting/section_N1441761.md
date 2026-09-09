---
id: "section_N1441761"
type: "section"
title: "Entering Opening Balances"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Chart of Accounts Management > Entering Opening Balances"
parent: "chapter_N1439850"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1441761.html"
anchors: ["bridgehead_N1441861", "procedure_N1441878", "bridgehead_N1441957", "procedure_N1441970"]
sha256: "a843725e9a45feabf1484041f553f20edf06e4dd8f92dbe7e5b3ef769d4274f9"
---

The opening balance for each general ledger account is the amount in the account when you first start using it in NetSuite. The date of the opening balance is included on each account record. After an opening balance has been entered for an account, that account can be used in NetSuite transactions.

-   If you don't use NetSuite OneWorld:
    
    -   For accounts included in your initial NetSuite chart of accounts, you can enter opening balances for your go-live date on each account record as you create the account. See [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).
        
    -   You may want to obtain a trial balance report in debit/credit format, from your accountant or from your previous accounting management system, to use as a worksheet for entering opening balances in NetSuite.
        
    -   For accounts added later, you can enter opening balances after account records have been created in NetSuite on the Opening Balances page. For example, you created a new petty cash account. Use the Opening Balance page to enter the amount of starting cash in that account.
        
-   If you use NetSuite OneWorld, you must create and save accounts, then enter opening balances from the Opening Balances page.
    

You enter opening balances for the first time on the Opening Balances page. See [Entering Opening Balances for the First Time](#bridgehead_N1441861).

If necessary, you can go back and change opening balances later. You make changes through a transaction search. See [Changing Opening Balances](#bridgehead_N1441957).

## Entering Opening Balances for the First Time {#bridgehead_N1441861}

The Opening Balances page enables you to enter balances for multiple accounts at one time.

#### To enter opening balances for the first time: {#procedure_N1441878}

1.  Go to _Setup > Accounting > Setup Tasks > Enter Opening Balances ( Administrator )_.
    
    You can enter an opening balance for any account for the first time on this page.
    
    You can't enter an opening balance for a new summary account.
    
    Accounts that already have opening balances are not available on this page. See [Changing Opening Balances](#bridgehead_N1441957).
    
2.  Select the correct posting period.
    
3.  If you're using NetSuite OneWorld, select a subsidiary.
    
4.  If necessary, modify the date.
    
5.  For each account, enter a debit or credit according to the starting balance, then save.
    
    You can enter either a debit or a credit. If you enter a debit, the credit field disables. If you enter a credit, the debit field disables.
    

When you save the Opening Balances page, NetSuite generates journal entries to create opening balances.

NetSuite tracks the difference between the opening balances' debits and credits in the **Out of Balance By** field.

## Changing Opening Balances {#bridgehead_N1441957}

When you save an account's opening balance, NetSuite generates a journal transaction. To change the balance, you must run a transaction search to find the journal transaction and then directly edit that transaction record.

#### To find a transaction and change its opening balance: {#procedure_N1441970}

1.  Go to _Transactions > Management > Search Transactions_.
    
2.  When the Transaction Search page appears, select the following filters, and click **Submit**:
    
    -   **Account** - select the account with the opening balance you need to change
        
    -   **Transaction Type** - select Journal
        
3.  From the list of search results, locate the journal entry for that opening balance and click **Edit** next to that entry.
    
    Opening balance journals usually have text flagging them in the **Memo** field.
    
4.  On the lower portion of the Journal page, you can make changes to transaction lines as necessary. Click **Done** after each line change.
    
5.  When you have completed your edits, click **Save**.
    

After you have created accounts and entered opening balances, you can review the chart of accounts. See [Setting Up Historical Balances in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442160.html).

### Related Topics:

-   [Feature-Specific, System-Generated Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4078513386.html)
-   [Chart of Account Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440268.html)
-   [Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3947502870.html)
-   [Viewing the Chart of Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442506.html)
-   [Making Changes to Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442743.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
