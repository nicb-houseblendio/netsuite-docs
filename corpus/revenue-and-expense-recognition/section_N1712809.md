---
id: "section_N1712809"
type: "section"
title: "Revenue Commitment with One-Time Revenue Item Example"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Revenue Commitment Examples > Revenue Commitment with One-Time Revenue Item Example"
parent: "section_N1710191"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1712809.html"
anchors: []
sha256: "c65fe1911fa44cadd2256dbf31b2c5c59ef99141598d6b36c0dda53700c33754"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

This simplified example shows how revenue is recognized when you add an item to an invoice created for a sales order with a revenue commitment.

In this scenario, a text messaging company offers its customers the following service:

-   Basic text messaging services - 1 year contract ($120) that covers 250 messages a month.
    

The billing and revenue recognition for the contract is as follows:

-   Basic text messaging service is billed monthly at $10.
    
-   Revenue recognition schedule is a 12 month, even period schedule.
    
-   Rev Rec on Rev Commit. box is checked on the sales order.
    

| Item | Sales Price per One Year Contract | Revenue Recognition Schedule |
| --- | --- | --- |
| Basic Text Messaging Service | $120 | 12 month |

In one month, the text message usage for a customer exceeds the 250 message limit specified in the contract, triggering an additional, one-time charge of $5.00.

| Item | Source | Sales Price | Invoice Amount | Revenue Recognized |
| --- | --- | --- | --- | --- |
| Basic Text Messaging Service | Sales order | $120 / 12 months | $10 | Per Revenue Recognition Schedule |
| Overage Fee | Invoice | $5 | $5 | Fully recognized when billed |

The income for the Overage Fee is fully recognized upon saving the invoice. The revenue commitment and revenue recognition schedule don't apply to any item lines added directly to the invoice. The G/L impact for the monthly invoice created for this example is as follows:

| Account | Debit | Credit |
| --- | --- | --- |
| Accounts Receivable | 15 |  |
| Revenue |  | 5 |
| Deferred Revenue |  | 10 |

For more information, see [Billing Additional Items on Orders with Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1706812.html).

### Related Topics

-   [Revenue Commitment Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710191.html)
-   [Base Currency Transaction Without Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811804072.html)
-   [Base Currency Transaction with Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811804909.html)
-   [Foreign Currency Transaction with Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811805482.html)
-   [VSOE with Foreign Currency Revenue Commitment Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710377.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
