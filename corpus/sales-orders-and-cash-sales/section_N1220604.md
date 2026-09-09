---
id: "section_N1220604"
type: "section"
title: "Viewing the Status of Sales Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Sales Orders > Viewing the Status of Sales Orders"
parent: "chapter_N1215966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1220604.html"
anchors: []
sha256: "a1235fe95dc19792c74f11cdb0c38c5380452cb049938533cbe347b9cb4a62be"
---

With advanced shipping, your shipping and accounting teams work separately to fulfill and bill orders. You can fulfill all or part of sales orders separately from invoices. Your sales orders have statuses that show where they are in the fulfilling and billing process. The system sets these statuses, and you can't change them manually.

To enable the Advanced Shipping feature, an administrator can go to _Setup > Company > Enable Features (Administrator)_. On the Transactions subtab, check **Advanced Shipping**, and then click **Save**.

#### To view the status of a sales order:

1.  Go to _Opportunities > Transactions > Sales Orders_.
    
2.  You'll see the status of each sales order in the **Status** column.
    

Here are the possible statuses:

-   Without Advanced Shipping:
    
    -   **Closed** - The sales order is closed and won't be fulfilled or billed.
        
    -   **Pending Approval** - The sales order hasn't been approved yet.
        
    -   **Pending Fulfillment** - The order is waiting for an invoice or cash sale to be created.
        
    -   **Partially Fulfilled** - The order is partially shipped.
        
    -   **Fulfilled** - The order is fully shipped and billed
        
    -   **Canceled** - The sales order has been canceled. Canceled is a terminal status and cannot be undone. You must copy or recreate the sales order if it's needed again.
        
-   With Advanced Shipping:
    
    -   **Closed** - The sales order is closed and won't be fulfilled or billed.
        
    -   **Pending Approval** - The sales order hasn't been approved yet.
        
    -   **Pending Fulfillment** - The sales order is approved and pending shipment of items ordered.
        
    -   **Partially Fulfilled** - The sales order is partially shipped, regardless of billing status.
        
    -   **Pending Billing** - The sales order is waiting for an invoice or cash sale to be created, including partially billed sales orders.
        
    -   **Pending Billing/Partially Fulfilled** - The sales order is approved and partially fulfilled. Billing occurs when an invoice or sales order is created.
        
    -   **Billed** - The sales order is completely shipped and an invoice has been created.
        
    -   **Canceled** - The sales order has been canceled by clicking Cancel Order. Canceled is a terminal status and cannot be undone. You must copy or recreate the sales order if it's needed again.
        

On the sales orders page, next to the sales order, click **View**. You can click **Edit** next to a sales order to make changes to the order.

To see what's already been fulfilled and invoiced for a sales order, go to a sales order and click the **Items** subtab. The Fulfilled and Invoiced columns show the quantity fulfilled and invoiced for each line item.

### Related Topics

-   [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html)
-   [Sales Order Entry Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216314.html)
-   [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html)
-   [The Standard Sales Order Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218600.html)
-   [Approving Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218788.html)
-   [Closing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698204292.html)
-   [Reopening a Closed Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161133765436.html)
-   [Invoicing Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1219162.html)
-   [Viewing the Status of Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1220604.html)
-   [Printing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221008.html)
-   [Creating Invoices or Cash Sales from Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221414.html)
-   [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
