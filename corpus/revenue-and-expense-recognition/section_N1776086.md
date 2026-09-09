---
id: "section_N1776086"
type: "section"
title: "Amortization Schedules"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Schedules"
parent: "chapter_N1765678"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776086.html"
anchors: []
sha256: "0ca246edce5fc6b4ec30ed23f9968fc4c06b7dd71602a7c92fbf0d290c262313"
---

After the Amortization feature has been set up, amortization schedules are generated for purchase transactions containing items or expense lines that have associated amortization templates. Each schedule indicates the posting periods in which expenses should be recognized, and the amount to be recognized in each period.

An amortization schedule is generated when the purchase transaction is saved. If you're using approval routing for vendor bills, the amortization schedule isn't created until the bill is approved. The only way to delete an amortization schedule is to remove the line that has an amortization schedule from the transaction.

Note:

You can't delete a schedule that has associated journal entries. If you need to delete a schedule that has posted journal entries associated with it, you must delete the journal entry before you can delete the schedule.

The amortization schedule isn't a transaction and doesn't post to the general ledger. The schedule details the expense amounts that will post and when they'll post to recognize deferred expenses over time. The amortization posting occurs when you generate amortization journal entries. See [Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777836.html).

You can't generate an amortization schedule for a vendor bill line derived from a purchase order line with an accrual. The amortization settings are disabled for these lines on the vendor bill.

Amortization schedules determine the journal entries that need to be generated to record the impact of purchased items and expenses. For each posting period, NetSuite provides a list of journal entries required to recognize expenses. See [Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777836.html).

Amortization schedules and the journal entries generated from them are subsidiary specific in NetSuite OneWorld. You can view and edit only amortization schedules and journal entries for subsidiaries to which you have access.

The Lists permission Amortization Schedules controls access to amortization schedules. For more information, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).

See the following for information about working with amortization schedules:

-   [Reviewing the Amortization Schedules List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776296.html)
    
-   [Viewing an Amortization Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776675.html)
    
-   [Editing an Amortization Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777207.html)
    
-   [Mass Updating Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777416.html)
    
-   [Creating an Amortization Schedule Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0822030054.html)
    

### Related Topics

-   [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html)
-   [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html)
-   [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html)
-   [Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777836.html)
-   [Using Percent-Complete Amortization for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780615.html)
-   [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html)
-   [Amortization Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1789982.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
