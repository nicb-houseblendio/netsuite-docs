---
id: "section_N1231176"
type: "section"
title: "Marking an Order Shipped"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Pick, Pack, and Ship > Marking an Order Shipped"
parent: "section_N1229691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231176.html"
anchors: ["procedure_N1231209"]
sha256: "fbb84b40c73e6137843e59f5ebc3ad3416e2c4de229fcf3dca1149fb574abeab"
---

The Pick, Pack, and Ship feature gives your warehouse and shipping departments separate processes for each step to fulfill orders.

After you have marked items on an order as picked and packed, they need to be marked shipped to the destination.

#### To mark orders shipped: {#procedure_N1231209}

1.  Go to _Shipping > Shipping > Mark Orders Shipped_.
    
2.  Optionally, filter the list of orders you want to mark as shipped:
    
    1.  In the **Customer** field, select a customer to show only orders from a specific customer.
        
    2.  In the **Order Type** field, select a transaction type.
        
    3.  In the **Bulk Fulfill from Location** field, select a location to show only orders that have the selected location set in the Location column on the sales order line.
        
        Select **Unchanged** to show all orders regardless of fulfillment location.
        
        Note:
        
        This field only shows if you use the Locations feature.
        
3.  In the **Ship Via** field, select the shipping method you want to set on all orders shipped.
    
    If you do not want to change the shipping method that is set on each individual order, select **Unchanged**.
    
4.  In the **Mark Shipped** column, check the box next to each order you want to mark as shipped.
    
    You can click the **Mark All** button to select all orders in the list.
    
    You can also select a specific order in the list by entering the sales order number in the Select Order Number field and then pressing Enter.
    
5.  Click **Submit**.
    

When you check multiple orders, the orders are processed together as one job. If it will take more than 10 seconds to process them, the Job Status page opens to show the jobs being processed.

You can process several jobs at once and track them on the Job Status page. For each job being processed, the page shows the following:

-   Job ID and name
    
-   Date and time the job was initiated
    
-   Status of the job
    
-   Percentage of the job complete
    
-   Any related error messages
    
-   Results column with a link to a processing log
    

Click the Order Processing Log link in the **Results** column to open the Processed Orders page. This page details the following information about each transaction in the job:

-   Original transaction type, date, and number
    
-   Processed transaction type, number, and status
    
-   Errors associated with a transaction being processed
    

### Related Topics:

-   [Pick, Pack, and Ship Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229796.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html)
-   [Commitment Settings for Reallocation of Picked or Packed Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0525105436.html)
-   [Fulfilling Orders Using Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230473.html)
-   [Marking an Order Packed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230849.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
