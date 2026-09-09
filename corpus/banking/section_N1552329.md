---
id: "section_N1552329"
type: "section"
title: "Reconciling Bank Statements"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Bank Account Reconciliation and Reporting > Reconciling Bank Statements"
parent: "chapter_N1552053"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1552329.html"
anchors: ["procedure_N1553099", "procedure_N1553154", "procedure_N1553214", "procedure_N1553273", "procedure_N1553343"]
sha256: "9aa5b35644faab1a503aac00673612aa0026317d1773d03eab086fea8a7d849c"
---

Note:

This is the original reconciliation feature, which is no longer supported as of NetSuite 2021.1. A redesigned version of bank data matching and statement reconciliation is available, which enables you to match and reconcile account transactions without requiring Microsoft Excel or third-party tools. For details, see [Bank Data Matching and Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4842302228.html).

If you have accounts that still use the original reconciliation feature, you can edit your accounts to use the redesigned feature. See [Editing Accounts to Use the Match Bank Data and Reconcile Account Statement Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_20260810001.html).

Reconcile your bank statement against your bank account register to keep your NetSuite account accurate.

If the items have cleared the bank, but do not yet appear on a statement, you can manually mark transactions as cleared in the check register. Go to _Reports > Financial > Chart of Accounts_. Click the name of the account. Check the box in the Clr column if a transaction is cleared, but not yet reconciled. A manually cleared transaction is not associated with a statement date and does not appear on a Bank Reconciliation Report. The account register shows if a cleared transaction is reconciled and identifies the reconciliation date. Transactions that require reconciliation have a Reconcile link in the Reconcile column.

Note:

If the Clr column contains YES or NO instead of a check box, the account is using the redesigned version of transaction matching and statement reconciliation. To clear transactions, you must go to the Match Bank Data page. For details, see [Bank Data Matching and Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4842302228.html) and [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html).

Checks written in a previous month that are not cleared display on the Reconcile Bank Statement page on the Deposits and Credits subtab. Until these checks are cleared they do not appear on a Bank Reconciliation Report.

For information about reconciling transactions that were previously reconciled and subsequently canceled, see [Troubleshooting Reconciliation History Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1554407.html).

If you void a check, reconcile the voiding journal entry. For details on voiding checks, see [Voiding a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3951602420.html).

If you change the amount of a previously reconciled transaction, the transaction becomes unreconciled again. Open the correct statement period for the transaction and reconcile the transaction again.

Note:

If you change the account of the transaction, the transaction does not become unreconciled.

Transfers to and from bank accounts appear on your bank statement as other transactions and are reconciled in the same method. Enter deposits and credits, and checks and payments as required.

When you reconcile a bank account, all reconciled transactions are automatically marked cleared. To close a period, not all transactions have to be reconciled.

Tip:

You can remove the cleared status from a transaction through the register for the bank account. Click Actions, then click Go To Register. On the account register, locate the transaction and clear the Clr box.

If the Clr column contains YES or NO instead of a check box, the account is using the redesigned version of transaction matching and statement reconciliation. To clear transactions, you must go to the Match Bank Data page. For details, see [Bank Data Matching and Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4842302228.html) and [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html).

Note:

International users may be required to use alternative methods for reconciling bank statements. For example, you might be required to make adjustments to accommodate special taxes on new transactions such as the Goods and Services Tax (GST) in Australia. For more information, see [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html).

You can begin an account reconciliation and then resume at a later time. NetSuite preserves the reconciliation until you return to save it or save and print it. For more information, see [Completing a Reconciliation at a Later Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1553886.html).

For permissions to reconcile bank statements, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

To reconcile custom transactions, go to Accounting Preferences and then check the **Show All Transaction Types In Reconciliation** box. See [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

#### To reconcile your bank statement: {#procedure_N1553099}

1.  Go to _Transactions > Bank > Reconcile Bank Statement_.
    
2.  In the **Account** field, select the bank account you are reconciling.
    
    If your account does not appear, on your account record, you need to clear the **Use Match Bank Data and Reconcile Account Statement Pages** box (see [Editing an Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4641794885.html)). As of NetSuite 2021.1, this box is automatically checked for newly-created accounts.
    
    Warning:
    
    The Reconcile Bank Statement and Reconcile Credit Card Statement pages are no longer supported and will be removed in the future. For information about the redesigned reconciliation feature, see [Bank Data Matching and Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4842302228.html).
    
    The selected bank account determines the default subsidiary and currency. This filters the open transactions at the line level.
    
    Note:
    
    If you enter transactions and then change bank accounts, NetSuite changes the currency and subsidiary and clears all line item transactions.
    
    The **Last Reconciled Balance** field provides the balance of this account from the last time you reconciled your bank statement.
    
3.  In the **Statement Date** field, enter or pick the date of the statement.
    
4.  In the **Start Date** field, enter the beginning of the reconciliation period. Unreconciled transactions before this date do not display on the subtabs.
    
5.  In the **Ending Statement Balance** field, enter the closing balance on the statement.
    
    The **Reconciled This Statement** and **Difference** fields update as you check the reconcile box next to transactions.
    
    The **Difference** field displays the amount that you must reconcile; when the difference is zero, reconciliation is complete.
    
    NetSuite calculates the **Difference** field amount by subtracting the combined amounts of the **Last Reconciled Balance** and **Reconciled This Statement** from the **Ending Statement Balance**.
    
    Tip:
    
    You can specify the number of items that display on the page at _Home > Set Preferences_ > General > Number of Rows in List Segments.
    

#### Deposits and Credits {#procedure_N1553154}

1.  Click the **Deposits and Credits** subtab.
    
    This subtab shows deposits and credits to be reconciled.
    
    A **Yes** shows in the **Cleared** column for all transactions that have been marked as cleared through the bank on the account register.
    
    If you use NetSuite OneWorld, note that only transactions for the subsidiary associated with the bank account are listed.
    
2.  Check the boxes next to the transactions you want to reconcile.
    
    As you check transactions, the **Reconciled This Statement** field is updated, and the total of those transactions shows on the **Deposits and Credits** subtab.
    
    -   To reconcile all deposits and credits, click **Mark All**.
        
    -   If you mark bank transactions as **Cleared** on an ongoing basis, when you open a reconciliation you can click **Mark All Cleared to Reconcile**, which updates all transactions already cleared to be marked for reconciliation. Then, each transaction does not need to be marked individually.
        
    
    Note:
    
    Click the **Date** or **Tran No.** links to view the original transaction. Click the **Payor** link to view the entity record.
    

#### Checks and Payments {#procedure_N1553214}

1.  Click the **Checks and Payments** subtab.
    
    This subtab shows checks and payments that need to be reconciled. Credit card refund transactions also show on this subtab.
    
    A **Yes** shows in the **Cleared** column for all transactions that have been marked as cleared through the bank on the account register. Transactions must be both cleared and reconciled to close out a period.
    
    If you use NetSuite OneWorld, note that only transactions for the subsidiary associated with the bank account are listed.
    
2.  Check the boxes next to the transactions you want to reconcile.
    
    As you check transactions, the **Reconciled This Statement** field is updated, and the total of those transactions shows on the subtab.
    
    -   To reconcile all checks and payments, click **Mark All**.
        
    -   If you mark bank transactions as **Cleared** on an ongoing basis, when you open a reconciliation you can click **Mark All Cleared to Reconcile** , which updates all transactions that are already cleared to be marked for reconciliation. Then, each transaction does not need to be marked individually
        
    
    Note:
    
    Click the **Date** or **Check No.** links to view the original transaction. Click the **Payee** link to view the entity record.
    

#### New Charges {#procedure_N1553273}

1.  Click the **New Charges** subtab.
    
2.  Fill in the appropriate information for a reconciled charge, and then click **Add**.
    
    You can enter a charge with a date after the statement date for the reconciliation, and the charge remains reconciled with this statement.
    
    If you use NetSuite OneWorld, note the following:
    
    -   **Payee** (vendor or other entity) must be associated with the same subsidiary as the bank account.
        
        Note:
        
        If you have shared vendors and customers with multiple subsidiaries and this subsidiary is a secondary subsidiary to one or more shared entities, the **Payee** field lists all of the entities to which this subsidiary is assigned. Selecting a shared entity payee enables you to enter line items for all of the entity's open transactions as well as the open transactions belonging to this subsidiary. For more information about shared records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    -   **Accounts** are restricted to non-bank accounts associated with the same subsidiary and currency as the selected bank account.
        
    -   Only classes, departments, and locations associated with the same subsidiary as the bank account are available.
        
3.  Repeat this process for each reconciled charge.
    
    An example of an other charge is your bank service charge.
    
    As you add transactions, the Reconciled This Statement field is updated, and the total of all the other charges is shown on the subtab.
    

#### New Deposits {#procedure_N1553343}

1.  Click the **New Deposits** subtab.
    
2.  Fill in the appropriate information for the deposit, and then click **Add**.
    
    You can enter a deposit with a date after the statement date for the reconciliation, and the deposit remains reconciled with this statement.
    
    An example of an other income is the interest your bank pays you.
    
    If you use NetSuite OneWorld, note the following:
    
    -   **Payor** (vendor, customer, or other entity) must be associated with the same subsidiary as the bank account.
        
        Note:
        
        If you have shared vendors and customers with multiple subsidiaries and this subsidiary is a secondary subsidiary to one or more shared entities, the **Payor** field lists all of the entities to which this subsidiary is assigned. Selecting a shared entity payor enables you to enter deposits for the entity as well as this subsidiary.
        
    -   **Accounts** are restricted to non-bank accounts associated with the same subsidiary and currency as the selected bank account.
        
    -   Only classes, departments, and locations associated with the same subsidiary as the bank account are available.
        
    
    As you add transactions, the **Reconciled This Statement** field is updated, and the total of all the other charges is shown on the subtab.
    
3.  Repeat this process for each reconciled deposit.
    

Note:

When you have cleared all the transactions listed on the statement and entered any additional charges or deposits, the **Ending Statement Balance** should equal the **Reconciled This Statement** balance plus the **Last Reconciled Balance**. Use the **Difference** field to track your progress in matching these balances.

When finished, choose one of three options:

-   Click **Save** to reconcile your bank statement.
    
-   Click **Save & Print** to save and print your reconciliation.
    
-   Click **Complete Later** to save your reconciliation until you return to submit or print it.
    

To view your previous reconciliations, go to _Transactions > Bank > Reconcile Bank Statement_. Click **History**.

### Related Topics

-   [Entering Transactions While Reconciling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1553560.html)
-   [Completing a Reconciliation at a Later Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1553886.html)
-   [Deleting a Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1554015.html)
-   [Printing Reconciliation Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1554190.html)
-   [Bank Register Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1554649.html)
-   [Reconciliation Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1555001.html)
-   [Reconciliation Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1556925.html)
-   [Reconciliation History Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1557193.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
