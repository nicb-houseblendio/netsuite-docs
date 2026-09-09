---
id: "section_N1687451"
type: "section"
title: "Associating Revenue Recognition Templates with Items"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Associating Revenue Recognition Templates with Items"
parent: "chapter_N1678106"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html"
anchors: []
sha256: "33d4a7c644025accfcbfd86fc29879043e3cf5f60c79041a662f4ef3516383f7"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Item Configuration for Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4340443927.html).

Revenue recognition templates are used to generate revenue recognition schedules for items sold, based on the association of templates with items.

You can associate a revenue recognition template with the following item types:

-   Assembly
    
-   Serialized Assembly
    
-   Lot Numbered Assembly
    
-   Kit/Package
    
-   Inventory
    
-   Serialized Inventory
    
-   Lot Numbered Inventory
    
-   Non-Inventory for Sale/Resale
    
-   Other Charge for Sale/Resale
    
-   Service for Sale/Resale
    

You can associate a revenue recognition template with an item on the item record to make it the default on all transactions. When the item is entered on a sales transaction, the associated template appears on the transaction line automatically. This default can be edited as necessary for specific transactions. See [Setting a Revenue Recognition Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687732.html).

You don't have to designate a revenue recognition template on an item record. If a deferred revenue account is designated on an item record, you can select a revenue recognition template for the item when it's entered on each sales transaction. See [Setting a Revenue Recognition Template on a Transaction Item Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688475.html).

You can set the default for an item so that Hold Revenue Recognition is automatically checked when the item is added to a transaction. See [Delaying Revenue Recognition for an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688873.html).

When you enter a transaction, the following occurs for any item associated with a revenue recognition template:

-   **Revenue is deferred** - The revenue amount is posted to a deferred revenue account.
    
-   **A revenue recognition schedule is created** - Revenue amounts are scheduled to be recognized across periods based on the terms defined by the template.
    

If you want to defer revenue for sales of discount and markup items, you should use non-posting discount and markup items. See [Deferring Revenue for Discount and Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688734.html).

Important:

To apply a revenue recognition template to an item, you must associate a deferred revenue account with that item on its item record. When Revenue Recognition is enabled, NetSuite automatically adds a default account with a type of Deferred Revenue to the Chart of Accounts because at least one account of this type is required for the feature. You can create additional Deferred Revenue type accounts as needed.

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html)
-   [Revenue Recognition Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1695172.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
