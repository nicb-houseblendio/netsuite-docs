---
id: "section_N1225980"
type: "section"
title: "Fulfill Multiple Orders Using Advanced Shipping"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Advanced Shipping > Fulfill Multiple Orders Using Advanced Shipping"
parent: "section_N1224089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1225980.html"
anchors: ["procedure_N1226000"]
sha256: "4c3bb69b1f402ae82c06585dca09403fff7ee127ed051da5e040b857196265eb"
---

Use this process to fulfill many orders at one time when Advanced Shipping is enabled. For details about enabling the Advanced Shipping feature, read [Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224089.html).

#### To fulfill multiple orders: {#procedure_N1226000}

1.  Go to _Shipping > Shipping > Fulfill Orders_.
    
2.  Select a customer to show only orders for that customer.
    
3.  Select the period these fulfillments are posting to.
    
4.  Accept or enter the date.
    
5.  Set the shipment status you want to apply to these orders.
    
6.  In the **Transaction Type** field, select to filter the list for sales orders or transfer orders.
    
7.  In the **Bulk Fulfill From Location** field, choose the location you want to fulfill these orders from.
    
8.  In the **Filter By** field, choose one of the following to filter the orders shown:
    
    -   **Some Items Committed** - the list shows orders that have one or more items committed to be fulfilled.
        
    -   **All Items Committed** - the list shows orders that have all items committed to be fulfilled.
        
    -   **Respect Ship Complete** - the list shows only the orders that are committed according to their ship complete setting. This includes all orders that are not restricted to ship complete.
        
    -   **Ignore Item Availability** - the list shows all open orders regardless of the availability of items on the orders.
        
    
    Note:
    
    You cannot fulfill or bill sales orders with the status Pending Approval. You also cannot close lines on a sales order with this status. If you need to make changes to an order that is pending approval, you can remove line items.
    
9.  In the **Fulfill** column, check the boxes next to the orders you want to fulfill or click **Mark All** to select all available orders.
    
10.  Click **Submit**.
     
     The Processed Orders list appears. It lists the item fulfillment created for each order fulfilled.
     

You can edit the item fulfillments created from the Processed Orders list. Click the number in the **Processed Number** column next to the item fulfillment you want to edit. When the item fulfillment appears, click **Edit**. Make any changes, and click **Save**.

All orders you checked are processed together as one Job. If it will take more than 10 seconds to process, the Job Status page opens to show the jobs being processed. For each job being processed, the page shows the Job ID and name, date initiated, status, and percent complete. You can process several fulfillment jobs at once and track them on the Job Status page.

Your inventory is updated for the items that you fulfilled. To see what has been fulfilled and invoiced for a sales order, go to the **History** subtab on the order and click **Fulfillments & Invoices**.

You can also print a label for your shipment. To do this, go to _Transactions > Management > Print Checks and Forms_, and then click the Shipping Labels item. For more information about printing shipping labels, read [Printing Shipping Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262680.html).

### Related Topics:

-   [Fulfill a Single Order Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224254.html)
-   [Fulfilling Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
