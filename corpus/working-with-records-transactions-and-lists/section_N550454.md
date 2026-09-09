---
id: "section_N550454"
type: "section"
title: "Defining Subsidiaries for OneWorld Transactions"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Creating Transactions > Defining Subsidiaries for OneWorld Transactions"
parent: "section_N546079"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550454.html"
anchors: []
sha256: "4c81726318e3a187a891b7686ac883fb3cec796892165f0131d0d696aa68718f"
---

Each transaction in NetSuite OneWorld, except advanced intercompany journal entries, is tied to one subsidiary. When a transaction includes an entity, such as a customer, the transaction is assigned to the same subsidiary as the entity. For transactions without entities, you must manually select a subsidiary. When you process transactions in bulk, such as fulfillments, bill payments, or commission authorizations, select the appropriate subsidiary to filter the list of transactions to process.

Intercompany journal entries post to two subsidiaries. These journal entries record transactions between subsidiaries. Each advanced intercompany journal record includes an originating subsidiary and one or more receiving subsidiaries. For more information, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html).

Some time entries and expense transactions may be associated with multiple subsidiaries. Each time or expense record is associated with the subsidiary of the employee. In addition, a customer or project can be defined for each line of these records. If the Intercompany Time and Expenses feature isn't enabled, each line-level customer or project must be associated with the same subsidiary as the employee. If this feature is enabled and related accounting preferences are set, customers and projects from other subsidiaries can be selected at the line-level. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html), [Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908140.html), and [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html).

When a transaction has line-level associations to more than one subsidiary, the general ledger posts only to the subsidiary identified in the transaction header. Advanced intercompany journal entries can be created to transfer time, expense, or both charges from one subsidiary to another. An automated adjustment process is available for intercompany expenses. For more information, see [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html).

Note:

In NetSuite OneWorld, List view pages and search results convert the transaction currency to the base currency of the user's subsidiary. For more information about List view pages, see [List View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495842.html#bridgehead_N495933).

### Related Topics

-   [Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546079.html)
-   [Working with Addresses on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N553515.html)
-   [Creating New Records as You Enter Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546596.html)
-   [Editing Records as You Enter Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546716.html)
-   [Using Transaction Links](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551392.html)
-   [Linking a Transaction to a Support Case](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4470989794.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
