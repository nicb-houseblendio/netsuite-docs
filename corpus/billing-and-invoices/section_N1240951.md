---
id: "section_N1240951"
type: "section"
title: "Billing or Invoicing a Sales Order"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Billing or Invoicing a Sales Order"
parent: "section_N1235134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html"
anchors: []
sha256: "9c70324f7a55d71bd0b3b7f3a46562d6062a10ce1597e08a46cde5fcd87369a0"
---

Billing a sales order creates a record of debt owed to you by your customer for a sale. When you bill a sales order, your accounts receivable ledger increases by the amount of the bill.

Usually, you bill customers for a sale when you ship the items on the order. The process for billing your customers depends on whether you use the Advanced Shipping feature:

-   **Without Advanced Shipping** - You use a single transaction to fulfill and bill sales orders at the same time. Fulfilling a sales order automatically creates a bill based on the fulfillment. You can partially fulfill a sales order and any items fulfilled will also be billed.
    
-   **With Advanced Shipping** - You use separate transactions to fulfill and bill sales orders. First, you fulfill the sales order to indicate the items are being shipped. Next, you create a bill for the shipped items. Even if you ship only part of an order, you can still create an invoice or cash sale for the entire order.
    
    To bill orders, fulfill part or all of a sales order, and then create an invoice or cash sale for the shipped items and rendered services. You can bill a single sales order or multiple sales orders.
    
    You can't include a partially processed sales order when bulk billing orders. Partially processed sales orders need to be billed individually.
    

Note:

You can't fulfill or bill sales orders with the status Pending Approval. If you need to make changes to an order that's pending approval, you can remove line items.

Lines from both a vendor bill and any related bill credit appear on the Billable Items list located on the Items subtab.

To convert a sales order to an invoice or cash sale, go to _Transactions > Sales > Bill Sales Orders_.

If you ship only part of an order, you can ship and create an invoice or cash sale for the rest of the order later.

After billing a sales order, you can view the Items subtab of the order and the Invoiced column, which shows how many of each item you've billed.

To enable Advanced Shipping, go to _Setup > Company > Setup Tasks > Enable Features > Transactions_ > Transactions (Administrator). Check the **Advanced Shipping** box, and click **Save**.

To turn off Advanced Shipping, go to _Setup > Company > Setup Tasks > Enable Features > Transactions_ > Transactions (Administrator). Clear the **Advanced Shipping** box, and click **Save**.

Note:

After you enable Advanced Shipping, you can't turn it off unless all fulfilled sales orders are billed.

You can also use the Advanced Shipping feature with the Advanced Billing feature. For more information, read [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html).

### Related Topics

-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Using the Billing Tab and Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4483926245.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4063198073.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)
-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Displaying Deposit Balance on Customer Statements and Remittance Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4204723346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
