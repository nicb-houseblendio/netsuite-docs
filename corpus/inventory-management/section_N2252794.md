---
id: "section_N2252794"
type: "section"
title: "Inventory Setup with Locations and Multi-Locations"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Management Setup > Inventory Setup with Locations and Multi-Locations"
parent: "chapter_N2249539"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2252794.html"
anchors: ["bridgehead_N2253582", "bridgehead_N2253594", "bridgehead_N2253618"]
sha256: "f847eb5de4774c1bb22150b2d60c53a92f19222ac5d5b615d86626943e35d913"
---

You can track inventory on item records, even if you don't use locations on your account. If you have multiple locations, choosing to track each location can have a big impact on your inventory management. The following topics describe the inventory tracking options and how your location setup may affect them:

-   [Inventory Only](#bridgehead_N2253582)
    
-   [Inventory with Locations](#bridgehead_N2253594)
    
-   [Inventory with Multi-Location Inventory](#bridgehead_N2253618)
    

The following chart describes the ways you can track inventory depending on which features you use:

| Available Functionality | Inventory Only | With Locations | With Multi-Location Inventory |
| --- | --- | --- | --- |
| Create item records | yes | yes | yes |
| Use inventory level warnings | yes | yes | yes |
| Adjust inventory levels | yes | yes | yes |
| Track inventory costing | yes | yes | yes |
| Create location records | no | yes | yes |
| Track transactions by location | no | yes | yes |
| Identify a location on a transaction | no | yes | yes |
| Create sales reports filtered by location | no | yes | yes |
| Track stock of items by location | no | no | yes |
| Identify a location on each item record | no | no | yes |
| Fulfill orders from a distinct location | no | no | yes |
| Receive inventory to several locations | no | no | yes |
| Transfer items between locations | no | no | yes |
| Create inventory reports filtered by location | no | no | yes |
| Track inventory using bins on a per-location basis | no | no | yes |

## Inventory Only {#bridgehead_N2253582}

The basic setup involves tracking inventory without setting up locations. This setup is ideal if you have only one location where you receive, stock, and sell your items.

After you enable features for inventory management, you can create inventory item records to track inventory of items, parts, or finished goods, as well as associated costs. See [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html). If you have non-inventory items that you want to convert into an Inventory Item type, see [Converting Non-Inventory Items to Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2258046.html).

## Inventory with Locations {#bridgehead_N2253594}

The Locations feature enables you to define location records that identify each of your offices or warehouses. You can also create a hierarchy of locations to track information by locations within groups of locations.

For example, you can create a parent location called East Coast, then create sublocations for it called New York and Georgia. You could even create sublocations for the Georgia location called Atlanta Warehouse and Atlanta Sales Office.

To create location records, see [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html) or [Locations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263024.html).

Note:

Defining location records alone does not enable you to identify each item with a location. To track inventory across locations or set a preferred location, use the Multi-Location Inventory feature. See [Inventory with Multi-Location Inventory](#bridgehead_N2253618).

After you create location records, you can perform additional setup procedures:

-   On inventory item records, you can select a location to classify your items and limit the items that roles can access. For instructions, see [Restricting Access to Records by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265799.html).
    
-   Set the Allow Per-Line Locations preference to configure per-line classification of transactions. This preference lets you display the Location column in the Items sublist and on print documents. For instructions, see [Configuring Per-Line Locations for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162024160153.html).
    

For more information, see [Inventory Management with Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162100850596.html).

## Inventory with Multi-Location Inventory {#bridgehead_N2253618}

If you stock, sell, and fulfill items in more than one location, you can use [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html) to manage inventory for your distinct locations.

Note:

You cannot disable this feature manually after you enable it and distribute items. Contact Customer Support if you want to disable this feature.

The Multi-Location Inventory feature lets you associate each inventory item and transaction with a location. You can track purchasing costs, sales income, stock levels, and valuation for each item in each location. You can also transfer inventory between locations. When you generate reports, you can filter by location for inventory status, revenue, valuation, activity, and fulfillment status, depending on other features you use.

Note:

You should not use location records to identify areas within your warehouse, such as a bin, shelf, or dock. Doing so causes difficulties with fulfillments, LIFO and FIFO costing, and reporting. You should use a bins feature for this purpose. See [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html).

When you create item records, you can choose a preferred location. You can set reorder points and preferred stock levels per location to help with replenishment and planning operations. You can configure a preference that alerts you when your inventory reaches these levels. See [Setting the Inventory Level Warnings Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2254698.html).

If you enable the [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html) feature, you can automate demand-based inventory replenishment, which does not affect tracking inventory by locations. For other features associated with Multi-Location Inventory, see [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html).

### Related Topics

-   [Inventory Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161970666917.html)
-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Enabling Features for Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161963741628.html)
-   [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
