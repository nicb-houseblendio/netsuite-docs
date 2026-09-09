---
id: "section_N2262573"
type: "section"
title: "Assessing Stock Levels"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Assessing Stock Levels"
parent: "chapter_N2250682"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2262573.html"
anchors: ["bridgehead_N2263144", "bridgehead_N2263200", "bridgehead_N2263282", "subsect_0604111134"]
sha256: "0d89e591eba4be85ca87d262542318ba6a76d9c92e008280b52aab876815c06a"
---

Inventory Management provides multiple ways of accessing inventory data for viewing real-time information about item quantities and value. With this information, you can assess how much you have, how much you need, and the value of your stock on hand. Then, you can determine how your stock levels affect your inventory workflow.

For example, if stock of an item is too low, then your order-to-delivery cycle time increases, and this can negatively affect customer service. If stock of an item is too high, then your overhead is increased by having money tied up in items sitting on shelves.

Here are several ways to access item information:

-   View the Items list by going to _Lists > Accounting > Items_.
    
-   [View an Individual Item Record](#bridgehead_N2263144)
    
-   [View Inventory Reports and Saved Searches](#bridgehead_N2263200)
    
-   [Utilize Stock Replenishment](#bridgehead_N2263282)
    

Information from item records, reports, and saved searches may include multiple quantities and inventory levels. They're listed in the following table along with a definition to help you understand the differences between them as you assess your inventory:

| Quantity/Level | Definition |
| --- | --- |
| Quantity Available | Quantity On Hand less Quantity Committed Note: Quantity Available is never tracked as a negative quantity. An item is either non-available (quantity 0) or available (a positive quantity). You cannot commit items in an underwater state. |
| Quantity On Hand | Quantity currently stocked, including Quantity Committed |
| Quantity Committed | Quantity promised to customers on approved sales orders that are not yet fulfilled |
| Quantity On Order | Quantity on approved purchase orders pending receipt from the vendor |
| Quantity To Order | Preferred Stock Level less Quantity Available |
| Quantity Back Ordered | Quantity committed to sales for which there is no stock to fill the order |
| Reorder Point | Quantity level at which you need to place an order to replenish stock, or build more of this item. |
| Preferred Stock Level | This is the optimum quantity to maintain in stock of an item. The ideal quantity is the amount you need to fulfill orders in a timely manner without either running out or overstocking. This quantity is used to determine your replenishment needs on the Order Items page. It is the quantity you want to have in stock after an order is placed. The preferred stock level you set is used to calculate the quantity of items to be ordered on the Order Items page. |
| Safety Stock | This is a measure of the amount of stock you want to keep on hand to account for variations in demand so that you do not run out. It is a buffer amount of an item you prefer to keep in stock at all times so that you do not run out. |

Additional quantities, such as quantity in transit and quantity allocated, may appear depending on features and transactions that you use. If you use the Multiple Units of Measure feature, additional on-hand and available quantities appear in your base unit. For information about viewing stock levels for the Multi-Location Inventory feature, see [Item Settings and Stock Levels for Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305626.html) and [View Transfer Data on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html#bridgehead_N2309039). For information about multiple units of measure, see [Assigning Units of Measure to Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212390.html).

Questions you may ask during stock assessment include:

-   Do I have items at or below their preferred stock level or reorder point?
    
-   How many backorders do I have?
    
-   Do I need materials to assemble items?
    
-   What quantity should I order?
    
-   What is the lead time to receive items?
    
-   Has demand increased or decreased for an item?
    

Your answers to these questions determine how you order your items and materials. In general, many companies order inventory with the goal of keeping inventory at an optimum level rather than keeping many extra items on hand.

It is ideal to keep enough goods to service customers by fulfilling orders in a timely manner without having extra stock on hand. Extra stock reduces funds tied up in idle stock.

To assess stock information and determine your replenishment needs, identify information about your items and materials. For example, stock available and customer demand. Then, you can determine the quantities of items you need.

When you view item stock status on item records or on the item list, you can use these quantities to determine inventory replenishment needs. For example, you could determine that:

-   An item with a quantity available below the preferred stock level and a quantity on order of zero may need to be ordered.
    
-   An item with a large quantity available and large quantity on order may need to be ordered less often.
    
-   An item with a low preferred stock level and a high quantity backordered may need to be ordered more frequently or in higher quantities.
    
-   An item with any quantity backordered and a quantity on order of zero may need to be ordered.
    
-   An item that is backordered in one location, but has high quantities in another location may need to be redistributed.
    

## View an Individual Item Record {#bridgehead_N2263144}

Access item records and view item quantities, including inventory levels that you set, by doing the following:

1.  Go to _Lists > Accounting > Items_.
    
2.  From the Items list, click **View** next to the item record you want to access.
    
3.  On the **Purchasing/Inventory** subtab, you can view inventory settings and quantities per location.
    
4.  If you specify bins on the item record, on the **Bin Numbers** subtab, you can view quantities per bin.
    
5.  Based on features you use, on the **Inventory Detail** subtab, you can view quantities across specific item attributes, including bins.
    
    For more information, see [Inventory Detail Subrecord](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html#procedure_N2271907).
    

## View Inventory Reports and Saved Searches {#bridgehead_N2263200}

You can view inventory reports that provide different views of inventory details across multiple items. For more information about available reports, read the following topics:

-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)
    
-   [Inventory Level Assessments with Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2354076.html)
    
-   [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html)
    

To track specific quantities across items, you can also use these saved searches:

-   [Inventory Balance Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518564230.html) - lets you compare between on hand and available inventory across items, which may include additional attributes like inventory status.
    
-   [Inventory Detail Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518565583.html) - lets you view the absolute impact and positive or negative impact of each inventory detail line from a transaction.
    

## Utilize Stock Replenishment {#bridgehead_N2263282}

NetSuite can automatically assess item replenishment needs and make suggestions for purchases. After you enter stock information an item record, NetSuite can suggest when to reorder the item and how many to purchase. This can be done using the following features:

-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
    
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
    

By assessing item stock levels and sales information in reports, you can determine the optimum stock levels for your items and streamline your inventory.

If you use the Multi-Location Inventory feature, see [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html). This article provides information about taking surplus items out of one location and move them into another location with too few.

## Handle Stock Level Issues {#subsect_0604111134}

To handle underwater inventory, quantity discrepancies, or insufficient quantities on transactions, you can review the following articles:

-   [Reviewing Negative Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2268458.html)
    
-   [Review Item Line/Inventory Detail Quantity Mismatch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1456591.html#bridgehead_0919021216)
    
-   [Mismatched Transaction Handling Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1456591.html#procedure_N1456922)
    
-   [Avoiding Underwater Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2264208.html)
    
-   [Handling Backorders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263962.html)
    
-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
    
-   [Disabling Use Bins Settings and Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0512092419.html)
    
-   [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html)
    

### Related Topics

-   [Inventory Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161970666917.html)
-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Inventory Management with Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162100850596.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Purchasing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html#bridgehead_N2251155)
-   [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html)
-   [Warehouse Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317586.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
