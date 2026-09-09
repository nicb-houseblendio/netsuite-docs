---
id: "section_N1253848"
type: "section"
title: "Applying Billing Schedules"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Applying Billing Schedules"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html"
anchors: ["bridgehead_N1253877", "procedure_N1253954", "bridgehead_N1254036", "procedure_N1254050", "bridgehead_4024118935", "bridgehead_N1254141", "procedure_N1254179", "procedure_N1254288"]
sha256: "b74bcbda6aac8e378e7115c9d687176c9ec9b1ac692db1c4b616be10f02684d6"
---

The Advanced Billing feature enables you to create billing schedules that you apply to sales orders or to line items on sales orders. When you apply a billing schedule, the order is billed in according to that schedule.

Note:

By default, billing schedules are applied to each line individually, not the subtotal, unless you use the Apply to Subtotal option.

## Assigning a Default Billing Schedule to an Item {#bridgehead_N1253877}

You can assign a billing schedule on an item record. Then, when the item is chosen on sales transactions, the billing schedule is applied by default. You can change default billing schedules on individual transactions.

Note:

The billing schedule shows on line items only if forms are customized to show schedules on lines. Read [Assigning a Billing Schedule to a Line Item](#bridgehead_N1254141).

You can assign billing schedules to the following item records:

-   Inventory (including matrix and serialized)
    
-   Assembly (including serialized)
    
-   Kit/Package
    
-   Non-Inventory (for sale and resale)
    
-   Other Charge (for sale and resale)
    
-   Service (for sale and resale)
    

#### To assign a billing schedule to a new item record: {#procedure_N1253954}

1.  Go to _Lists > Accounting > Items > New_ > New.
    
2.  Click the item type you want to create.
    
3.  On the item record, enter information in the necessary fields.
    
4.  On the **Sales / Pricing** subtab under Sales in the **Billing Schedule** field, select the billing schedule you want to associate with this item.
    
5.  Click **Save**.
    

To apply a billing schedule to an existing item, go to _List > Accounting > Items_, click **Edit** next to the item, and make your changes.

## Assigning a Billing Schedule to a Transaction {#bridgehead_N1254036}

You can apply a billing schedule to an entire transaction.

#### To apply a billing schedule to a new sales order: {#procedure_N1254050}

1.  Go to _Transactions > Sales > Enter Sales Orders_.
    
2.  In the **Start Date** field, enter the date the first invoice is to be created.
    
    If you leave this field blank, the first billing date defaults to the sales order date.
    
3.  Choose a customer in the **Customer** field.
    
4.  On the **Billing** subtab, in the **Billing Schedule** field, choose a billing schedule for all items on this order.
    
    To enter a new billing schedule, click **New**.
    
5.  Fill in other fields as necessary.
    
6.  Click **Save**.
    

To apply a billing schedule to an existing sales order, go to _Transactions > Sales > Enter Sales Orders_ > List, click **Edit** next to the sales order, and make your changes.

## Assigning a Billing Schedule to an Invoice Subtotal {#bridgehead_4024118935}

To create a fixed amount billing schedule for an invoice subtotal, set the sales order Type to Standard and the Recurrence Frequency to Custom. Check the **Apply to Subtotal** box and enter a schedule of fixed currency amounts based on the pre-tax, pre-discount invoice total.

For example, suppose you have an invoice with three transactions with a subtotal of $300. The transactions total $50, $100, and $150, respectively, for a subtotal of $300. The customer wants to pay the invoice in three $100 installments, so define three payments of $100 each, totaling $300.

#### To apply a billing schedule to a transaction subtotal:

1.  Go to Transactions > Sales Order > Enter Sales Order.
    
2.  In the **Start Date** field, enter the first invoice date.
    
    If this field is left blank, the first billing date is the date of the sales order.
    
3.  In the **Customer** field, select a customer.
    
4.  On the **Billing** subtab, in the **Billing Schedule** field, select a billing schedule for the transaction subtotal.
    
    To enter a new billing schedule, click **New**. To create and apply a subtotal billing schedule, set the **Type** field to **Standard** and the **Recurrence Frequency** field to **Custom**, and then check the **Apply to Subtotal** box.
    
5.  Fill in any other required fields.
    
6.  Click **Save**.
    

## Assigning a Billing Schedule to a Line Item {#bridgehead_N1254141}

You can apply a billing schedule to an individual line item on a transaction. To do this, you need to customize the following transaction forms to show line item billing schedules:

-   Sales orders
    
-   Online order forms
    

#### To customize your transaction forms for line-item billing schedules: {#procedure_N1254179}

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  On the Custom Transaction Forms page, click **Customize** next to the transaction form you want to change.
    
3.  In the **Name** field, enter a name for this form. For instance, you could name it Billing Schedule Sales Order.
    
    This name appears in the Custom Form field on transactions.
    
4.  Click the **Sublist Fields** subtab.
    
5.  In the **Show** column, check the box next to **Billing Schedule** to show the billing schedule column when you view the transaction.
    
6.  Click the **Printing Fields** subtab.
    
7.  Click the **Columns** subtab under **Printing Fields**.
    
8.  Check the **Print/Email** box next to **Billing Schedule** to show the billing schedule column when you print or email the transaction.
    
9.  Click **Save**.
    

Now, when you choose this custom form in the Custom Form field on transactions, you can choose a billing schedule for each line item.

#### To apply a billing schedule to a sales order line item: {#procedure_N1254288}

1.  Go to _Transactions > Sales > Enter Sales Orders_.
    
2.  In the **Custom Form** field, select the customized sales order form.
    
3.  In the **Start Date** field, enter the first invoice date.
    
    If you leave this field blank, the first billing date defaults to the sales order date.
    
4.  In the **Customer** field, select a customer.
    
5.  On the **Items** subtab, in the **Items** column, choose an item.
    
    If the item has a billing schedule assigned on the item record, that billing schedule autofills in the Bill. Sched. column. You can choose another billing schedule for that item.
    
6.  Click **Add**.
    
7.  Fill in any other required fields on the form.
    
8.  Click **Save**.
    

### Related Topics

-   [Advanced Billing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html)
-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html)
-   [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html)
-   [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html)
-   [Discount and Markup Items and Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html)
-   [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
