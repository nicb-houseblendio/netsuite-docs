---
id: "section_N1223692"
type: "section"
title: "Bulk Fulfilling Orders"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Fulfilling Orders > Bulk Fulfilling Orders"
parent: "section_N1223349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223692.html"
anchors: ["procedure_N1223710", "bridgehead_N1223894", "procedure_N1223909"]
sha256: "98a6844e9811a8d14c679e1831821cad27e66830c9db249443996cd47437d3a8"
---

You can fulfill many orders simultaneously from the same location. You select the location from which you want to fulfill the orders and submit the orders for processing. NetSuite processes the orders in the background.

#### To bulk fulfill orders: {#procedure_N1223710}

1.  Go to _Transactions > Order Management > Fulfill Orders_.
    
2.  Optionally filter the list of orders by selecting a customer you want to fulfill an order for.
    
3.  Select the period you want the fulfillments to post to.
    
4.  In the **Set Shipment Status To** field, select the status you want these fulfilled sales orders to be set to.
    
    Note:
    
    This field appears only when the Pick, Pack, and Ship feature is enabled.
    
5.  In the **Transaction Type** field, select to filter the list for sales orders or transfer orders.
    
6.  To choose the location from which you want to fulfill the orders, select a location in the **Bulk Fulfill From Location** field and clear the Filter box.
    
7.  In the **Filter By** field, choose one of the following to filter the orders shown:
    
    -   **Some Items Committed** - The list shows orders that have one or more items committed to be fulfilled.
        
    -   **Respect Ship Complete** - The list shows only the orders that are committed according to their ship complete setting. This includes all orders that are not restricted to ship complete.
        
    -   **All Items Fully Committed** - The list shows orders that have all items committed to be fulfilled.
        
    -   **Ignore Item Availability** - The list shows all open orders regardless of the availability of items on the orders.
        
    
    If you use the Multiple Shipping Routes feature, you generate an item fulfillment for each address. The shipping address and the corresponding shipping method for each order is displayed in the list of orders for fulfillment.
    
    Note:
    
    You cannot fulfill or bill sales orders with the status Pending Approval. You also cannot close lines on a sales order with this status. If you need to make changes to an order that is pending approval, you can remove line items.
    
    For more information, see [Item Fulfillments and Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263863.html).
    
8.  In the **Ship Via** field, choose the shipping method for the selected sales orders. To use the shipping method as specified on the sales order, select Default From Order.
    
9.  Check the **Fulfill** box next to the orders you want to fulfill.
    
    You can also select the orders you want to process by scanning the sales order barcode in the **Select Order Number** field in the Orders subtab. This field appears only when the Bar Coding and Item Labels feature is enabled.
    
    The Customize button in the Orders subtab lets you add more columns to the list or add more filters above the list.
    
10.  Important:
     
     In this step, the selected sales orders will enter the processing queue and will be fulfilled with the values selected.
     
     Click **Submit** to fulfill the sales orders.
     

All orders you checked are processed together as one Job. If it takes more than 10 seconds to process, the Job Status page opens to show the jobs being processed. For each job being processed, the page shows the Job ID and name, date initiated, status, and percent complete. You can process several fulfillment jobs at once and track them on the Job Status page. Go to _Transactions > Order Management > Fulfill Orders > Status_ to view the status of the sales order fulfillment process.

When fulfillments are in the processing queue, they no longer appear on the Fulfill Orders page.

You can enable a preference to send a confirmation email showing the total quantity shipped upon fulfillment of orders. For more information, read [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html).

## Bulk Update Fields {#bridgehead_N1223894}

The bulk fulfillment page includes a Set Fields subtab where you can enter updates for orders being fulfilled.

For example, if you bulk fulfill a group of sales orders, you may want to update the memo field on all of the orders to say 'Q1 Rush processing.' You are able to enter the memo text on the Set Fields subtab and all orders processed show the new text.

#### To update fields during a bulk process: {#procedure_N1223909}

1.  Go to _Transactions > Order Management > Fulfill Orders_ to open the Fulfill Orders page.
    
2.  Click the **Set Fields** subtab to choose the fields to update and select the data for entry.
    
3.  In the **Field** column, choose a field to update.
    
4.  Depending on the field you select, data can be entered in one of the following fields:
    
    -   In the **Selection** column, choose a setting for the field.
        
    -   In the **Checked** column, define whether a box is checked or cleared.
        
    -   In the **Text** column, enter text to be entered in the chosen field.
        
    -   In the **Date** column, choose a date to be entered in the chosen field.
        
5.  Click **Add**.
    
6.  Repeat these steps for each field you want to update during this bulk process.
    
7.  Complete other fields on the fulfillment form as necessary.
    
8.  Click **Submit**.
    

When you submit the form, the fulfillments are generated and the fields are updated as you have specified.

Note:

Only fields in the header of the form are available to be updated during bulk fulfillment or invoicing.

### Related Topics:

-   [Bulk Fulfilling Orders Using a CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226924.html)
-   [Handling Order Fulfillment Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0527091947.html)
-   [Fulfilling Orders with UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1279306.html)
-   [Fulfilling Orders with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1271195.html)
-   [Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263041.html)
-   [Bar Codes and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
