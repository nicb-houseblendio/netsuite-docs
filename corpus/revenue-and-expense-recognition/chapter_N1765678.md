---
id: "chapter_N1765678"
type: "chapter"
title: "Expense Amortization"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization"
parent: "book_N1675734"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html"
anchors: []
sha256: "3c5d0ff5a8dee939a90b2d00821fcc83910de279e04feeabb87c773094418ab7"
---

The Amortization feature enables you to record the general ledger impact of item purchases and expense charges across multiple future periods. The Accounting Periods feature must be enabled before the Amortization feature can be enabled.

The process for amortizing expenses is similar to deferred revenue recognition methods, and you can use them together. For more information, see [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html) and [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

When Amortization is enabled, NetSuite automatically adds a default account with a type of Deferred Expense to the Chart of Accounts because at least one account of this type is required for the feature. NetSuite doesn't differentiate between prepaid expense and deferred expense. Accounts of the type Deferred Expense are included as Other Current Assets on the balance sheet. You can create additional Deferred Expense accounts as needed. For more information about enabling this feature and setting associated preferences, see [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html).

Important:

When the Amortization feature is enabled, you should make change to expenses on purchase transactions by using vendor credits rather than changing the original transaction. This preserves your historical data and audit trail. See [Vendor Credit Amortization Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774542.html) and [Setting an Amortization Template on a Vendor Credit Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html).

After Amortization has been enabled, you can create amortization templates that indicate how to post expenses from associated items and expenses. For each template, you can select from a choice of standard terms or define your own custom terms, set the time period over which recognition occurs, define an offset to delay the start of recognition, and set up an initial amount to be recognized. See [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html).

To amortize costs for an item on a bill or bill credit, an amortization template must be associated with the item and a deferral account must be specified on the item record or on the template. You can set an amortization template on an item record. This template becomes the default for the item on all bills and credits. You also can associate an amortization template with an item on the item line of bill or credit to apply only to that specific item purchase. See [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html).

To amortize costs for an expense, an amortization template must be associated with the expense line item on the transaction record, and a deferral account must be specified on the account record or on the template used. See [Associating Amortization Templates with Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html).

Amortization schedules are generated for vendor bills and credits containing items or expenses that have associated amortization templates. Each schedule indicates for an item sale the posting periods in which expenses should be recognized and the amount to be recognized in each period. See [Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776086.html).

Amortization schedules provide a basis for the generation of journal entries that record the impact of amortized items and expenses. When you enter a vendor bill, the bill item amounts post directly to an expense account except for items associated with amortization templates. For information about vendor bills without amortization, see [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html). When an amortization template is linked, the expense amount is deferred by posting to a deferred expense account. The amount is later recognized as an expense by moving it out of the deferral account and into a regular expense account using general journal entries at scheduled intervals. NetSuite provides a user interface where you can generate all journal entries required for amortization for a selected posting period. See [Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777836.html).

You can also link an amortization template to a manual journal entry to create an amortization schedule for the journal entry. For instructions to do this, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).

If the Project Management feature is enabled, you can use variable amortization schedules to recognize expenses based on the percentage of project work completed. See [Using Percent-Complete Amortization for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780615.html).

In U.K. editions, use a foreign currency amortization schedule to amortize the foreign currency amounts of transactions rather than the base currency amounts. Create journals using the historical transaction exchange rates. See [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html).

NetSuite provides amortization reports. See [Amortization Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1789982.html).

### Related Topics

-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)
-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Using Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1701780.html)
-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Using Sales Order Revenue Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1750747.html)
-   [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
