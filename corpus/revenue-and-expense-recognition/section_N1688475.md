---
id: "section_N1688475"
type: "section"
title: "Setting a Revenue Recognition Template on a Transaction Item Line"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Associating Revenue Recognition Templates with Items > Setting a Revenue Recognition Template on a Transaction Item Line"
parent: "section_N1687451"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688475.html"
anchors: ["procedure_N1688545"]
sha256: "316fa15ed00c6400d9ea92f9c67b5f9285cd92974e71a594044039ba6949e7b3"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For information about the current feature, see [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

When you enter sales transactions, you can change the revenue recognition template for the item lines. The template change applies to the specific transaction only. Your change may modify a default from the item record or to select a value when there is no default.

You can apply revenue recognition templates to items on the following types of transactions:

-   Sales Orders
    
-   Invoices
    
-   Cash Sales
    
-   Revenue Commitments
    
-   Cash Refunds
    
-   Return Authorizations
    
-   Revenue Commitment Reversals
    
-   Credit Memos
    

Important:

You can't associate a revenue recognition template with an item unless it has a Deferred Revenue Account selected on the item record. You can't add a revenue recognition template to the following transaction types when the transaction is in a closed period: invoice, credit memo, cash sale, and cash refund.

#### To change the revenue recognition template on an item line: {#procedure_N1688545}

1.  On the transaction record, select values for the main body fields as needed.
    
2.  On the **Items** subtab, select an item.
    
3.  In the **Rev. Rec. Schedule** column, select the appropriate template.
    
    If you select a variable template, you must also select the associated project in the **Customer** column.
    
4.  Select the following additional values for the line item as needed:
    
    -   **Rev. Rec. Start Date** - Whether this date is required is determined by the Revenue Recognition Term Source on the Revenue Recognition Template. For more information, see [Revenue Recognition Term Source](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1680012).
        
    -   **Rev. Rec. End Date** - Whether this date is required is determined by the Revenue Recognition Term Source and Revenue Recognition Period on the Revenue Recognition Template. For more information, see [Revenue Recognition Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1683147).
        
    -   **VSOE** - This column is available only when the VSOE feature is enabled. Click the pencil icons to display the VSOE fields. For more information, see [Using Percent-Complete Revenue Recognition for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1694795.html) and [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
        
5.  Click **Add**.
    
6.  Click **Save**.
    

Now the item is associated with the revenue recognition template for this sale, and a revenue recognition schedule will be generated. The point at which this schedule is generated varies according to the type of transaction and your account's enabled features preference settings. For example, if an approval process is in place, a schedule isn't generated for a sales order until it's approved.

-   When an invoice or cash sale contains an item with a revenue recognition template, a revenue recognition schedule is created when the sale is approved or saved.
    
-   When a sales order contains an item with a revenue recognition template, a revenue recognition schedule is created when the sale is billed.
    

Note:

You may be able to customize a transaction form to use a particular revenue recognition template for all items on the transaction. To do so, click **Customize** on the form.

### Related Topics

-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)
-   [Setting a Revenue Recognition Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687732.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Deferring Revenue for Discount and Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688734.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
