---
id: "section_N1688734"
type: "section"
title: "Deferring Revenue for Discount and Markup Items"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Associating Revenue Recognition Templates with Items > Deferring Revenue for Discount and Markup Items"
parent: "section_N1687451"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688734.html"
anchors: []
sha256: "d4a19356ad084c8b36d227c40709c497b3465578016af19da5264dbc6045fecf"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Discount and Markup Items in Advanced Revenue Management (Essentials)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4369060813.html).

This topic describes behavior for the classic Revenue Recognition feature. For the Advanced Revenue Management (Essentials) behavior, see [Discount and Markup Items in Advanced Revenue Management (Essentials)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4369060813.html). The behavior is different.

To discount or markup transactions and items that defer revenue, you must use **non-posting** discount and markup items. This ensures that both the net amount of each line and the transaction as a whole are recognized correctly. Posting discounts can't be applied to sales transactions that have revenue recognition templates or schedules.

Non-posting discount and markup items don't post to a general ledger account. When a discount/markup item without an account specified is added to a transaction, it doesn't post as an individual transaction line. Instead, the item to which it's applied posts the net amount of the discount/markup. For example, when you create a sales transaction and add a non-posting discount after a line-item, the discount is applied to the previous line-item only. The net amount of the transaction is then correct and the appropriate revenue posts.

For example, you can create a sales transaction that sells a service item for $1,200.00 to be recognized over 12 periods. You want to apply a $200.00 discount to the service item, making the total invoiced amount $1,000.00.

If you apply the discount using a non-posting discount item in the amount of $200.00, then the discount doesn't post to the general ledger when the transaction is saved. Instead, the discount is applied to the line-item amount and adjusts the net amount of the invoice. Then the total amount scheduled for amortization is $1,000.00.

If you had instead applied a posting discount, the full $1,200 posts to the ledger, in addition to a $200 offsetting debit posting to the related discount account. This distorts the revenue recognition and isn't allowed when sales transactions have revenue recognition templates or schedules.

The net amount posted on a transaction is also used to make commission calculations when you use the Commissions feature.

For more information about non-posting discount items, read [Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html).

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)
-   [Setting a Revenue Recognition Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687732.html)
-   [Setting a Revenue Recognition Template on a Transaction Item Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688475.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
