---
id: "section_N2290234"
type: "section"
title: "Calculating Item Demand"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Demand Planning > Calculating Item Demand"
parent: "section_N2286970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html"
anchors: ["kaltura_player_144", "procedure_N2290291", "bridgehead_N2291319", "bridgehead_N2291331", "bridgehead_N2291372"]
sha256: "f53007bf3819d93124ff15706ddb1aac39f8744615718b9667520d0a371cb687"
---

Use the Calculate Item Demand Plan page to forecast an item's demand over a future period. NetSuite doesn't consider past forecast quantities, but reviews historical demand to estimate upcoming demand.

For example, you can look at an item's demand over the past six months to forecast demand for the next six months.

To calculate demand, choose a projection method, select the data to use for analysis, and set the forecast period. NetSuite uses this forecast data to project future demand across a designated time period and suggests a plan for orders.

After you submit the Calculate Item Demand Plan page, NetSuite creates a demand plan for each selected item. Demand plans record the expected future demand for an item based on previous demand. You can then view, edit, and use these demand plans to create supply plans for items.

Note:

If estimates or quotes don't have rates, they won't appear in the Demand Plan. If rates are 0, the entered quantities aren't counted either.

<a id="kaltura_player_144"></a>

#### To calculate item demand: {#procedure_N2290291}

1.  Go to _Transactions > Demand Planning > Calculate Item Demand Plan_.
    
2.  If you use NetSuite OneWorld, select a **Subsidiary**.
    
3.  If you use the Multi-Location Inventory feature, select a **Location**.
    
    The list of items shows only time-phased replenishment items for the selected location.
    
4.  You can forecast demand for items in two ways:
    
    -   Set a time frame to review an item's historical sales data to analyze previous sales trends and forecast future sales.
        
    -   Use current demand (such as opportunities, quotes and existing sales orders) to forecast future sales. This method isn't based on a calculated forecast.
        
    
    Select a **Projection Method**:
    
    -   **Linear Regression** - Projects future inventory by using past demand and applying the ordinary least squares method.
        
    -   **Moving Average** - Projects future inventory by using the moving average of historical demand to calculate the average stock level needed and applying that average to upcoming periods.
        
        NetSuite uses the historical duration parameter to calculate the moving average demand in the past. The moving average is used as a smoothing function to minimize demand variations. The same average is used for all projected periods.
        
        For example:
        
        -   Today is 2/1/2011.
            
        -   Historical duration is set to 3 months.
            
        -   Projected duration is set to 2 months.
            
        
        The following results:
        
        |  | 10/1/2010 | 11/1/2010 | 12/1/2010 | 1/1/2011 | 2/1/2011 | 3/1/2011 |
        | --- | --- | --- | --- | --- | --- | --- |
        | Historical Demand Data | 5 | 4 | 5 | 6 |  |  |
        | Projected Demand Data |  |  |  |  | 5 | 5 |
        
    -   **Seasonal Average** - Examines past demand to identify seasonal trends and uses those trends to forecast future stock levels.
        
        Note:
        
        When you use this method, you have to set the projection interval to Monthly.
        
    -   **Sales Forecast** - When using NetSuite for your sales operations, this option uses forward-looking sales forecast data to project inventory demand.
        
        When you use the Sales Forecast method, NetSuite uses the following transaction types for projection calculations:
        
        -   cash sale
            
        -   invoice
            
        -   estimate
            
        -   opportunity
            
        -   sales order
            
        -   item fulfillment
            
        
        The following table shows the date and quantity considerations.
        
        | Transaction Type | Date | Quantity |
        | --- | --- | --- |
        | Estimate
        -   Estimates without any associated sales orders, invoices, or cash sales
        
         | Expected Ship Date Note: Data is not referenced when an expected ship date is not populated. | Estimate Quantity |
        | Opportunity
        
        -   Opportunities without any associated sales orders, invoices, or cash sales
        
         | Expected Ship Date Note: Data is not referenced when an expected ship date is not populated. | Opportunity Quantity |
        | Sales Order
        
        -   Only approved sales orders
        
         | Expected Ship Date Note: If an expected ship date is not listed, then the Transaction Date is used. | Quantity remaining that is not yet shipped |
        | Item Fulfillment
        
        -   Only for fulfillments associated with a sales order
        
         | Transaction Date | Quantity Shipped |
        | Cash Sale
        
        -   Standalone cash sales
        -   Cash sales created from estimates
        -   Cash sales created from sales orders when Advanced Shipping is disabled
        
         | Transaction Date | Cash Sale Quantity |
        | Invoice
        
        -   Standalone invoice or invoice from estimate
        -   Invoice created from estimate
        -   Invoice created from sales order when advanced shipping is off
        
         | Transaction Date | Invoice Quantity |
        
5.  In the **Projection Interval** field, choose the period of time demand is calculated for. For example, select Weekly to project how much demand is expected per week, as opposed to per month.
    
    If you use the Seasonal Average method, only a Monthly interval is supported.
    
    The **Projection Start Date** field shows the first date of the forecast demand period.
    
6.  In the **Projection Duration** field, enter the number of periods to project demand. For example, enter **6** to calculate demand for a six month period.
    
    Note:
    
    You can only enter whole numbers. For example, if you enter 3 and select Months, demand is forecast for three months.
    
7.  **Historical Analysis Duration** - Enter the number of periods in the past you want to use to calculate demand projection.
    
    -   For Moving Average, enter the number of past periods to calculate the next moving average value.
        
    -   For Linear Regression, enter the number of past periods to base the linear regression projection on.
        
    -   This field isn't required when using the Sales Pipeline projection method.
        
    -   For Seasonal Average, enter the number of past periods to use for calculating the future demand.
        
8.  Select all items for which you want to calculate demand.
    
9.  The **Alternate Source Item** field lets you to select another item to use its historical data for calculating demand.
    
    For example, if you're setting up Item A for demand planning but it doesn't have much sales history, you can choose Item B as an alternate source. When NetSuite calculates demand for Item A, it uses Item B's history for the calculation.
    
    The alternate source must be the same type as the original item. For example, if the original is an inventory item, the alternate must also be an inventory item.
    
    Note:
    
    When you create a demand plan using an alternate source, NetSuite still applies the expected demand change for the original item.
    
10.  Click **Submit**.
     

After you submit, NetSuite creates demand plans for all selected items. To view the plans, go to _Transactions > Demand Planning > Item Demand Plans._.

When calculating demand, NetSuite includes transactions dated before the start date for items using Entered and Planned Orders as the demand source. These transactions are treated as existing demand orders on the planning calculation's start date:

-   A sales order that is not closed
    
-   A sales order that is not fully shipped
    
-   A sales order that has a date that is before the start date
    

Sales and purchase orders dated before the start date are expected to be received or shipped on the day of the supply calculation.

If an item has no transaction history, you can use another item's history, enter your own forecast, or import the sales order history.

## Assemblies and Demand Calculations {#bridgehead_N2291319}

If an assembly's components are set to calculate demand source from Entered and Planned Orders, you don't need to create demand plan. NetSuite creates necessary orders for the assembly and its components when their calculation runs.

## CSV Import {#bridgehead_N2291331}

Account administrators and other users with Import CSV File permission can use the Import Assistant to import demand plans. For more information, see [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html). For general information about using CSV import for items, see [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html).

## SOAP Web Services {#bridgehead_N2291372}

You can use SOAP web services to add, update, delete, search, and retrieve demand plans. See [Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3679563.html) in the SOAP web services section of the Help.

### Related Topics

-   [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html)
-   [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html)
-   [Monitoring the Demand Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291615.html)
-   [Viewing, Editing, and Deleting a Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291961.html)
-   [Manually Entering an Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2292418.html)
-   [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html)
-   [Monitoring the Supply Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293790.html)
-   [Viewing, Editing, and Deleting a Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294140.html)
-   [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html)
-   [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html)
-   [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html)
-   [Distribution and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296427.html)
-   [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html)
-   [Time Fences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3848058018.html)
-   [Planning Action Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3865354301.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
