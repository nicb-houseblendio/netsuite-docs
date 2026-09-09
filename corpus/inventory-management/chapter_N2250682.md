---
id: "chapter_N2250682"
type: "chapter"
title: "Basic Inventory Management"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management"
parent: "book_N2249433"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html"
anchors: ["bridgehead_161972020739", "bridgehead_1527530735", "subsect_65155750995", "bridgehead_N2259180", "bridgehead_1527531134", "bridgehead_161972153069", "bridgehead_1527531600", "bridgehead_N2259472", "bridgehead_3811939098"]
sha256: "6a003a872bcae7e68c3034166f883d461703527bfe77d6abaa0558db77db0ac3"
---

This section describes the basic processes and tasks for inventory management. It includes the forms you can use to perform the tasks.

Some of the tasks depend on other features that you enable along with the Inventory feature. See [Enabling Features for Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161963741628.html) or [Inventory Setup with Locations and Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2252794.html).

## Assess Stock Levels {#bridgehead_161972020739}

View inventory quantities on individual item records, lists, or through inventory reports and saved searches. Aside from tracking stock quantities and levels, you might also be able to identify quantity discrepancies and other such issues. See [Assessing Stock Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2262573.html).

Run a report to view any negative inventory quantities that you can adjust or replenish. See [Reviewing Negative Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2268458.html).

## Adjust Inventory Levels {#bridgehead_1527530735}

Adjust the on-hand quantity of your inventory items, without entering a purchase order, by using either of these forms: Inventory Adjustment or Inventory Worksheet. See [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).

If you use the [Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296970.html) feature, you can perform a physical count and adjust inventory based on the results of the count. An approved count automatically creates the necessary inventory adjustments to reconcile your inventory.

## Move Inventory {#subsect_65155750995}

If you have multiple locations, you can view item records or review negative inventory to assess your stock levels in each location. See [Item Settings and Stock Levels for Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305626.html) or [Reviewing Negative Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2268458.html).

To handle inventory requirements across locations, you can transfer inventory through the following forms:

Note:

NetSuite provides Inventory Distribution forms that let you assign unallocated inventory to single or multiple locations, as part of your [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html) setup. Right after you configure your locations, distribute your unallocated inventory. You can process succeeding inventory movements through inventory transfers or transfer orders. See [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html).

-   **Inventory Transfer** - to transfer inventory by increasing the on-hand quantity on one location and decreasing the quantity on another location. See [Basic Inventory Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4660882963.html).
    
-   **Transfer Order** - to schedule and track the movement of inventory items. See [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html).
    
-   **Intercompany Transfer Order** - in NetSuite OneWorld accounts, to move inventory between locations in two different subsidiaries within your company. See [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html).
    
-   **Bin Transfers and Bin Putaway** - If you use the Bin Management feature, you can transfer items between bins or put away items in bins. See [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html).
    

## Track Inventory in Bins and by Status {#bridgehead_N2259180}

If you enable the Bin Management feature, you can identify and track regular inventory items in bins within your location. The Advanced Bin/Numbered Inventory Management feature provides support for serialized or lot-numbered items and enhanced tracking per location. See [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html).

Also, when you use the Advanced Bin/Numbered Inventory Management feature, you can enable the Inventory Status feature. Inventory Status provides the ability to associate a status to inventory items. See [Inventory Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515696627.html).

## Replenish Inventory {#bridgehead_1527531134}

As you receive items through purchase orders, your inventory levels are automatically adjusted. See [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html). For information about the purchasing process within the inventory workflow, see [Inventory Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html).

When you set reorder points and preferred stock levels for your inventory items, you can use the Order Items form to determine which ones need to be replenished. You can submit purchase orders in bulk for these items. See [Ordering Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html) or [Item Settings and Stock Levels for Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305626.html).

If you have multiple locations, you can move inventory based on your reorder point and preferred stock level to replenish another location through these forms:

-   **Replenish Location By Inventory Transfer** - Based on the quantities you enter on this worksheet, NetSuite creates an inventory transfer and updates your inventory for each location.
    
-   **Replenish Location By Transfer Order** - This form enables you to create multiple transfer orders to schedule and track inventory replenishment across your locations.
    

See [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html).

Depending on the Manufacturing features you use, you can build assemblies to generate stock and add them to your inventory. See [Manufacturing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1506100009.html).

## Sell and Fulfill Inventory {#bridgehead_161972153069}

Selling and fulfilling items from your inventory affects your stock levels, accounting records, and item commitment. You can track backordered items through reports and receive alerts for underwater inventory. See [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html).

## Commit Inventory {#bridgehead_1527531600}

Depending on your settings for item commitment preferences, you can allocate inventory to open orders by using the [Committing Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3765928460.html) form. If you want to create and run a schedule for committing orders, use the Commit Order Schedule form. See [Creating Commit Orders Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4713119268.html).

## Reallocate Items {#bridgehead_N2259472}

When you receive inventory from your vendor, those items are committed to existing open orders or backorders. You can use the Reallocate Items transaction to manually reallocate these items to different open orders than the ones they are automatically allocated to.

You can reallocate items to orders as needed instead of using the item commitment allocated automatically.

For example, you receive a shipment of widgets from your vendor. These widgets are automatically allocated to existing open orders. On the same day, a customer calls you in need of widgets. You can enter an order for that customer and then reallocate the new shipment of widgets to fill the new order.

See [Reallocating Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263567.html) topic.

## Process Items in a Warehouse {#bridgehead_3811939098}

You can use a combination of item, manufacturing, and inventory management features to set up bar coding, build assemblies, or track bins. You can process inventory in your warehouse and get them ready to ship to customers. See [Warehouse Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317586.html).

### Related Topics

-   [Inventory Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161970666917.html)
-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Inventory Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html)
-   [Inventory Management with Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162100850596.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
