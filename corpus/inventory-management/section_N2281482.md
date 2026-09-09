---
id: "section_N2281482"
type: "section"
title: "Selling Inventory"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Sales and Fulfillment > Selling Inventory"
parent: "section_N2281204"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281482.html"
anchors: ["bridgehead_N2281549", "procedure_N2281627", "bridgehead_N2281705", "bridgehead_3811914790", "bridgehead_3811916368"]
sha256: "6a4810a92520e7be38a3f721d01283ed69ed76fc7b268b11007a95dbea06214f"
---

Record inventory sales by adding an item to a sales transaction. Sales transactions that affect inventory levels include sales orders, invoices, and cash sales.

When you add an item on a sales order, the inventory record for the item is automatically checked to see if the item is available. By default, available items are committed from your inventory and reserved for that customer. Because sales are integrated with inventory records, inventory records are automatically updated with each sale.

Selling an item affects information tracked on the item record. If the item can be filled from the quantity available:

-   the item is committed to the sale
    
-   the quantity committed increases
    
-   the quantity available decreases
    
-   the cost of goods sold increases
    

If the item cannot be filled from the quantity available, then the quantity backordered increases.

If you set the **Perform Item Commitment After Transaction Entry** preference, inventory items are committed as you enter or approve each transaction. See [Order Management Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1388149.html) or [Committing Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3765928460.html).

## Inventory Sales and Item Commitment {#bridgehead_N2281549}

Item commitment is the method used to track what you promise to deliver to your customers. Based on the items on a sales order, NetSuite tracks how much of each item you sell. It calculates how much has been sold and how much can be ordered. It shows which sales orders to fulfill first when you receive more stock.

Depending on stock level and item type, items can be committed either when they are sold or received. The flowchart below explains how items are committed:

![Item Commitment diagram](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/InventoryManagement/itemCommittment1.png)

When you commit an item on a sales order, the number of items committed increases by the ordered quantity.

For example, you currently have 100 widgets available and on hand with no outstanding orders. When you create a sales order for 70 widgets, you can commit the ordered quantity. Your available quantity adjusts to 30 widgets (on hand quantity of 100 - quantity committed on orders of 70).

Item commitment for drop ship and special order items works differently from commitment for regular items. When you set an item to drop ship or special order on a sales order, it is not committed. It also doesn't immediately affect your item commitment count. See [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html) and [Special Order Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html).

## Availability, Ship Complete and Item Commitment {#procedure_N2281627}

By default, you commit available items to an order. On the **Items** subtab of an order, you can change the default commit option. You can choose to commit items only when an entire order or line item can be fulfilled. You can also manually defer commitment. In the **Commit** column, you can select one of the following:

-   **Available Qty** - Items for this line item are committed as available. Available items are shipped, and items that aren't available are placed on back order.
    
-   **Complete Qty** - This line item only ships when all items are committed.
    
-   **Do Not Commit** - Items aren't committed to this line item until this setting is changed.
    

You can also set transaction line items to ship only when completely available. For customers who prefer to receive orders only when they are completely fulfilled, check the **Ship Complete** box. This option is on the Financial subtab of the customer records.

For example, your customer Bob buys widgets and widget covers from you. Bob cannot use the widgets without the covers, and he prefers that you send them to him all together. You mark Bob's customer record as Ship Complete.

When Bob orders 20 widgets and 20 widget covers, you have 20 widgets in stock, but only 15 covers. Because Bob's order is marked Ship Complete, it does not appear in the fulfillment queue to send a partial fulfillment. After all 20 widgets AND all 20 widget covers are available together, Bob's order appears in the fulfillment queue.

You can also set an individual order to ship only when all items are available, even if the customer record is not marked. To ship an order only when all items are available, check the **Ship Complete** box on the Shipping subtab of the transaction.

To fulfill orders in bulk, filter the list of orders to show only orders that can be completely fulfilled. Select **Respect Ship Complete** in the **Filter By** field.

## Inventory Sales and General Ledger Accounts {#bridgehead_N2281705}

Not only is the commitment of items to customers tracked in your account, but inventory values are also tracked in your general ledger. When you sell items, the total value of the inventory sold is deducted from your Inventory Asset account. The total cost of the inventory sold is added to your Cost of Goods Sold (COGS) account.

Use reports to monitor the value of your inventory assets on hand. You can also determine if you have too much cash tied up in stock on hand. For more information, read [Inventory Value Assessments with Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2358468.html).

## Enhanced Item Allocation {#bridgehead_3811914790}

If you use the Demand Planning feature, read [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html) for more information about automating item commitment.

## Fulfillment {#bridgehead_3811916368}

After you have recorded a sale, you need to get the product to your customer. Enter a fulfillment each time you physically take an item out of inventory and ship it to the customer. For more information, read [Fulfilling Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281951.html).

### Related Topics

-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Purchasing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html#bridgehead_N2251155)
-   [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Warehouse Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317586.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
