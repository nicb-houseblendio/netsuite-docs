---
id: "section_N1774211"
type: "section"
title: "Setting an Amortization Template on a Vendor Credit Line Item"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Configuration for Amortization > Setting an Amortization Template on a Vendor Credit Line Item"
parent: "section_N1773475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html"
anchors: ["procedure_N1774250", "procedure_N1774376"]
sha256: "547c302034bf4aa35305ddc3128ab4a6a16f632e57a973511722fd5a348aeaf6"
---

To create a vendor credit, you can enter an individual vendor credit transaction or generate a credit from an existing vendor bill. You can select amortization templates for items when you enter a credit.

On a generated credit, items inherit amortization templates from the related bill. These inherited templates can't be edited. You can add templates for items that didn't have them on the bill, and add items with templates, to a generated credit.

Important:

When using amortization, you should change expenses on purchase transactions using vendor credits rather than changing the original transaction. This preserves your historical data and audit trail. For an example, see [Vendor Credit Amortization Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774542.html).

#### To associate an amortization template with an item on a vendor credit: {#procedure_N1774250}

1.  Go to _Transactions > Purchases/Vendors > Enter Vendor Credits_.
    
2.  Under Primary Information, select values for the fields as needed.
    
3.  On the **Items** subtab, select an item.
    
4.  In the **Amort. Schedule** column, select the appropriate template.
    
    A deferral account must be specified one either the template or the item record. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).
    
    If you select a variable template, you must also select the associated project in the Customer column dropdown.
    
5.  Enter an amortization start and end date, if needed.
    
    An error occurs if either of these dates is in an accounting period that isn't yet set up. You must create accounting periods for the range of time your amortization schedules will cover. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).
    
    An error also occurs if either of these dates is before the posting period selected for the transaction.
    
6.  Enter the residual amount not to be recognized if needed.
    
7.  Enter additional information as needed for this line item.
    
8.  Click **Add**.
    
9.  Click **Save**.
    

Now, the item is associated with the amortization template for this vendor credit. When the transaction is saved, an amortization schedule is created.

A vendor credit created from an existing bill retains the bill's amortization settings and posts to accounts appropriately. The deferred expense is debited, the expense account is credited and the amortization dates from the bill autofill on the vendor credit.

#### To generate a credit directly from an existing vendor bill: {#procedure_N1774376}

1.  To generate a credit from a bill, go to _Transactions > Purchases/Vendors > Enter Bills > List_, and click **View** beside a bill
    
2.  In the vendor bill record, click **Credit**.
    
3.  Verify that an amortization template appears in the **Amort. Schedule** column for the line and other information is correct.
    
4.  Click **Save**.
    

Note:

If amounts are set to be posted to periods that have closed between the posting date of the vendor credit and the **Amortization Start Date**, these amounts post to the oldest open period.

### Related Topics

-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)
-   [Setting an Amortization Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773719.html)
-   [Setting an Amortization Template on a Vendor Bill Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773966.html)
-   [Vendor Credit Amortization Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774542.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
