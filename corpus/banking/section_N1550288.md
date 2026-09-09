---
id: "section_N1550288"
type: "section"
title: "Reconciling Credit Card Statements"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Company Credit Cards > Reconciling Credit Card Statements"
parent: "chapter_N1548363"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1550288.html"
anchors: ["procedure_N1550346", "procedure_N1550406", "procedure_N1550480", "bridgehead_N1550557", "bridgehead_N1550622"]
sha256: "ab9bd7ca52fe508dc85fa0eac2cbef7f82ba804abc3a0d180a0a8361728c0d7a"
---

Note:

This is the original reconciliation feature, which is no longer supported as of NetSuite 2021.1. A redesigned version of transaction matching and statement reconciliation is available, which enables you to match and reconcile account transactions without requiring Microsoft Excel or third-party tools. For details, see [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html).

As with your bank statements, you should reconcile your credit card statement against your credit card register to keep your NetSuite accounts accurate.

If you use online banking, you can import credit card statement data. For more information, see [Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1550803.html).

The reconciliation process includes verifying transactions on your credit card account and your ledger account:

-   Payments and credits (such as for returned merchandise)
    
-   Charge and cash advances
    
-   Fees and chargebacks
    

You can mark a credit card transaction as cleared from the chart of accounts if it has gone through, but does not yet appear on the statement. Go to _Reports > Financial > Chart of Accounts_. Click the name of the account linked to the credit card. Check the box in the **Clr** column if a transaction is cleared, but not yet reconciled.

When you reconcile a transaction, it is automatically marked cleared. Transactions must be both cleared and reconciled before closing a period.

Tip:

You can unclear a cleared transaction through the register for the credit card account. Click Actions, then click Go To Register. On the account register, locate the transaction and clear the Clr box. This makes the transaction unreconciled again.

If you change the amount of a previously reconciled transaction, the transaction becomes unreconciled again. Open the correct statement period for the transaction and reconcile the transaction again.

Note:

If you change the account of the transaction, the transaction does not become unreconciled.

You can begin a credit card account reconciliation and then resume later. NetSuite preserves the reconciliation until you return to save it or save and print it. For more information, see [Completing a Reconciliation at a Later Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1553886.html).

#### To reconcile a credit card statement: {#procedure_N1550346}

1.  Go to _Transactions > Bank > Reconcile Credit Card Statement_. You can also access this page by clicking the **Reconcile** link for a transaction on the credit card's ledger account register.
    
2.  In the **Account** field, select the credit card you are balancing.
    
    If your account does not appear, on your account record, you need to clear the **Use Match Bank Data and Reconcile Account Statement Pages** box (see [Editing an Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4641794885.html)). As of NetSuite 2021.1, this box is automatically checked for newly-created accounts.
    
    Warning:
    
    The Reconcile Bank Statement and Reconcile Credit Card Statement pages are no longer supported and will be removed in the future. For information about the redesigned reconciliation feature, see [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html).
    
    If you use NetSuite OneWorld, the subsidiary associated with this account displays in the **Subsidiary** field.
    
    The **Last Reconciled Balance** field displays the balance of this account from the last time you reconciled your credit card statement. If it is incorrect, ensure that all previous reconciliations are complete and accurate.
    
3.  In the **Statement Date** field, enter or pick the date of the statement.
    
4.  In the **Start Date** field, enter the beginning of the reconciliation period.
    
5.  In the **Ending Statement Balance** field, enter the closing balance on the statement.
    
    The **Reconciled This Statement** field updates as you check off transactions.
    
    The **Difference** field keeps track of the difference between the **Ending Statement Balance** and the combined total of the **Last Reconciled Balance** and **Reconciled This Statement** fields.
    
    Tip:
    
    You can specify the number of items that display on the page at _Home > Set Preferences_ > General > Number of Rows in List Segments.
    

#### Payments and Credits {#procedure_N1550406}

1.  Click the **Payments and Credits** subtab.
    
    This subtab displays payments and credits to be reconciled.
    
    If you make a general journal entry against a credit card account, the entry on the **Payments and Credits** subtab displays in the **Credit** column in the register for the account.
    
    A **Yes** displays in the **Cleared** column for all transactions that have been marked as cleared on the account register. Transactions must be both cleared and reconciled before closing a period.
    
    The **Date** column displays the date of the transaction.
    
    Click the link to view the original transaction.
    
    The **Type** column displays the transaction type.
    
    The **Tran No.** column displays the check number reference.
    
    Click the link to view the original transaction.
    
    The **Payor** column displays to whom payments were made.
    
    Click the link to view the entity record.
    
    The **Memo** column displays a brief description or information about the nature of the transaction.
    
    The **Amount** column displays the total amount of the transaction.
    
    If you use NetSuite OneWorld, note that only transactions for the subsidiary associated with the credit card account are listed.
    
    Note:
    
    When you mark a transaction as reconciled, a transaction not marked cleared automatically clears.
    
2.  Check the boxes next to the transactions you want to reconcile.
    
    As you check transactions, the **Last Reconciled Balance** field is updated, and the total of those transactions displays on the subtab.
    
    -   To reconcile all payments and credits, click **Mark All**.
        
    -   If you mark credit card transactions as **Cleared** on an ongoing basis, when you open a reconciliation you can click **Mark All Cleared to Reconcile**. This button updates all transactions that are already cleared to be marked for reconciliation. Then, each transaction does not need to be marked individually.
        
3.  If you want to select and reconcile all transactions, click **Mark All**.
    

#### Charges and Cash Advances {#procedure_N1550480}

1.  Click the **Charges and Cash Advances** subtab.
    
    This subtab displays charges and cash advances made to this credit card account that need to be reconciled.
    
    If you make a general journal entry against a credit card account, the entry on the **Charges and Cash Advances** subtab displays in the **Charge** column in the register for the account.
    
    A **Yes** displays in the **Cleared** column for all transactions that have been marked as cleared on the account register. Transactions must be both cleared and reconciled to close out a period.
    
    The **Date** column displays the date of the transaction.
    
    Click the link to view the original transaction.
    
    The **Type** column displays the transaction type.
    
    The **Check No.** column displays the check number of the transaction, reference number of credit card transactions, and so on.
    
    Click the link to view the original transaction.
    
    The **Payee** column displays to whom payments were made.
    
    Click the link to view the entity record.
    
    The **Memo** column displays a brief description or information about the nature of the transaction.
    
    The **Amount** column displays the total amount of the transaction.
    
    If you use NetSuite OneWorld, note that only transactions for the subsidiary associated with the credit card account are listed.
    
    Note:
    
    When you mark a transaction as reconciled, a transaction not marked cleared automatically clears.
    
2.  Check the boxes next to the transactions you want to reconcile.
    
    As you check transactions, the **Last Reconciled Balance** field is updated, and the total of those transactions displays on the subtab.
    
    -   To reconcile all deposits and credits, click **Mark All**.
        
    -   If you mark credit card transactions as **Cleared** on an ongoing basis, when you open a reconciliation you can click **Mark All Cleared to Reconcile**. This button updates all transactions that are already cleared to be marked for reconciliation. Then, each transaction does not need to be marked individually.
        
3.  If you want to select and reconcile all transactions, click **Mark All**.
    

#### New Charges {#bridgehead_N1550557}

1.  Click the **New Charges** subtab.
    
2.  Fill in the appropriate information for each charge, and then click **Add**.
    
    If you use NetSuite OneWorld, note the following:
    
    -   **Payor** (vendor or other entity) must be associated with the same subsidiary as the credit card account.
        
        Note:
        
        If you have shared vendors and customers with multiple subsidiaries and this subsidiary is a secondary subsidiary to one or more shared entities, the **Payor** field lists all of the entities to which this subsidiary is assigned. Selecting a shared entity payor enables you to enter charges for the entity as well as this subsidiary. For more information about shared records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html) and [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    -   **Accounts** are restricted to non-bank accounts to which the subsidiary associated with the credit card account has access.
        
    -   Only classes, departments, and locations associated with the same subsidiary as the credit card account are available.
        
    
    As you add transactions, the **Reconciled This Statement** field is updated, and the total of all the other charges is shown on the subtab.
    

Note:

Charges you enter here are submitted if you click **Complete Later**, **Save**, or **Save & Print**.

#### New Credits {#bridgehead_N1550622}

1.  Click the **New Credits** subtab.
    
2.  Fill in the appropriate information for the credit, and then click **Add**.
    
    If you use NetSuite OneWorld, note the following:
    
    -   **Payee** (vendor, customer, or other entity) must be associated with the same subsidiary as the credit card account.
        
        Note:
        
        If you have shared vendors and customers with multiple subsidiaries and this subsidiary is a secondary subsidiary to one or more shared entities, the **Payee** field lists all of the entities to which this subsidiary is assigned. Selecting a shared entity payee enables you to enter credits for the entity as well as this subsidiary.
        
    -   **Accounts** are restricted to non-bank accounts to which the subsidiary associated with the credit card account has access.
        
    -   Only classes, departments, and locations associated with the same subsidiary as the credit card account are available.
        
    
    As you add transactions, the **Reconciled This Statement** field is updated, and the total of all the other charges is shown on the subtab.
    
    Note:
    
    Credits you enter here are submitted if you click **Complete Later**, **Save**, or **Save & Print**.
    
3.  Repeat for each credit.
    

When you have reconciled all the transactions listed on the statement and entered any additional credits or charges, the statement balance should equal the sum of the last reconciled balance and the transactions reconciled this statement.

Use a balance adjustment journal entry to manage any difference.

Use the **Difference** field to track your progress in matching these balances.

When you have finished, choose one of three options:

-   Click **Save** to reconcile your credit card statement.
    
-   Click **Save & Print** to save and print your reconciliation.
    
-   Click **Complete Later** to save your reconciliation until you return to submit or print it.
    

Note:

When you click **Complete Later**, only the reconciliation is reserved. Credits and charges entered on the **New Credits** and **New Charges** tabs are submitted as new transactions.

Your credit card account is reconciled. To view your three previous reconciliations, go to _Transactions > Bank > Reconcile Credit Card Statement_. Click **History**. For more information, see [Reconciliation History Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1557193.html).

To view the Reconciliation Summary report for your account, go to _Reports > Banking/Budgeting > Reconciliation_. You can click **View Detail** to see reconciliation details. For more information, see [Reconciliation Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1555001.html) and [Reconciliation Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1556925.html).

Warning:

Although you can edit a previously saved reconciliation statement, you should delete the statement and create a new one. Editing a previously saved reconciliation statement can cause future reconciliation imbalances. See [Deleting a Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1554015.html).

### Related Topics

-   [Creating Company Credit Card Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3758988949.html)
-   [Entering Company Credit Card Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548500.html)
-   [Paying the Company Credit Card Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548897.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
