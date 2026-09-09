---
id: "section_N2415916"
type: "section"
title: "Creating an Expense Category"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Expenses > Creating an Expense Category"
parent: "chapter_N2415855"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415916.html"
anchors: ["procedure_N2415948", "subsect_157920746063"]
sha256: "0a36664b993398d0dc127ea03507a7ddce9383127b86daf63613683d68010c84"
---

Expenses can be grouped into expense categories that are associated with specific expense accounts.

When employees enter expense reports, they select a category for each expense, and the expense automatically posts to the associated expense account.

#### To create an expense category: {#procedure_N2415948}

1.  Go to _Setup > Accounting > Setup Tasks > Expense Categories > New_.
    
2.  In the **Name** field, enter the name of this expense category.
    
3.  In the **Description** field, enter a description of this category.
    
    This description shows in the Expense Categories list.
    
4.  If you use Charge-Based Billing, in the **Expense Item** field, select an item to associate with this category.
    
    For more information, see [Expense Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4042372470.html).
    
5.  In the **Expense Account** field, select the expense account for items charged to this category.
    
    Create new accounts at _Lists > Accounting > Accounts > New_.
    
6.  If you use corporate card expenses for expense reports, check the **Personal Corporate Card Expense** box. This designates this expense category for personal expenses charged to a corporate credit card. For more information, see [Corporate Card Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531259544.html).
    
    Note:
    
    Corporate card expense categories can only use other asset accounts. If your company doesn't use expanded account lists, the corporate card field on expense categories is disabled. Any expense category attached to an other asset account is automatically designated a corporate card expense. To enable the expanded account list preference, go to _Setup > Accounting > Preferences > Accounting Preferences_ > General Ledger.
    
7.  If you would like to specify a rate for this category on expense reports, check **Rate is Required** and enter a default rate.
    
    When entering expense reports with this category, the **Quantity** and **Rate** fields are used to calculate the expense amount.
    
8.  If you use OneWorld, select the subsidiaries you want this expense category to be available to. The list of available subsidiaries is filtered based on the subsidiaries available to use the selected expense item or expense account.
    
9.  Click **Save**.
    

You can choose to add the Expense Category field to show on the expense sublist of purchase transactions. Then, line-item expenses can be grouped by category. When you choose a category in the expense sublist, the account defaults from the category record and can"t be changed.

The following transactions can be customized to show expense categories:

-   Checks
    
-   Bills
    
-   Vendor Credits
    
-   Purchase Orders
    
-   Expense Reports
    

To customize a transaction, view the transaction and click Edit. Then, in the Customize list, click Customize Form.

## Expense Account Override on Expense Reports {#subsect_157920746063}

You can select an expense account for individual expense items on an expense report. By default, expense accounts on line items for expense reports are determined by the selected expense category. The Account field is automatically hidden on expense report forms for line items. You must customize your expense report forms to enable expense account override.

You can also remove the Category field from expense reports and the field is no longer required. The Account field is now required. It is populated automatically by the Category field. However, you can update the Account field to select a different account.

Note:

You can"t use personal corporate card expenses if you hide the Category field on expense line items.

You can change the settings of the Expense Account field on the Custom Transaction form. The Expense Account field is hidden by default. Keep it hidden for roles that don't need to work with this field. If you experience inconsistencies in the expense category, you can fix the account by re-selecting the expense category (select another category and then select the correct category again). This action will set the account to be the same as the account in the expense category.

For more information, see [Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907845.html) and [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

### Related Topics

-   [Creating a Saved Search With Expense Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162020704920.html)
-   [Receiving Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2416180.html)
-   [Receiving Expenses With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2416424.html)
-   [Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2416930.html)
-   [Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2415855.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
