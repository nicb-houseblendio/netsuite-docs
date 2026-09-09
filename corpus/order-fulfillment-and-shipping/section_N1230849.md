---
id: "section_N1230849"
type: "section"
title: "Marking an Order Packed"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Pick, Pack, and Ship > Marking an Order Packed"
parent: "section_N1229691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230849.html"
anchors: ["procedure_N1230881"]
sha256: "e03856906cee1c1192de0e9ed17966e067bf52587b5fd47731b5915043ad89eb"
---

The Pick, Pack, and Ship feature gives your warehouse and shipping departments separate processes for each step to fulfill orders.

After you have picked/fulfilled items for an order, they need to be packed and then shipped to the customer.

#### To mark orders packed: {#procedure_N1230881}

1.  Go to _Shipping > Shipping > Mark Orders Packed_.
    
2.  Optionally, filter the list of orders you want to mark as packed:
    
    1.  In the **Customer** field, select a customer to show only orders from a specific customer.
        
    2.  In the **Order Type** field, select a transaction type.
        
    3.  In the **Bulk Fulfill from Location** field, select a location to show only orders that have the selected location set in the Location column on the sales order line.
        
        Select **Unchanged** to show all orders regardless of fulfillment location.
        
        Note:
        
        This field only shows if you use the Locations feature.
        
3.  In the **Ship Via** field, select the shipping method for the orders you're packing.
    
    If you do not want to change the shipping method that is set on each individual order, select **Unchanged**.
    
4.  To select a specific order, enter the sales order number in the **Select Order Number** field and press Enter.
    
    If the sales order number is displayed in the list, the Pack box is checked next to the order.
    
5.  In the **Pack** column, check the box next to each order you want to be marked as packed.
    
    You can click the **Mark All** button to select all orders in the list.
    
6.  Click **Submit**.
    

When you bulk pack orders, the orders are processed together as one job. If it will take more than ten seconds to process them, the Job Status page opens to show the jobs being processed.

You can process several jobs at once and track them on the Job Status page. For each job being processed, the page shows the following:

-   Job ID and name
    
-   Date and time the job was initiated
    
-   Status of the job
    
-   Percentage of the job complete
    
-   Any related error messages
    
-   Results column with a link to a processing log
    

Click the Order Processing Log link in the Results column to open the Processed Orders page. This page details the following information about each transaction in the job:

-   Original transaction type, date, and number
    
-   Processed transaction type, number, and status
    
-   Errors associated with a transaction being processed
    

Now, the items are packed and need to be shipped to the customer. To mark orders shipped, go to _Shipping > Shipping > Mark Orders Shipped_.

### Related Topics:

-   [Pick, Pack, and Ship Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229796.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html)
-   [Commitment Settings for Reallocation of Picked or Packed Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0525105436.html)
-   [Fulfilling Orders Using Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230473.html)
-   [Marking an Order Shipped](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231176.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
