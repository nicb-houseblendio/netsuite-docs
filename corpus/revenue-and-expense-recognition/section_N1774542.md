---
id: "section_N1774542"
type: "section"
title: "Vendor Credit Amortization Example"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Configuration for Amortization > Vendor Credit Amortization Example"
parent: "section_N1773475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774542.html"
anchors: []
sha256: "ff37a1ca9a295e2d6ef2cba77890ac1a829799707cce43b5bce536943696a5fb"
---

When using amortization, you should change expenses on purchase transactions using vendor credits rather than changing the original transaction. This preserves your historical data and audit trail.

When an item on a vendor credit is associated with an amortization template, expense recognition that's occurred is backed out of deferral accounts and expense accounts according to the schedule.

For example, a bill is created for $1200 and spans 12 amortization periods. $1200 posts to the deferred expense account when the vendor bill posts. Then, after the first period is over, $100 is removed from the deferred expense account and moved to the appropriate expense account.

Next, you enter a vendor credit for the $1100 that is still deferred and not yet posted to the expense account. The $1100 credit spans the remaining 11 amortization periods from the original bill.

In the second amortization period, the $1100 is backed out of the deferred expense account. For the remainder of the bill term, one time each period an amortization journal entry debits and credits the expense account for $100, with a net effect of $0.

### Related Topics

-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)
-   [Setting an Amortization Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773719.html)
-   [Setting an Amortization Template on a Vendor Bill Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773966.html)
-   [Setting an Amortization Template on a Vendor Credit Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
