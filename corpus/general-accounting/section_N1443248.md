---
id: "section_N1443248"
type: "section"
title: "Merging Accounts"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Chart of Accounts Management > Making Changes to Accounts > Merging Accounts"
parent: "section_N1442743"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1443248.html"
anchors: ["procedure_N1444791"]
sha256: "8d15c94429cb7e54efc56c41e0f1703b062e206ac98845a72752ce1f260624ad"
---

Merging accounts enables you to combine all the information and transactions from one account into another.

Important:

Merging bank and credit card accounts automatically un-reconciles the reconciled transactions in the Merge From account. You must re-reconcile these transactions in the register of the Merge To account.

You can merge one account into another if they're the same account type and the account you want to merge has no attached subaccounts. You can combine an account with a parent account or with a subaccount. For example, a store owner has a bank account for petty cash and a bank account for cash-on-hand. The owner has decided to keep all the cash in one place. Because the petty cash account doesn't have any subaccounts, the owner can merge that account into the cash-on-hand account.

Important:

You can't merge summary accounts.

The following accounts can't be merged:

-   Accounts Payable
    
-   Accounts Receivable
    
-   Advances Paid
    
-   Inventory Asset
    
-   Undeposited Funds
    
-   Failed ACH Transactions
    
-   Intercompany Clearing
    
-   Intercompany Payable/Receivable
    
-   Accrued Purchases
    
-   Payroll Liabilities
    
-   Refunds Payable
    
-   Sales Taxes Payable
    
-   Opening Balances
    
-   Cost of Goods Sold
    
-   Uncategorized Income
    
-   Uncategorized Expense
    
-   ALL non-posting registers
    

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In 2013.1, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. In 2014.1, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that are not currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html) and [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

#### To merge accounts: {#procedure_N1444791}

1.  Go to _Lists > Accounting > Accounts_.
    
    Note:
    
    Your user role must have both ADMI\_ACCOUNTING and LIST\_ACCOUNT permissions to access _Setup > Accounting > Manage G/L > Chart of Accounts_.
    
2.  Click the **Edit** link to the left of the account you want to merge into another account.
    
3.  On the Account page, from the **Actions** list, select **Merge**.
    
4.  On the Merge Accounts page, select the account into which you want to merge this account.
    
    Only similar account types show in the **Merge Into** list.
    
5.  Click **Save**.
    
6.  At the prompt to confirm the merge, click **OK**.
    
    The chart of accounts displays the combined accounts.
    

The information and transactions for this account are combined with those of the account into which you merged. In the example above, the transactions for petty cash now appear on reports as cash-on-hand transactions.

### Related Topics:

-   [Changing Names of General Ledger Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442914.html)
-   [Adding or Changing Account Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1443085.html)
-   [Deleting Accounts and Making Accounts Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1444958.html)
-   [Making Changes to Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442743.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
