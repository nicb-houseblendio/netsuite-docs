---
id: "section_N1253492"
type: "section"
title: "Creating Billing Schedules From an Estimate or Sales Order"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Creating Billing Schedules From an Estimate or Sales Order"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html"
anchors: ["procedure_N1253504"]
sha256: "ac3a32466f6589b60bea9b0edbffb30cfe13f269ab1e5e63737ff943beb79e81"
---

You can create a billing schedule when entering an estimate or sales order.

#### To create a billing schedule from an estimate or sales order: {#procedure_N1253504}

1.  Go to one of the following:
    
    -   _Transactions > Sales > Prepare Estimates_
        
    -   _Transactions > Sales > Enter Sales Orders_
        
2.  On the **Billing** subtab, select **New** in the **Billing Schedule** field.
    
3.  Follow the steps in [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html) to create the schedule.
    
4.  A billing schedule created from a transaction can be identified as Public or Private.
    
    -   Private billing schedules are only visible in the transaction they're created from.
        
    -   Public billing schedules are visible on any transaction.
        
    
    By default, billing schedules created from transactions are Private.
    
    To set the status to Public, check the **Public** box.
    
    Note:
    
    Milestone billing schedules cannot be marked public.
    
5.  Click **Save**.
    

If you create a private billing schedule from an estimate, that schedule is attached to items on the resulting sales order. When the sales order is created from the estimate, the private schedule can also be added to new lines you add to the sales order.

Private billing schedules can be made Public, but not the other way around.

You can view the billing schedule list at _Lists > Accounting > Billing Schedules_, and choose to view **Public**, **Private** or **All** schedules in the top of the page in the **Type** field. Each private schedule shows a link to its associated transaction and a link to the billing schedule record.

Note:

Editing a billing schedule doesn't update existing instances on open sales orders.

To update existing instances, go to _Transactions > Sales > Enter Sales Orders > List_ to open the sales order and re-save it. Upon saving, the billing schedules are updated with your changes.

Now, you can apply this billing schedule to sales or items to generate invoices. For more information about applying a billing schedule, read [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html).

### Related Topics

-   [Advanced Billing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html)
-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html)
-   [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html)
-   [Discount and Markup Items and Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html)
-   [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
