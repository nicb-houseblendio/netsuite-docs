---
id: "section_N1254744"
type: "section"
title: "Billing Customers Using Billing Schedules"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Billing Customers Using Billing Schedules"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html"
anchors: ["bridgehead_N1254780", "bridgehead_N1254976", "procedure_N1254989", "procedure_N1256164"]
sha256: "dac51d6fbfbf3ea856c8585bc35ab927fdbfd10256323415ee444f7170aad8a5"
---

With Advanced Billing, orders associated with a billing schedule generate bills according to that schedule. After bills are scheduled, you can [Create Bills from the Billing Queue](#bridgehead_N1254780) or [Bill Manually](#bridgehead_N1254976).

## Create Bills from the Billing Queue {#bridgehead_N1254780}

When you assign a billing schedule to a sale or line, NetSuite adds a bill to the billing queue at the scheduled intervals. Then, you can generate the bills in the billing queue.

For more information, read [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html).

Note:

Use the Bill Sales Orders page for orders with billing schedules and the Invoice Billable Customers page for invoices related to expenses, items, and time.

#### To create bills from the queue:

1.  Go to _Transactions > Sales > Invoice Sales Orders_.
    
2.  Filter the list by selecting a customer to show only their transactions.
    
    Select **All** to display all transactions without filtering.
    
3.  Select the period for posting this transaction.
    
    You can't post to a closed period.
    
4.  NetSuite defaults to today's date for the transaction date. You can enter or select a different date if needed.
    
5.  In the **Next Bill On or Before** field, enter a date to filter the fulfillment list.
    
6.  Choose whether you want to print or email the form.
    
7.  Choose an Accounts Receivable account. The payment will post to this account when the bill is paid.
    
8.  Check this box if you've already processed credit card charges for these transactions outside NetSuite.
    
    Note:
    
    If you check this box and submit, NetSuite automatically marks the Credit Card Approved box and sets the Account field on bills you're processing.
    
9.  Check the **Hide Unfulfilled Orders** box to filter the list to show only fulfilled orders.
    
    Note:
    
    This field is visible only if the Invoice in Advance of Fulfillment preference is enabled.
    
    Important:
    
    If you've enabled Invoice in Advance of Fulfillment and Advanced Shipping, and you check this box, sales orders with billable items will appear in the Sales Orders reminder and the Sales Orders to Bill list.
    
10.  To scan in transaction bar codes, click the **Select Order Number** field.
     
     Note:
     
     To scan in bar codes, you must select **All** in the entity field.
     
11.  To select the orders you want to bill, check the boxes in the **Invoice** column.
     
12.  Click **Submit**.
     
     The system creates bills for the selected transactions.
     

## Bill Manually {#bridgehead_N1254976}

For orders that have billings outstanding, you can create the remaining invoices manually. You can either create the next scheduled invoice or invoice the entire remaining balance.

After an invoice is created, you can print, email or fax it to your customer.

#### To create remaining invoices manually: {#procedure_N1254989}

1.  Go to _Transactions > Sales > Enter Sales Orders > List_ > List.
    
2.  On the **Sales Orders** page, click the date next to the order you want to invoice.
    
3.  On the sales order:
    
    -   Click the **Next Bill** button to create the next schedlued invoice, then click **Save**.
        
    -   Click the **Bill Remaining** button to invoice the remaining balance and override the billing schedule, then click **Save**.
        

#### To send the invoice to the customer: {#procedure_N1256164}

1.  Go to _Transactions > Sales > Create Invoices > List_.
    
2.  On the **Invoice** list, click the date next to the invoice.
    
3.  On the invoice:
    
    -   Click **Save & Print** to print the invoice.
        
    -   Click **Save & Email** to email the invoice.
        
    -   Click **Save & Fax** to fax the invoice.
        

### Related Topics

-   [Advanced Billing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html)
-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html)
-   [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html)
-   [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html)
-   [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html)
-   [Discount and Markup Items and Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
