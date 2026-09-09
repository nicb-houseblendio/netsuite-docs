---
id: "chapter_N1678106"
type: "chapter"
title: "Using Revenue Recognition"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition"
parent: "book_N1675734"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html"
anchors: []
sha256: "87413adfe0852384e5a69382679343397d91ee1de0476b280df9c3d5e28871e1"
---

Note:

Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For information about the current feature, see [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

The Revenue Recognition feature lets you record the general ledger impact of sales transactions across multiple future periods.

The Accounting Periods feature must be enabled before the Revenue Recognition feature can be enabled. When Revenue Recognition is enabled, NetSuite automatically adds a default account with a type of Deferred Revenue to the Chart of Accounts because at least one account of this type is required for the feature. You can create additional Deferred Revenue type accounts as needed. For more information about enabling this feature and setting associated preferences, see [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html).

After Revenue Recognition has been enabled, you can create revenue recognition templates that indicate how revenue from associated items should be posted. For each template, you can select from a choice of standard terms or define your own custom terms, set the time period over which recognition occurs, define an offset to delay the start of recognition, and set up an initial amount to be recognized. For more information, see [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html).

To recognize revenue for the sale of an item, you must associate a deferred revenue account with that item on its item record. You can set a revenue recognition template on an item record. This template becomes the default for all sales of the item. You can also associate a revenue recognition template with an item on the item line of a transaction record to apply only to that specific item sale. For more information, see [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html).

Revenue recognition schedules are generated for sales transactions containing items that have associated revenue recognition templates. Each schedule indicates the posting periods when revenue should be recognized and the amount to be recognized in each period for each item sale. For more information, see [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html).

Revenue recognition schedules provide a basis for the generation of journal entries that record the impact of item sales. NetSuite provides a user interface for you to generate all journal entries required for revenue recognition for a selected posting period. For information, see [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html).

If the Bill Costs to Customers feature is enabled so that you can bill costs back to customers for time, items, and expenses incurred on projects, you can defer the sales revenue for these costs that you bill. See [Deferring Revenue When Billing Costs to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1693662.html).

If the Project Management feature is enabled, you can use variable revenue recognition schedules to recognize revenue based on the percentage of project work completed. See [Using Percent-Complete Revenue Recognition for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1694795.html).

NetSuite provides revenue recognition reconciliation reports. For information, see [Revenue Recognition Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1695172.html).

Important:

The Revenue Recognition feature must be enabled for the following features to be available: Revenue Commitments, VSOE, and Sales Order Revenue Forecasting.

### Related Topics

-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)
-   [Using Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1701780.html)
-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Using Sales Order Revenue Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1750747.html)
-   [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html)
-   [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
