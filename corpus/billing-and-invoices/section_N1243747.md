---
id: "section_N1243747"
type: "section"
title: "Using Progress Invoicing"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Progress Invoices > Using Progress Invoicing"
parent: "section_N1243687"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243747.html"
anchors: ["procedure_N1243802"]
sha256: "4363c007a444be169da40942c5d016507652d8158b934b6042ee6dc3ebcd0013"
---

Many service businesses use progress billing to bill for portions of projects as they're completed.

With progress billing, you can create and approve a progress sales order. When a portion of the project is done, fulfill the progress sales order. Then, create a progress invoice for a percentage of the total cost.

To create a progress invoice, create a progress sales order first. Without the corresponding sales order, a progress invoice isn't recorded correctly. For more information about creating a progress sales order, read [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html).

If you use advanced shipping, there are separate processes for fulfilling progress sales orders and creating corresponding invoices. For more information about advanced shipping, read [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html).

If you don't use advanced shipping, you use a single process to fulfill and bill progress sales orders. Fulfilling a progress sales order automatically creates an invoice from the sales order.

#### To create an invoice from a progress sales order: {#procedure_N1243802}

1.  Go to _Billing > Sales > Bill Sales Orders_.
    
2.  On the Bill Sales Order page, select the customer you want to create an invoice for.
    
    All open sales orders for that customer appear in a list on the page.
    
3.  In the **Process** column, click **Invoice** next to the progress sales order you want to create an invoice for.
    
4.  Under **Primary Information**, in the **Custom Form** field, select **Standard Progress Invoice**.
    
5.  On the **Item** subtab, enter the percentage being billed in one of two ways:
    
    -   Click the number of the line item you want to change.
        
        In the **Current %** field, enter the percentage of the sales order to be billed for, and click **Add**.
        
    -   Click **Fill %**.
        
        Enter the percentage that all line items are to be billed for, and click **OK**.
        
6.  Click **Save**.
    

When you've completed another portion of this project, repeat these steps to fulfill and invoice the sales order again.

To accept a customer payment for the invoice, go to _Customers > > Accounts Receivable > Accept Customer Payments_.

### Related Topics

-   [Creating Invoices from Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243970.html)
-   [Creating Invoices from Fulfilled Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244143.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
