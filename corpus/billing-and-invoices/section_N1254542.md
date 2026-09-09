---
id: "section_N1254542"
type: "section"
title: "Discount and Markup Items and Billing Schedules"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Discount and Markup Items and Billing Schedules"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html"
anchors: []
sha256: "14d26a8c97148f5df5eccadf7f0e734c698d47f30fb896918eb2511578293d11"
---

You can't assign billing schedules to discount or markup items, but you can include them on orders with a billing schedule. Here's how discounts and markups are applied to sales:

-   When you include a percentage discount item on a sales order with a billing schedule, the discount is applied to each billing instance.
    
    For instance, suppose an item costs $100 and is invoiced in two $50 billings. The sales order includes a 10% discount item. The first invoice totals $45 ($50 minus the 10% discount). The second invoice is also $45 ($50 minus the 10% discount). The total billing amount for the order is $90 ($100 minus the 10% discount).
    
-   When you add a currency amount discount item to a sales order with a billing schedule, the entire discount amount appears on the first invoice by default.
    
    For example, suppose an item costs $100 and is invoiced in two $50 billings. The sales order includes a $20 discount item. The first invoice totals $30 ($50 minus the $20 discount). The second invoice is $50. The total billing amount for the order is $80 ($100 minus the $20 discount).
    
    Note:
    
    This might make the discount amount greater than the billing total on the first invoice. If this happens, you'll need to adjust the discount amount on the first invoice. When you update the discount amount on the invoice, the next invoice will include the remaining discount amount.
    

### Related Topics

-   [Advanced Billing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html)
-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html)
-   [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html)
-   [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html)
-   [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html)
-   [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
