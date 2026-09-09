---
id: "section_N1221414"
type: "section"
title: "Creating Invoices or Cash Sales from Sales Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Sales Orders > Creating Invoices or Cash Sales from Sales Orders"
parent: "chapter_N1215966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221414.html"
anchors: ["subsect_1124012829", "procedure_0617033248"]
sha256: "bfe76f0cebf7c1be1b4ff4ccc3a29c1bb71b9d3fd873019bc6bc72b2702bdd2d"
---

A sales order is a promise to deliver goods or services. Sales orders don't affect your accounts until you deliver the goods and create an invoice or cash sale.

A cash sale when you sell something and get paid right away. An invoice is when you sell something but don't get paid right away.

Note:

The type of sales order form you used determines whether you create an invoice or cash sale. The cash sale form creates a cash sale, and the invoice form creates an invoice.

The process for creating an invoice or cash sale depends on whether you've enabled the Advanced Shipping feature.

-   **Without Advanced Shipping**, you use one process to fulfill and bill sales orders. When you fulfill an order, it automatically creates an invoice or cash sale.
    
-   **With advanced shipping**, you have separate processes for fulfilling sales orders and creating invoices or cash sales. For more information about advanced shipping, read [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html).
    

If you use the Multiple Currencies feature, NetSuite uses the sales order's currency for the new transaction. For more information, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).

You can fulfill a single sales order or multiple sales orders.

## Error Messages {#subsect_1124012829}

When creating an invoice or cash sale from a sales order, you'll see an error message if:

-   Two users try to bill the same order at the same time.
    
-   One user tries to bill an individual order during the time that another user is bulk billing orders.
    
    (If the individual instance is processed before the bulk instance, the bulk processing status displays an error requesting an item to be selected for the transaction.)
    
-   A user accidentally double-clicks the Save button and submits two requests.
    

If this happens, you'll see an error message saying the transaction has already been processed.

Note:

This error does not show in the following circumstances:

-   If you're creating an invoice from an opportunity.
    
-   If you're creating a new invoice or cash sale.
    
-   If you're editing an existing invoice or cash sale.
    
-   If you make a copy of an invoice and then save it again.
    

#### To create an invoice or cash sale from a single sales order:

1.  Go to _Transactions > Sales > Fulfill Orders (Administrator)_.
    
2.  On the Fulfill Orders page, select the customer.
    
3.  From the **Bulk Fulfill From Location** list, select the location to be used to fulfill the order, or select **New** to enter a new location.
    
4.  In the **Process** column, click **Fulfill** next to the sales order.
    
5.  Click **Save**.
    
    The selected sales order appears as an invoice or cash sale.
    
6.  Make any changes you need to the invoice or cash sale.
    
    Note:
    
    To generate deferred revenue for billable time, you need to manually select revenue recognition schedules on the **Billable Time** subtab located on the **Items** subtab.
    
7.  Click **Save**.
    
    NetSuite creates an invoice or cash sale for the sales order.
    

To accept a customer payment for the invoice, go to _Transactions > Customers > Accept Customer Payments (Administrator)_.

Note:

You can't include a partially processed sales order when fulfilling multiple orders. Partially processed sales orders must be fulfilled individually.

#### To create invoices or cash sales from multiple sales orders:

1.  Go to _Transactions > Sales > Fulfill Orders (Administrator)_.
    
2.  On the Fulfill Orders page, select the customer, or select **All** to list all open sales orders.
    
3.  From the **Bulk Fulfill From Location** list, select the location to be used to fulfill the order, or select **New** to enter a new location.
    
4.  In the **Fulfill** column, check the boxes next to the sales orders you want to fulfill.
    
5.  Click **Submit**.
    
    The Processed Orders list appears. It lists the transactions created when the sales orders are fulfilled.
    

#### To edit the transactions created from the Processed Orders list: {#procedure_0617033248}

1.  In the Processed Number column, click the number next to the transaction you want to edit.
    
2.  When the transaction appears, click **Edit**.
    
3.  Make any changes, and click **Save**.
    

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
-   [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html)
-   [Using Consolidated Billing for Projects and for Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233909.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
