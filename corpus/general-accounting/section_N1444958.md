---
id: "section_N1444958"
type: "section"
title: "Deleting Accounts and Making Accounts Inactive"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Chart of Accounts Management > Making Changes to Accounts > Deleting Accounts and Making Accounts Inactive"
parent: "section_N1442743"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1444958.html"
anchors: ["procedure_N1445003", "procedure_N1445069"]
sha256: "3454976479c6db5b12586f711ef56dcdc30fcba8df9ff51ad4160ebad1475b7c"
---

An account is a category of transactions related to a specific type of asset, liability, equity, income, or expense. Your accounts are listed in your chart of accounts. You can customize your chart of accounts to make it more useful. You can delete accounts that are never used, inactivate accounts that are not currently being used, or both.

-   Accounts that are inactive appear in your chart of accounts only when the Show Inactives box is checked. If you don't want to see inactive accounts, clear the Show Inactives box on the chart of accounts. Marking an account inactive **doesn't** alter the amount in that account. You must move any amount to another account to reduce the amount to zero.
    
-   Accounts that have been deleted no longer show in your chart of accounts.
    

Many accounts can't be deleted. You can delete an account if there is no activity in the account and if the account isn't required by NetSuite. For example, the non-posting Sales Order account can't be deleted because NetSuite uses this account for sales orders. Also, certain accounts can't be deleted because they're required for reporting purposes. Reports are hard-coded with these accounts, therefore, NetSuite doesn't permit you to delete them. You can, however, make them inactive.

You can delete or make accounts inactive from individual account records, or directly on the chart of accounts list.

#### To delete or make accounts inactive from account records: {#procedure_N1445003}

1.  Go to _Lists > Accounting > Accounts_.
    
2.  Click the **Edit** link for an account that you want to delete or mark inactive.
    
3.  On the Edit Account page, from the **Actions** list, select **Delete**.
    
    If **Delete** isn't available in the **Actions** list, this account can't be deleted.
    
4.  To make an account inactive, check the **Inactive** box.
    
    Summary accounts are inactive by default. To automatically inactivate its children accounts, first edit the account record to clear the **Summary** box and then save the record. Second, edit the account record to clear the **Inactive** box and then save the record. Third, edit the account record to check the **Inactive** box and then save the record. All children accounts are updated to inactive status.
    
    Important:
    
    Inactivating and activating accounts may limit access to subsidiaries for users assigned custom roles.
    
5.  Click **Save**.
    

#### To delete or make accounts inactive from the chart of accounts list: {#procedure_N1445069}

1.  Go to _Lists > Accounting > Accounts_.
    
2.  Check the **Show Inactives** box.
    
    Your chart of accounts refreshes and an **Inactive** column and a **Delete** column are added.
    
3.  For the accounts you want to delete or make inactive, check the boxes in the appropriate columns.
    
    Accounts that have the word **No** in the **Delete** column can't be deleted from your chart of accounts.
    
4.  Click **Submit**.
    

Important:

If you receive a warning that an account can't be deleted because it's associated to a child entity or transaction, you must delete all transactions associated with the account before you can delete the account. You can do a transaction search filtered by the account to review the associated transactions. If you can't delete these transactions, you can mark the account inactive.

### Related Topics:

-   [Changing Names of General Ledger Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442914.html)
-   [Adding or Changing Account Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1443085.html)
-   [Merging Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1443248.html)
-   [Making Changes to Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442743.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
