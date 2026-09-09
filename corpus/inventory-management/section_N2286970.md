---
id: "section_N2286970"
type: "section"
title: "Demand Planning"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Demand Planning"
parent: "chapter_N2285050"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html"
anchors: ["kaltura_player_141", "bridgehead_N2287026", "bridgehead_N2287086"]
sha256: "ca658f4c3b5737df290026f5d7c7469cbcce434ce7bd6449a4eafdbbf7e5bda9"
---

Warning:

To use Demand Planning you must enable Advanced Inventory Management.

You can use NetSuite Demand Planning to analyze your stock demand needs. This feature helps you figure out what you need to reorder and lets you create orders based on a supply plan that adds stock when you need it. This information is especially helpful for items with demand that fluctuates throughout the year.

You can see exactly when to reorder items and in what quantities, so you can maintain optimal stock levels. Demand planning helps you to keep the right amount of stock to fill orders without having extra inventory sitting around.

Demand Planning uses demand and supply plan records to track anticipated supply and demand.

Note:

When you use Demand Planning, you can also use the Available to Promise feature to calculate availability. See [Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300269.html).

<a id="kaltura_player_141"></a>

## Demand Plans {#bridgehead_N2287026}

A demand plan shows the expected future demand for an item based on past or projected demand.

You can create a demand plan automatically using the Calculate Demand Plan page. This page starts the process to review past demand for items and estimate upcoming demand.

You can forecast demand for items using one of the following methods:

-   Choose a time frame to review an item's sales history data and analyze previous sales trends, and forecast future sales with similar trends.
    
-   Use current demand from opportunities, quotes, and existing sales orders to forecast future sales. This method is not based on a calculated forecast.
    
    NetSuite uses this forecast data to estimate demand over a set period in the future and suggests a plan for orders.
    

## Supply Plans {#bridgehead_N2287086}

A supply plan shows the suggested schedule for purchasing or manufacturing more of an item. The supply plan lists suggested purchase and work orders to increase item supply, based on lead times and expected demand.

Safety stock level settings are considered in supply calculations. Also, the supply plan incorporates lead times, so you place orders for items in time to meet higher demands. Purchase orders generated from supply plans use the preferred vendor from the item record.

For assembly item supply plans, all levels of a multi-tier assembly are considered. NetSuite plans work orders for all sub-components of the build, as well as purchasing of required raw materials.

You can generate a supply plan from a demand plan using the Calculate Supply Plan page.

Using demand and supply plans helps you keep an optimal level of inventory for items with fluctuating demand.

For example, you sell a Deluxe Seasonal Widget that has a 15-day lead time and demand for the widget varies from month to month. To ensure you order and stock the right amounts of the widget, you can use demand planning to do the following:

-   Create a demand plan to review the sales history and project future demand for the widget. The demand plan shows demand across future periods, which may be high in April and August and low in October and May.
    
-   From the demand plan, create a supply plan. The supply plan shows when to create purchase orders to get more widgets based on the expected demand data.
    

Note:

You can process up to 10,000 items at a time for Demand Planning functions.

The general workflow for demand planning is as follows:

1.  Set up the feature. This includes enabling the feature, setting your preferences, and setting up item records.
    
    See [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html).
    
    After you enable the feature, the Demand Planning links appear on the Transactions subtab.
    
2.  Calculate demand for items.
    
    To calculate demand, at a minimum, identify a projection method, period type, historical period, and projection period. If you use Multiple-Location Inventory, identify a location as well.
    
    You can use projection methods like Linear Regression, Moving Average, Seasonal Average, and Sales Forecast.
    
    See [Calculating Item Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html) or [Manually Entering an Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2292418.html).
    
3.  Review the demand plan.
    
    Review the projected demand, as calculated, and make any needed changes.
    
    See [Viewing, Editing, and Deleting a Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291961.html).
    
4.  Generate supply plans for items. This includes choosing a start and end date to generate plans. If you use Multiple-Location Inventory, identify a location as well.
    
    You can generate a supply plan from a demand plan using the Calculate Supply Plan page. For more information, see [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html) or [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html).
    
5.  Review supply plans.
    
    Look at the suggested orders for item replenishment and make any needed changes.
    
    See [Viewing, Editing, and Deleting a Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294140.html).
    
6.  Place orders for items.
    
    Generate the suggested orders using the Order Items or Mass Create Work Orders page.
    
    For more information, see [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html) and [Mass Creating Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330082.html).
    

You can use NetSuite reporting to monitor your demand plans, supply plans, purchase orders, and work orders. For more information, see [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html).

### Related Topics

-   [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html)
-   [Monitoring the Demand Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291615.html)
-   [Monitoring the Supply Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293790.html)
-   [Distribution and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296427.html)
-   [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html)
-   [Time Fences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3848058018.html)
-   [Planning Action Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3865354301.html)
-   [Enabling the Advanced Inventory Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162488513759.html)
-   [Inventory and Assembly Item Support](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162212992098.html)
-   [Advanced Inventory Management FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4401903074.html)
-   [Setting Up Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2285514.html)
-   [Distribution Resource Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4049498070.html)
-   [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html)
-   [Supply Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156424975823.html)
-   [Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300269.html)
-   [Supply Chain Control Tower](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519947103.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
