---
id: "section_N1721160"
type: "section"
title: "Updating VSOE Allocations and Delivery Status on a Transaction"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Updating VSOE Allocations and Delivery Status on a Transaction"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html"
anchors: []
sha256: "134b92fe73a00f6e281469cfa96baadcb92a10fc1c78fc70ccbfa8983e493c17"
---

You can click the Update VSOE button on the Accounting subtab to update the vendor-specific objective evidence (VSOE) allocation amount and delivery status on a transaction. VSOE prices can be changed only on transactions you've not yet billed. After billing, you can only change the delivery status.

For example, an order that you've not yet billed has only some items marked delivered. You can view the order and click Update VSOE to update the delivery status of the appropriate items. NetSuite recalculates the VSOE allocation based on the deferral settings and delivery status of all items on the order. You can also update the allocation amounts if you make your own calculations.

Note:

**Update VSOE** doesn't auto-calculate the allocation regardless of your transaction settings. To auto-calculate allocation, you must edit the transaction to make changes.

For example, a VSOE transaction bundle on an unbilled sales order includes the following:

| Item | Invoice price | VSOE Price | Delivered? | Deferral |
| --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | No | Defer Until Item Delivered |
| Software Product 101 | $1500 | $2000 | Yes | Defer Until Item Delivered |
| Software Product 103 | $2500 | $2500 | Yes | Defer Until Item Delivered |
| Total | $5500 | $5500 |  |  |

As shown, the revenue to be recognized upon invoicing for the sale is $4500. This total is derived from the VSOE prices of items that qualify for revenue recognition. The Installation Service 202 item doesn't qualify for revenue recognition because it's not marked delivered.

When you edit the sales order to mark the Installation Service 202 item as delivered, the allocated revenue for the item can then be recognized.

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
