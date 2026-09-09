---
id: "section_N3978408"
type: "section"
title: "Editing Grid Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Grid Order Management > Managing Grid Orders > Editing Grid Orders"
parent: "section_4274152949"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978408.html"
anchors: ["subsect_157053602438", "procedure_158029251948"]
sha256: "41486ac5511fbe18d5405eb793c3755a72a0fc0664fa7903af83d22cd04b2bb3"
---

You can edit grid orders that have been submitted through single or multi-grid order entry.

## Guidelines for Editing Grid Orders {#subsect_157053602438}

Read the following guidelines for editing grid orders:

-   Grid inventory adjustments can be edited.
    
-   Changes to a grid template don't automatically reflect in the grid orders where the template is used. To update a grid order, you either manually edit it and reload the grid template, or manually update the line items.
    
-   Users without grid access can't edit items that have been added through grid orders. When they edit other items and details on the transaction, the grid item details stay the same.
    
-   The Order Summary table is not shown on the Grid Order Entry form in Edit mode.
    
-   When you create sales orders from estimates with grid orders, the grid order is carried over. You can edit the item quantities in the sales order grid. When you convert estimates to transactions not supported by grid ordering, you can edit the order in the item sublist of transactions. For the list of transactions supported by grid order entry, refer to the table on [Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3975465.html).
    

Follow these instructions to edit grid orders.

#### To edit a grid order: {#procedure_158029251948}

1.  Go to Transactions > (Transaction type).
    
    Follow the standard path for editing the transaction. For example, to edit a sales order, go to _Transactions > Sales > Enter Sales Orders_.
    
2.  In the list of orders, click **Edit** beside the transaction.
    
3.  On the **Items** subtab of the order page, perform any of the following:
    
    -   To enter a new grid order, click **Open Grid**.
        
        For instructions, read the following topics:
        
        -   [Entering Single Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978320.html)
            
        -   [Entering Multi-Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4664083498.html)
            
        
        The **Open Grid** button is only available to users who have access to at least one of the supported custom record types.
        
    -   To edit an existing grid order, perform the following steps:
        
        1.  In the **Grid Template** column, look for the grid template name used in the grid order.
            
        2.  In the **Link** column, click the Open icon to display the existing grid order.
            
        3.  On the Grid Order Entry form, you can make the following changes depending on the grid preferences defined in your account.
            
            -   If you use the Enable Quantity Distribution preference, you can change the total order quantity. Enter the new value in the **Order Quantity** field, then click **Calculate**.
                
            -   To change specific item quantities, click the cell, then enter the value. Percentages and total values are automatically recalculated.
                
            
            For grid inventory adjustments, setting the value of the cell to zero removes the corresponding grid line item from the transaction. For more information about grid preferences, see [Setting Grid Order Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505110343.html).
            
        4.  Click **Submit**.
            
            -   Click **Submit & New** if you want to save the grid order and then enter another grid order.
                
            -   Click **Submit & Save** to enter the grid order and save the transaction. Use this option to enter transactions with large grid orders.
                
    -   Click a line item to change or add values.
        
        Changing the percentage in the **Quantity** field of a line item updates the percentage in its associated grid template when you open the grid.
        
    -   Apply line item discounts.
        
    -   Remove line items. To remove all transaction lines from the order, click **Clear All Lines**.
        
4.  After completing the changes, click **Save** on the order page.
    

### Related Topics

-   [Managing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274152949.html)
-   [Updating Multi-Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4664091990.html)
-   [Entering Single Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978320.html)
-   [Entering Multi-Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4664083498.html)
-   [Importing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499322449.html)
-   [Viewing the Grid Matrix Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4809938296.html)
-   [Roles and Permissions for Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505110051.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
