---
id: "section_N1693662"
type: "section"
title: "Deferring Revenue When Billing Costs to a Customer"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Deferring Revenue When Billing Costs to a Customer"
parent: "chapter_N1678106"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1693662.html"
anchors: ["bridgehead_N1693746", "procedure_N1693760", "procedure_N1693850", "bridgehead_N1693937", "bridgehead_N1694638"]
sha256: "c16e416f6b25df24a47016990de866e1551f6fce63828dd18e17f4098012485c"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Revenue Arrangement Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4333740355.html).

NetSuite lets you bill costs back to customers for time, items, and expenses you incur while working on a project for them. You can recognize the income over time and defer the sales revenue for these billed costs.

First, you must enable the Bill Costs to Customers feature. For more information, read [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html).

Defer revenue from costs you bill to customers using the following steps.

1.  [Billing Customers for Expenses Related to Deferred Revenue](#bridgehead_N1693746).
    
2.  [Enter the time, item, or expense, and mark it as billable](#bridgehead_N1693937).
    
3.  [Create an invoice that bills the customer for the cost you entered](#bridgehead_N1694638).
    

## Billing Customers for Expenses Related to Deferred Revenue {#bridgehead_N1693746}

You can set up expense accounts or items so that you can bill them to a customer and recognize revenue in a revenue account linked to that expense account or item.

#### To set up an expense account to post to a deferred revenue account: {#procedure_N1693760}

1.  Go to _Lists > Accounting > Accounts_.
    
2.  Click **Edit** next to the expense account you want to update.
    
3.  On the account record, in the **Track Billable Expense in** field, select an account. For example, select the **Sales** account. Then click **Save**.
    
4.  Open the record of the account you selected in the previous step. From the example, you would open the Sales account.
    
5.  Select an account in the **Deferral Account** field. For example, select Deferred Revenue.
    
6.  Click **Save**.
    

#### To set up an item to post to a deferred revenue account: {#procedure_N1693850}

1.  To set up an item, go to _List > Accounting > Items_.
    
2.  Click **Edit** next to the item.
    
3.  In the **Accounting** subtab on the item record, select a **Deferred Revenue Account**.
    
4.  Click the **Revenue Recognition / Amortization** subtab, and select a **Revenue Recognition Template** to associate with this item on sales transactions.
    
    If you don't select a template on the item record, you must manually select the revenue recognition schedule on the **Billable Items** subtab of the sales transaction.
    
5.  Click **Save**.
    

## Enter the time, item, or expense, and mark it as billable {#bridgehead_N1693937}

When you enter time transactions, purchase orders, bills, checks or credit card payments for time, an item or expense, you can check the Billable box and assign a billable customer for the item or expense.

Then, when you create an invoice for the customer, the expense appears on a Billable subtab.

## Create an invoice that bills the customer for the cost you entered {#bridgehead_N1694638}

When you create a customer invoice, the costs you've billed to customers show on the Billable Items, Billable Expenses and Billable Time subtabs. Click the appropriate subtab and check the line items you want to bill the customer for. Then click Save.

Note:

To generate deferred revenue for billable time, you must manually select revenue recognition schedules on the **Billable Time** subtab.

The items and expenses appear as normal line items on the invoice. The customer sees only a selling price that includes the markup spread over the expense items. However, you see the markup as a separate entry when you view the invoice in NetSuite.

On the Billable Expenses subtab of the invoice, you can select a schedule or enter revenue recognition dates for the time, item or expense.

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)
-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html)
-   [Revenue Recognition Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1695172.html)
-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
