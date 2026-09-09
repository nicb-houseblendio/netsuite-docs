---
id: "section_N1773966"
type: "section"
title: "Setting an Amortization Template on a Vendor Bill Line Item"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Configuration for Amortization > Setting an Amortization Template on a Vendor Bill Line Item"
parent: "section_N1773475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773966.html"
anchors: ["procedure_N1773986"]
sha256: "76deeee4e558b3a77cc3a8ba229f7b231f3b912baea3a308a157f4f9107c02c9"
---

When you enter a vendor bill, you can select amortization templates for items. You can modify the default template set in the item record or select a template when no default is available.

You can't select an amortization template for a vendor bill line derived from purchase order line with an accrual. The amortization settings are disabled for these lines on the vendor bill.

#### To associate an amortization template with an item on a vendor bill: {#procedure_N1773986}

1.  Go to _Transactions > Payables > Enter Bills_.
    
2.  Under Primary Information, select values for the fields as needed.
    
3.  On the **Items** subtab, select an item.
    
4.  In the **Amort. Schedule** column, select the appropriate template from the dropdown list.
    
    A deferral account must be specified on either the template or the item record. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).
    
    If you select a variable template, you must also select the associated project in the **Customer** column dropdown list.
    
5.  Enter an amortization start and end date, if needed.
    
    You must create accounting periods for the range of time your amortization schedules will cover, or an error will occur when you save the transaction. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).
    
    You'll also get an error if the start or end date is before the posting period selected for the transaction.
    
6.  Enter the residual amount not to be recognized if needed.
    
7.  Enter additional information as needed for this line item.
    
8.  Click **Add**.
    
9.  Repeat the steps on the **Items** subtab for additional items as needed.
    
10.  Click **Save**.
     

The item on the bill associated with an amortization template posts to a deferred expense account instead of a regular expense account.

You can customize a transaction form to use a specific template for all items on the transaction. To do so, click **Customize** on the form.

### Related Topics

-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)
-   [Setting an Amortization Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773719.html)
-   [Setting an Amortization Template on a Vendor Credit Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html)
-   [Vendor Credit Amortization Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774542.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
