---
id: "section_N1226422"
type: "section"
title: "Fulfilling Progress Sales Orders Using Advanced Shipping"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Advanced Shipping > Fulfilling Progress Sales Orders Using Advanced Shipping"
parent: "section_N1224089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226422.html"
anchors: ["procedure_N1226446"]
sha256: "e10778f940741e01ecaf06e198d0751c1199bc8392ba419b4af5477faeffa854"
---

Service businesses often use progress billing to bill for completed project portions.

When using progress billing, a progress sales order is created and approved. After a portion of the job has been completed, the progress sales order is fulfilled. Then, a progress invoice is created for a percentage of the total cost. Progress sales orders must be fulfilled individually.

#### To fulfill a progress sales order using advanced shipping: {#procedure_N1226446}

1.  Go to _Shipping > Shipping > Fulfill Orders_.
    
2.  Select a customer to show only orders for that customer.
    
3.  Select the period these fulfillments are posting to.
    
4.  In the **Filter By** field, choose one of the following to filter the orders shown:
    
    -   **Some Items Committed** - the list shows orders that have one or more items committed to be fulfilled.
        
    -   **All Items Committed** - the list shows orders that have all items committed to be fulfilled.
        
    -   **Respect Ship Complete** - the list shows only the orders that are committed according to their ship complete setting. This includes all orders that are not restricted to ship complete.
        
    -   **Ignore Item Availability** - the list shows all open orders regardless of the availability of items on the orders.
        
    
    Note:
    
    You cannot fulfill or bill sales orders with the status Pending Approval. You also cannot close lines on a sales order with this status. If you need to make changes to an order that is pending approval, you can remove line items.
    
5.  In the **Process** column, click **Fulfill** next to the order you want to fulfill.
    
6.  Click **Submit**.
    
7.  On the **Item Fulfillment** page, verify or enter information in the following fields:
    
    -   **Posting Period** - the period in which this fulfillment is recorded
        
    -   **Customer or Project** - the customer or project the order is for
        
    -   **Address** - where the order will be shipped
        
    -   **Order #** - the number of the order you are fulfilling
        
    -   **Date** - the date on which the order was fulfilled
        
    -   **Ref. No.** - a number you can later use to reference this partial fulfillment
        
    -   **Ship Via** - the shipping method being used for this order
        
    -   **Shipping cost** - the total cost of shipping for this order
        
    -   **Tracking Numbers** - enter any numbers associated with tracking this shipment
        
8.  In the **Quantity** field, for each item, enter the percentage that has been completed as a decimal.
    
    For example, for a project that has been 50% completed, enter 0.5.
    
    If you want to fulfill the entire order, enter the number 1 for each item.
    
9.  When you have finished:
    
    -   Click **Save** to save the information.
        
    -   Click **Save & Invoice** to save the information and create an invoice for the completed portion of the sales order.
        
    
    If you save without billing, you will need to create an invoice for the completed portion of the invoice at _Transactions > Sales > Bill Sales Orders_.
    

To see what has already been fulfilled and invoiced for an order, go to _Transactions > Sales > Enter Sales Orders > List_. Click View next to the sales order you want to view. Then, in the sales order record, click the Related Records subtab to view invoices, item fulfillments, and other related records.

### Related Topics:

-   [Fulfill a Single Order Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224254.html)
-   [Fulfill Multiple Orders Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1225980.html)
-   [Fulfilling Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
