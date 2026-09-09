---
id: "section_N1216500"
type: "section"
title: "Creating Sales Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Sales Orders > Creating Sales Orders"
parent: "chapter_N1215966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html"
anchors: ["subsect_0211012332", "subsect_0211012524", "bridgehead_4593540360", "bridgehead_4593543124"]
sha256: "610d79daccbd6e9b664db33b6c38c9494c000e5084fe9d2a485246e7ff21a5f9"
---

Enter sales orders to record items and services that you promise to customers. You can fulfill sales orders to track delivered and pending items and services. Sales orders don't affect your general ledger.

For information specific to Not-for-Profit (NFP), see [Pledge and Donation Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519955881.html).

NetSuite offers several types of predefined sales order forms. You or an administrator can also create customized sales order forms.

-   **Standard Sales Order** - A standard sales order lets you create an invoice or a cash sale, based on whether you enter billing terms or a payment method. See [The Standard Sales Order Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218600.html) for more information.
    
-   **Standard Sales Order - Cash Sale** - When you bill this type of sales order, NetSuite creates a cash sale transaction.
    
-   **Standard Sales Order - Invoice** - When you bill this type of sales order, NetSuite creates an invoice.
    
-   **Standard Sales Order - Progress Billing** - You can bill progress sales orders at intervals according to the fulfillment progress of the goods or services. See [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html) for more information.
    

If you enable and configure the **Automatic Location Assignment** feature, NetSuite automatically assigns a location to each sales order line. Assignments depend on available inventory and feature configuration. For more information, see [Order Fulfillment Automation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4440622374.html). To enter a sales order with automatic location assignment, see [Assigning Locations Automatically in a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4558169323.html).

## Choosing a Fulfillment Location {#subsect_0211012332}

You can choose a fulfillment location for each item in the Location column on a sales order line.

If you use the **Intercompany Cross-Subsidiary Fulfillment** feature, there's a change:

-   Instead of the Location column, use the **Inventory Location** column on each sales order line.
    
-   The Inventory Location column lets you select locations from the customer's subsidiary. This column also lets you select locations from any other subsidiaries that have a global inventory relationship with the transaction subsidiary.
    

For details, see [Intercompany Cross-Subsidiary Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515621767.html).

## Splitting an Order for Payment {#subsect_0211012524}

To split an order for payment, you have two options:

-   Create two separate invoices.
    
-   Make a copy of the transaction, then remove unwanted lines from both the original and the copy.
    

## Creating a Sales Order {#bridgehead_4593540360}

Entering a sales order with the standard sales order form lets you create a basic sales order, which can then be billed as an invoice or a cash sale. The minimum information you need to enter on a sales order is:

-   **Customer** - Who you're selling to. If you use the Projects feature, you can select a project or job.
    
-   **Date** - The transaction date (defaults to today).
    
-   **Status** - Where the order is in the fulfillment process. The sales order status can be either Pending Approval or Pending Fulfillment.
    
-   **Items** - Add at least one item in the Items tab.
    

For information about additional fields in the sales order header, see [Sales Order Header Fields](#bridgehead_4593543124).

#### To create a standard sales order:

1.  Go to _Opportunities > Transactions > Sales Orders > New_.
    
2.  In the **Custom Form** field, select **Standard Sales Order**.
    
    The standard sales order form is the default. For more information about how this form works, see [The Standard Sales Order Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218600.html).
    
3.  In the **Customer** field, select a customer.
    
    If you use the Projects feature, you can select a project or job.
    
    Note:
    
    If you add, edit, or delete a project after a sales order is billed:
    
    -   the sales order becomes a standalone sales order and is no longer associated with the invoice
        
    -   the invoice is removed from the Related Records subtab on the sales order
        
    
4.  Enter a date for the transaction. The current date is entered by default.
    
5.  Select the status of the transaction. Your company's accounting preferences determine the default status.
    
6.  In the **Items** subtab, add items to the sales order.
    
    To add an item, select it in the Item column, enter the quantity, and then click **Add**. You can enter additional details for each line item such as an inventory commitment setting, order priority, or expected ship date. See [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html) for more information.
    
7.  Enter additional information as necessary. You can enter general information in the sales order header. You can also enter information related to shipping, billing, payments, accounting, relationships, and communication:
    
    -   [Sales Order Header Fields](#bridgehead_4593543124)
        
    -   [Entering Shipping Information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4593450742.html)
        
    -   [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html)
        
    -   [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html)
        
    -   [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html)
        
    -   [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)
        
    -   [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html)
        
    -   [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html)
        
8.  Click **Save**. You can also do one of the following:
    
    -   Click **Save & Print** to save and print the form.
        
    -   Click **Save & Email** to save the form and email it.
        
    -   Click **Save and Fulfill** to save the information and immediately open a fulfillment form for this order.
        

Note:

The Save and Fulfill button shows on new sales orders only. It doesn't show when you edit an existing order. To edit an existing sales order, see [Editing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_8114418642.html).

## Sales Order Header Fields {#bridgehead_4593543124}

The sales order header fields let you add more details about a sales order transaction. You can enter general, sales, and classification information for reporting. The available fields may vary based on your company's enabled features. The standard sales order form fields are listed in the following table.

| Field | What It's For |
| --- | --- |
| **Primary Information** |
| End Date | When the sales order expires. |
| PO Number | The customer's purchase order number. |
| Memo | A note about the sales order. The memo appears on some sales order reports. You can also search for keywords in the **Memo** field using Search Transactions. |
| Start Date | When the first invoice is generated. The Advanced Billing feature must be enabled to create an invoice based on the start date. |
| **Sales Information** |
| Exclude Commissions | Check this box to skip commission calculations for this sales order and its sub-transactions. |
| Lead Source | Where the lead came from. |
| Opportunity | The related opportunity. This field appears only when the Opportunities feature is enabled. |
| Partner | The associated partner. If you use the Multi-Partner Management feature, you can associate partners with this transaction on the **Relationships** subtab. |
| Sales Effective Date | The date that determines the commission plan and sales team. |
| Sales Rep. | The sales representative assigned to the sales order. If you use the Team Selling feature, you can set this on the **Sales Team** subtab. |
| **Classification** |
| (OneWorld) Subsidiary | Defaults to the customer's primary subsidiary, unless its shared with multiple subsidiaries. If the customer record is shared with multiple subsidiaries, choose the subsidiary by which to classify the sales order. |
| Class | How to classify the sales order. |
| Department | The department to classify the sales order under. |
| Location | Where to classify the sales order. |

### Related Topics

-   [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html)
-   [Sales Order Entry Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216314.html)
-   [The Standard Sales Order Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218600.html)
-   [Approving Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218788.html)
-   [Closing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698204292.html)
-   [Reopening a Closed Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161133765436.html)
-   [Invoicing Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1219162.html)
-   [Viewing the Status of Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1220604.html)
-   [Printing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221008.html)
-   [Creating Invoices or Cash Sales from Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221414.html)
-   [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html)
-   [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html)
-   [Applying a Promotion on a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160312998339.html)
-   [Applying a Discount on a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160312998983.html)
-   [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html)
-   [Assigning Locations Automatically in a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4558169323.html)
-   [Getting Credit Card Authorization Automatically on Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218323.html)
-   [Creating Store Pickup Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4835438208.html)
-   [Customer Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_4738412727.html)
-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
