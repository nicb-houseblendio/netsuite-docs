---
id: "section_N1773475"
type: "section"
title: "Configuration for Amortization"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Configuration for Amortization"
parent: "section_N1767815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html"
anchors: []
sha256: "63fd9c9a010d893271fbb8abdfb47f4507144f3bfa69d2e6f9dfb11101764e21"
---

Amortization templates can be used to generate amortization schedules for items purchased based on the association of templates with items.

You can associate an amortization template with the following item types:

-   Non-Inventory for Purchase/Resale
    
-   Other Charge for Purchase/Resale
    
-   Service for Purchase/Resale
    

You can associate an amortization template with an item on the item record to make it the default on all transactions. When the item is entered on a purchase transaction, the associated template autofills on the transaction line. The template can be changed as needed for specific transactions. See [Setting an Amortization Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773719.html).

Amortization is supported for the following types of transactions:

-   **Vendor Bill** - Item lines on a bill can use the default amortization templates from item records, or you can select templates on the bill transaction. See [Setting an Amortization Template on a Vendor Bill Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773966.html).
    
-   **Vendor Credit** - Item lines on a credit can use the default amortization templates from item records or can inherit the amortization templates from the bill that generates the credit. You can also select templates on the credit transaction. [Setting an Amortization Template on a Vendor Credit Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html).
    

To amortize the costs of an item, a deferral account must be specified on the item record or amortization template record. If both records have deferral accounts, the template's deferral account is used. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).

When you enter a transaction, the following occurs for any item associated with an amortization template:

-   **Expenses are deferred** - The expense amount is posted to a deferred expense account, not to a standard expense account.
    
-   **An amortization schedule is created** - Expense amounts are scheduled to be recognized across periods based on the terms defined by the template.
    

Important:

A deferred expense account must be specified for amortization to be supported. Deferral accounts can be specified in item records, amortization templates, and expense account records. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).

### Related Topics

-   [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html)
-   [Amortization Template Term Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html)
-   [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html)
-   [Associating Amortization Templates with Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
