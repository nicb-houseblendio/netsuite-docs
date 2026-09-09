---
id: "section_N2295603"
type: "section"
title: "Gross Requirements Inquiry"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Demand Planning > Reporting on Demand Planning > Gross Requirements Inquiry"
parent: "section_N2295256"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295603.html"
anchors: ["procedure_N2295641"]
sha256: "4d66ba17a2fdf7368532f1939e3b264ec84465bdf4d0b282db36eaf20e21f637"
---

The Gross Requirements Inquiry provides an overview of the progressive supply and demand cycle, listing quantities required and supplied on each transaction date listed. Each transaction and date appears with the more-on-hand or less-on-hand quantity of the transaction. It also provides the resulting total quantity on hand for the item.

Important:

The NetSuite [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html) (MRP) solution replaces Time-Phased Planning and offers more features and better performance.

New customers should use the [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html) (MRP) solution. Existing customers should plan to move from Time-Phased Planning to MRP.

If you check the Show Details box in the header, each line of the Gross Requirement Inquiry details the orders that create the demand. This includes sales orders, transfer orders, and work orders that create demand for items and components.

When the Show Details box is checked, the Gross Requirement Inquiry shows these additional columns:

-   Order - This column lists the sales order or transfer order number that created the demand for the line. Click the number to open the order.
    
-   Assembly - This column lists the work order number that created the demand for the line. Click the number to open the order.
    

This list shows in segments of 250 lines and has a maximum of 1000 lines. For more information about line limitations, see [Limitations for Displaying Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159361334524.html).

Note:

NetSuite considers work order demand for orders with a production start date that is before the planning start date. NetSuite does not consider suggested work order demand for orders with a production start date that before the planning start date.

For example: Today is August 1st.

The start date of the planning run is August 1st.

Based on the forecast demand, a work order is suggested by the planning process. The suggested work order start date is July 30th. The start date is prior to the start date of the planning run. Therefore, the dependent demand of the components of this work order is not considered by the planning process.

#### To run a Gross Requirements Inquiry: {#procedure_N2295641}

1.  Go to _Transactions > Demand Planning > Gross Requirements Inquiry_.
    
2.  If you use NetSuite OneWorld, select a subsidiary.
    
3.  Optionally check the **Show Details** box.
    
4.  If you use the Multi-Location Inventory feature, select a location.
    
    The items list is filtered to show only items for the selected location that are time-phased replenishment items and have existing supply plans generated.
    

The following information for the selected item is displayed in the form header for reference:

-   **Unit of Measure** (supply plan unit only)
    
-   **Safety Stock Level**
    

The inquiry displays data retrieved from your account regarding all events that change the stock level of the selected item. Each line of the inquiry results shows the following:

-   **Date** - The expected date of receipt (for supply) or shipping (for demand orders.)
    
-   **Order Date** - The date an order needs to be placed to meet demand.
    
-   **Type** - The type of event that affects the inventory level.
    
    The following are the types of events you may see on an inquiry:
    
    -   Entered Demand Orders
        
    -   Entered Supply Orders
        
    -   Forecast from Demand Plan
        
    -   Planned Work Order - Component Consumption
        
    -   Planned Work Order - Assembly Build
        
    -   Planned Purchase Order
        
-   **Quantity** - The amount of the item that will be added to or removed from the on-hand amount resulting from the event on that line.
    
-   **Quantity on Hand** - The new total amount on hand including the amount changed by the event on that line.
    

The first line of the inquiry shows the beginning quantity on hand of the item. Subsequent lines show each transaction that adds or subtracts inventory to change the stock level and shows the new resulting quantity on hand.

For example, an inquiry may display the following:

| Date | Order Date | Type | Quantity | Qty on Hand |
| --- | --- | --- | --- | --- |
| 1/15 |  | Beginning inventory |  | 0 |
| 1/20 | 1/14 | Planned Supply: Purchase Order | 10 | 10 |
| 2/1 |  | Existing Supply Order | 8 | 18 |
| 3/1 |  | Item Demand | 9 | 9 |

Notice that an order is placed on January 14th and is expected to be received on January 20th. This order will add 10 units to the on hand count. Then, on February 1st, an order is expected that adds 8 more units to stock, bringing the total to 18. Finally, on March 1st, demand for the item removes 9 units from stock, leaving a total of 9 units on hand.

Important:

All posting and non-posting transactions recorded during a day are posted to Planned Supply Orders. The beginning on hand amount reflects the inventory on hand at the beginning of the day.

The inquiry details the anticipated movement of item quantities into and out of stock. The details provide the expected level of stock at any certain date. By viewing and assessing the inquiry, you can determine if the inventory variances look appropriate. This assessment enables you to make changes to supply plans as necessary to maintain optimal stock levels.

Note:

If you make changes to a Gross Requirements Inquiry, you must re-generate the supply plan and run a new inquiry to see the changes.

For example, you may view an inquiry and decide to create an order that is suggested on a supply plan. After you create the order at the Order Items page, you must regenerate the supply plan. Then, you must run a new inquiry to see the new order as a line on the inquiry. For details on ordering, see [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html).

### Related Topics

-   [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
