---
id: "chapter_N1701780"
type: "chapter"
title: "Using Revenue Commitments"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments"
parent: "book_N1675734"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1701780.html"
anchors: []
sha256: "d9ace352a79e89bec8f5780808c6f651f2b848f72f70bdfc029ccaea93e1cc7d"
---

Note:

Revenue Commitments is a feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For information about the current feature, see [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

Use revenue commitments when you want to recognize revenue separately from billing. This practice is common in businesses that invoice customers at specific project milestones or when the company meets specific contractual requirements. For example, a construction project contract may specify that you can only bill an invoice to the customer at certain milestones, based on completion of construction phases. However, as the contractor, you may incur expenses before reaching a milestone, and you may be required to recognize revenue as you've completed a portion of the project prior to issuing an invoice.

Without revenue commitments, companies attempt to recognize revenue without invoicing the customer by one of the following methods: creating an invoice and then holding it, creating a reversing journal, or creating an invoice, but deferring the revenue.

The Revenue Commitment transaction separates the billing and revenue recognition functions, letting you recognize revenue and bill customers at different times and to recognize revenue in amounts that differ from the amounts billed to customers. A revenue commitment is a non-posting transaction. It serves as the placeholder for the revenue recognition schedule that generates the posting revenue recognition journal entries.

An unbilled receivable posting occurs when revenue recognition is faster than the billing on a specific sales order. When billing occurs at a faster rate than revenue recognition, deferred revenue is increased. The deferred revenue reclassification process adjusts revenue and deferred revenue balances at the line item level. See [Advanced Revenue Commitments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703735.html) and [Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3752066884.html).

Revenue commitments and revenue commitment reversals can be generated when the sales order or return authorization line item is marked Hold Revenue Recognition. The associated revenue recognition schedules are created with a status of On Hold and are managed in the same way as other revenue recognition schedules. For details, see [Managing Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4029604484.html).

You can't create a stand-alone revenue commitment. All revenue commitments must be generated from, and are therefore linked to, a sales order. Similarly, revenue commitment reversals require a return authorization. At the end of the billing and recognition process, the total amount of revenue recognized and amounts invoiced to a customer must equal the total amount of the sales order. For more information, see [Billing Additional Items on Orders with Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1706812.html).

You can't create a credit memo directly from a sales invoice if the sales order is enabled with revenue commitment. You need to generate a return authorization first and then a revenue commitment reversal and a credit memo. For information about creating revenue commitments and revenue commitment reversals, see [Creating Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707026.html) and [Creating Revenue Commitment Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709562.html).

Because data about revenue commitments appears on revenue reports, such as the Billing and Revenue Summary, most of the fields on invoices also are on revenue commitments. A significant difference is that an invoice creates a customer liability (account receivable), while a revenue commitment creates an unbilled receivable amount. The unbilled receivables account is system generated. You can't define additional accounts.

For information about enabling, setting preferences, and assigning permissions for the Revenue Commitments feature, see [Setting Up the Revenue Commitments Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1702000.html). Note that the Revenue Recognition feature must first be enabled for Revenue Commitments to be available.

For details about transaction fields that are used for revenue commitments, see [Understanding Revenue Commitment Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1708322.html).

For examples of use cases for revenue commitments, see [Revenue Commitment Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710191.html).

### Related Topics

-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)
-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Using Sales Order Revenue Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1750747.html)
-   [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html)
-   [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
