---
id: "section_N1725637"
type: "section"
title: "Billing a VSOE Transaction"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Billing a VSOE Transaction"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html"
anchors: []
sha256: "38577712f699ec09cda84f0a7d305d8311a69fc34872efd9e44f5c7b50bbb621"
---

Important:

After a vendor-specific objective evidence (VSOE) bundle is invoiced, the allocation amount can't change. For example, you enter a sales order with three items. Only two of the items are marked delivered for VSOE and are eligible to have their allocated value recognized. After invoicing the sales order, you mark the third item delivered for VSOE. Marking the item delivered after invoicing doesn't impact the VSOE allocation. None of the VSOE settings impact the VSOE allocation after the order has been invoiced. Only the delivered flag may be checked after invoicing to start the revenue recognition process.

After values are allocated and billed to the customer, the VSOE allocation won't change. The delivery status at the time of billing and subsequent updates determine when the revenue recognition schedule is created and revenue is recognized.

In this example, you bill a sales order marked Is VSOE Bundle. The order includes the following:

| Item | Invoice price | VSOE Price | VSOE Allocation | Delivered? | Deferral |
| --- | --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | $1000 | No | Defer Until Item Delivered |
| Software Product 101 | $1500 | $2000 | $2000 | Yes | Defer Until Item Delivered |
| Software Product 103 | $2500 | $2500 | $2500 | Yes | Defer Until Item Delivered |
| Total | $5500 | $5500 | $5500 |  |  |

NetSuite doesn't create the revenue recognition schedule for the Installation Service 202 item at the time of billing because it's not delivered. When Installation Service 202 is marked Delivered, the revenue recognition schedule is created.

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
