---
id: "section_N1219162"
type: "section"
title: "Invoicing Sales Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Sales Orders > Invoicing Sales Orders"
parent: "chapter_N1215966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1219162.html"
anchors: ["subsect_0403012039", "subsect_1124013032"]
sha256: "dd043e2ad5bac3720e92a31d854d8148866d02dac03a95706070411981997627"
---

Invoicing a sales order, or billing, converts an approved sales order into an invoice or cash sale.

When you invoice sales orders, NetSuite uses standard forms by default.

Note:

If you use custom sales orders, you'll also need to create custom invoices and cash sales.

#### To invoice sales orders:

1.  Go to _Transactions > Sales > Invoice Sales Orders (Administrator)_.
    
2.  To filter the list of billable orders:
    
    -   Select a customer to see their orders, or select All to see all orders.
        
    -   In the **Next Bill On Or Before** field, to filter by billing date, enter a date.
        
3.  Set basic billing information for the orders you want to invoice:
    
    1.  In the **Posting Period** field, select the accounting period to which you want to post the transaction.
        
        Note:
        
        You can't post to a closed period.
        
    2.  In the **Date** field, enter the billing date (default is today's date).
        
    3.  In the **To Be Printed** field:
        
        -   To print the form, select **Yes**.
            
        -   If you don't want to print, select **No**.
            
        -   To follow the customer's default printing preference, select **Respect Customer Preference**. Set this preference on the Info subtab of the customer record in the **Send Transactions By** field.
            
    4.  In the **To Be Emailed** field:
        
        -   Select **Yes** to email this form.
            
        -   Select **No** if you don't want to email.
            
        -   Select **Respect Customer Preference** to send email based on the default preference on the customer record. Set this preference on the Info subtab of the customer record in the **Send Transactions By** field.
            
    5.  If the transactions you select have already had credit card charges performed outside NetSuite (such as by a card-swipe terminal) check the **Credit Card Approved** box.
        
        Note:
        
        If you check this box and submit this transaction, NetSuite automatically checks the **Credit Card Approved** box and sets the Account field on Cash Sales you process.
        
    
    Note:
    
    You can also set the billing information for other fields in the transaction. For more information, see [Bulk Update Fields](#subsect_1124013032).
    
4.  In the **Invoice** column, check the box for each the sales orders you want to bill.
    
    The **Order Type** column shows whether the sales order becomes an invoice or a cash sale. Whether you create an invoice or cash sale for the sales orders depends on the form you originally used to enter the orders. The cash sale form generates a cash sale and the invoice form generates an invoice.
    
5.  Important:
    
    In this step, the selected sales orders enter the processing queue and are billed with the data you selected or entered.
    
    Click **Submit** to create the invoice or cash sale.
    
    The Process Status page displays with the status of the sales orders submitted for billing. To view updates to the status, click **Refresh**.
    
6.  (Optional) If you converted the sales order to an invoice, go to _Transactions > Customers > Accept Customer Payments (Administrator)_ to apply a payment to the open invoice.
    
7.  (Optional) If you converted the sales order to a cash sale, you can choose to place the payment into Undeposited Funds or directly into a bank account. If you select Undeposited Funds, after the payment is approved, click **Make Deposits** to deposit the money from Undeposited Funds into a bank account.
    

## Invoicing Sales Orders with Advanced Shipping {#subsect_0403012039}

If you use advanced shipping, you can:

-   track sales orders separately from invoices
    
-   create invoices for a whole order even if the order has not been completely fulfilled
    

#### To use advanced shipping:

1.  Go to _Setup > Company > Enable Features (Administrator)_.
    
2.  Click the **Transactions** subtab.
    
3.  Check the **Advanced Shipping** box.
    
4.  Click **Save**.
    

#### To create invoices for an order that has not been completely fulfilled:

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_.
    
2.  Click the **Order Management** subtab.
    
3.  Check the **Invoice in Advance of Fulfillment** box.
    
4.  Click **Save**.
    

## Bulk Update Fields {#subsect_1124013032}

On the bulk billing page, you'll find a Set Fields subtab for updating orders.

For example, you might want to add a memo to all orders, like 'Q1 Rush processing.' You can add the memo text on the Set Fields subtab, and it will be applied to all processed orders.

#### To update fields in bulk:

1.  Go to _Transactions > Sales > Invoice Sales Orders (Administrator)_.
    
2.  Click the **Set Fields** subtab to choose the fields to update and select the data for entry.
    
3.  In the **Field** column, choose a field to update.
    
4.  Depending on the field you select, data is entered in one of the following fields:
    
    -   In the **Selection** column, choose a setting for the field.
        
    -   In the **Checked** column, define whether a box is checked or cleared.
        
    -   In the **Text** column, enter text for the chosen field.
        
    -   In the **Date** column, choose a date for the chosen field.
        
5.  Click **Add**.
    
6.  Repeat these steps for each field you want to update.
    
7.  Complete other fields on the billing form as necessary.
    
8.  Click **Submit**.
    

After submitting, the invoices are generated and the fields updated as specified.

Note:

Only header fields can be updated during bulk fulfillment or invoicing.

### Related Topics

-   [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html)
-   [Sales Order Entry Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216314.html)
-   [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html)
-   [The Standard Sales Order Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218600.html)
-   [Approving Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218788.html)
-   [Closing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698204292.html)
-   [Reopening a Closed Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161133765436.html)
-   [Viewing the Status of Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1220604.html)
-   [Printing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221008.html)
-   [Creating Invoices or Cash Sales from Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221414.html)
-   [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html)
-   [Closing Line Items on Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1220357.html)
-   [Invoicing Individual Line Items on Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0518111425.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
