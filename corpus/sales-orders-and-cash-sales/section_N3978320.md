---
id: "section_N3978320"
type: "section"
title: "Entering Single Grid Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Grid Order Management > Managing Grid Orders > Entering Single Grid Orders"
parent: "section_4274152949"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978320.html"
anchors: ["subsect_157017637293", "procedure_3730058962"]
sha256: "e531740abd9157071d95252daba4ca2664ab0015353d6625bafee25cd03c2e99"
---

You can add orders to transactions using one template per Grid Order Entry form. To do this, ensure that the item price is set for all price levels and currencies in the item record. Items without a price can't be added to a transaction's item sublist. To review the guidelines for grid order entry, see [Managing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274152949.html).

If you want to use multiple templates in one Grid Order Entry form for sales orders, see [Entering Multi-Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4664083498.html).

## Guidelines for Editing Grid Items on the Order Transaction Page {#subsect_157017637293}

Read the following guidelines for editing grid items on the Order Transaction page:

-   Changing the percentage in the **Quantity** field of a line item overrides the percentages defined in the grid template.
    
-   For grid inventory adjustments:
    
    -   The new quantity value is automatically computed and shown in the line items.
        
    -   You enter the unit cost for new orders. The unit cost automatically reflects the average cost when you have saved a new order. You can change the default value of the unit cost.
        
    -   If you use the Multi-Locations feature, changing the location of a grid line item automatically updates the location on the Grid Order Entry form.
        

Follow the instructions below to enter a Grid Order.

#### To enter a grid order: {#procedure_3730058962}

1.  Go to Transactions > (Transaction type).
    
    Follow the standard path for creating the transaction. For example, to create a sales order, go to _Transactions > Sales > Enter Sales Orders_.
    
2.  On the order page, enter values in the Primary Information and Classification sections.
    
3.  (Optional) Enter values in the Sales Information section.
    
4.  On the **Items** subtab, click **Open Grid**.
    
    Alternatively, you can add the parent matrix item on the **Items** subtab if the matrix item is already assigned to a grid matrix template. Ensure that your browser's set to enable popup lists from **system.netsuite.com** to use the Grid Order Entry popup form.
    
    The **Open Grid** button is available only to users who have access to the custom record types supported by Grid Order Management. For more information, see [Roles and Permissions for Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505110051.html).
    
5.  On the Grid Order Entry form, enter values in the Grid Order Information section.
    
    The following steps apply to single grid and multi-grid order entry.
    
    1.  In the **Name** field, select the name for the grid item or grid matrix template.
        
        To use the **%** wildcard in the **Name** field, see [Limitations of Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4273583432.html) for the supported combinations. Results may not be shown due to incorrect values or role restrictions. For Administrators, you can view the logs for error details.
        
        Based on your selected template, the **Type** and **Grid Attribute** fields are populated.
        
    2.  Enter or select values based on the type of transaction.
        
        -   **Sales orders and estimates** - In the **Expected Ship Date** field, enter the date you expect this item to be shipped from the vendor. You must enable the Demand Planning feature in your account to display this field.
            
        -   **Inventory adjustments** - Select a location from the list of options, which are based on the subsidiary. You must enable the Multi-Location feature in your account to display this field.
            
        -   **Transfer orders** - In the **Expected Receipt Date** field, enter the date when you expect to receive the item at the warehouse.
            
            If the Demand Planning feature is enabled in your account, enter the date in the **Expected Ship Date** field.
            
    3.  Specify a value for the order priority in the **Order Priority** field.
        
        For sales orders, the default order priority set for the customer is initially shown. To assign an order priority to a transaction item, replace the default value in the **Order Priority** field.
        
        If you edit the items of a sales order through Grid Order Entry, the default order priority set for the customer is used for added items. To change the order priority of added items, specify a value in the **Order Priority** column of the **Items** sublist.
        
        Default order priority applies only to sales orders and transfer orders.
        
6.  Enter values in the Order Details section.
    
    The following steps apply to single grid and multi-grid order entry.
    
    If the **Enable Quantity Distribution** preference is selected on the Grid Preference page, perform steps **a** and **b**.
    
    Changes to values in the line items are reflected when you reopen the Grid Order Entry form.
    
    1.  In the **Order Quantity** field, enter your total order quantity.
        
    2.  Click **Calculate**.
        
        The quantities are shown for each row and column cell based on the percentages set in the grid template, as well as all totals and inventory levels. Any order quantity that is more than the available quantity for the item is indicated in red.
        
    3.  In the grid, click a cell to review information for that item.
        
        The Item Information section displays selected details from the item record, including the grid attribute values that show for the item.
        
    4.  Review and specify rates.
        
        | **Sales Orders:** |
        | --- |
        | For sales orders, the **Price Level** field on the Grid Order Entry form and the **Price Level** column in the Items sublist are available if the Multiple Pricing feature is enabled in your NetSuite account. By default, the **Edit Rate** box or **Edit Rate and Price Level** box is not checked. This means that the system will use the NetSuite pricing hierarchy to populate the **Price Level** and **Rate** columns in the Items sublist (customer item pricing, group pricing, and customer pricing):
        -   In accounts with the Multiple Pricing feature enabled, the **Estimated Rate** field shows the item price based on the selected price level: Price = Item Price Level starting from Base Price down to the Last Price Level (whichever has the first value)
        
        -   In accounts without the Multiple Pricing feature: Price = Item.Base Price (baseprice)
        
        If the NetSuite item pricing hierarchy is used, it is possible that the values in the **Price Level** and **Estimated Rate** fields on the Grid Order Entry form do not match the values in the **Price Level** and **Rate** columns in the Items sublist. If you check the **Edit Rate** or **Edit Rate and Price Level** box, the system uses the value in the **Price Level** and **Estimated Rate** fields to populate the price level and rate values in the Items sublist. **To override the estimated rate:**
        
        -   In accounts with Multiple Pricing enabled:
            1.  Check the **Edit Rate and Price Level** box.
            2.  Select a price level.
            3.  To enter a custom rate, select **Custom** in the **Price Level** field, then enter a rate in the **Estimated Rate** field.
        -   In accounts without the Multiple Pricing feature
            1.  Check the **Edit Rate** box.
            2.  Enter a rate in the **Estimated Rate** field.
        
        If you change the currency in the **Accounting** tab of the transaction, the **Estimated Rate** field displays the currency rate set in the item record. If the currency rate is not available, the exchange rate applies to the base currency of the customer record. The Quantity Pricing feature is not considered for the rate value. |
        | **Purchase Orders:** |
        | For purchase orders, the **Estimated Rate** field on the Grid Order Entry form shows the value that was saved in the **Purchase Price** field of the item record: Price = Item.Purchase Price (cost) By default, the **Edit Rate** box is not checked. This means that the system will use the NetSuite pricing hierarchy to populate the **Rate** column of the Items sublist. If the NetSuite item pricing hierarchy is used, it is possible that the value in the **Estimated Rate** field does not match the value in the **Rate** column in the Items sublist. For example, if the vendor has a preferred purchase price on the item record, the system uses that price to populate the **Rate** column. If the **Edit Rate** box is checked, the **Estimate Rate** field becomes available for editing. The system then uses the value in the **Estimated Rate** field to populate the rate values in the Items sublist. **To override the estimated rate:** Check the **Edit Rate** box and enter a rate in the **Estimated Rate** field. If you change the currency in the **Accounting** tab of the transaction, the **Estimated Rate** field displays the currency rate set in the item record. If the currency rate isn't available, the exchange rate applies to the base currency of the customer record. The Quantity Pricing feature isn't considered for the rate value. |
        
    5.  To change an item quantity, click the cell, then enter the new value. Computed values in the grid are automatically recalculated when you change item quantities.
        
        If you select the **Enable Quantity Distribution**, you can't edit the item quantities in the grid. Percentages must be changed in the grid template.
        
7.  Click **Submit** to enter the grid order and return to the order transaction.
    
    -   Click **Submit & New** if you want to save the grid order and then enter another one.
        
    -   Click **Submit & Save** to enter the grid order and save the transaction. Use this option to enter transactions with large grid orders.
        
8.  Verify the line items on the **Items** subtab of the Order Transaction page and click **Save**.
    

### Related Topics

-   [Managing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274152949.html)
-   [Entering Multi-Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4664083498.html)
-   [Editing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978408.html)
-   [Importing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499322449.html)
-   [Printing Transaction Records Using the Grid Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1499306991.html)
-   [Viewing the Grid Matrix Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4809938296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
