---
id: "section_N2296427"
type: "section"
title: "Distribution and Demand Planning"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Demand Planning > Distribution and Demand Planning"
parent: "section_N2286970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296427.html"
anchors: ["procedure_N2296463", "bridgehead_N2296540", "bridgehead_N2296570", "bridgehead_N2296586", "svg_1", "svg_1background", "svg_1Layer_1", "svg_1Node_1", "svg_2", "svg_2background", "svg_2Layer_1", "svg_2Node_1", "bridgehead_N2296658", "svg_3", "svg_3background", "svg_3Layer_1", "svg_3Node_1", "svg_4", "svg_4background", "svg_4Layer_1", "svg_4Node_1", "bridgehead_4060805059"]
sha256: "327f11bdb2c4e977464cf219ca8221259d70f24c4526a6ec6d698c49e253a58e"
---

If your company handles distribution of assemblies, you can use Demand Planning to assist in your production and distribution.

Important:

The NetSuite [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html) (MRP) solution replaces Time-Phased Planning and offers more features and better performance.

New customers should use the [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html) (MRP) solution. Existing customers should plan to move from Time-Phased Planning to MRP.

Demand Planning is available for assemblies only when you use the Advanced Inventory Management **and** Work Orders features. For more information, see [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html).

## Supply Plans and Assembly Items {#procedure_N2296463}

When you use Demand Planning for assemblies, you can use a supply plan as a list of daily ordering recommendations. A supply plans is generated based on the following:

-   outstanding purchase orders, work orders, and transfer orders
    
-   safety stock
    
-   item demand
    
-   existing sales orders or forecasts from a demand plan
    

For more information, see [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html).

When you calculate supply plans for an assembly, the supply for all related components in the assembly's Bill of Materials is also evaluated. If a work order is suggested for an assembly, NetSuite evaluates determines if additional work orders for sub-assemblies or purchase orders for component items. Work orders that prompt component consumption of materials are evaluated for additional supply requirements of components. This is true when the demand source for sub-assemblies and components is set to Entered and Planned Orders.

## Supply Source for Assemblies {#bridgehead_N2296540}

If you use the Allow Purchases for Assemblies preference, you can determine whether to purchase or build needed assemblies on supply plans. This depends on the setting for the Supply Source field on the item record. For more information, see about the Supply Source field in [Entering Purchasing and Inventory Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2167714.html).

## Assembly Replenishment Strategies {#bridgehead_N2296570}

Distributors that sell assembly items can choose an inventory replenishment model that is an appropriate strategy to fit their needs. Two common methods discussed below are the Build to Stock method and Build to Order method. Both of these strategies are supported using the NetSuite Demand Planning feature.

For example, Smith Computers and Jones Computers are companies that sell similar systems, but they each use different supply chain strategies.

## Build to Stock {#bridgehead_N2296586}

Smith Computers sells their product at retail stores and they use a Build to Stock supply strategy.

When a customer comes in to make a purchase, the Smith Computers product is readily available at the store. There is no wait time. Customers pay for the product at the retail location and take it home immediately.

In the Build to Stock model, Smith Computers determines replenishment ordering requirements for components based on the forecast demand of the item's final assembly. This forecast demand of the final assembly is in the demand plan.

The graphic below shows that the Smith Laptop Assembly item is comprised of component items that have supply sources of both Buy and Build.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                               

To deploy a Build to Stock model, the following are suggested demand source selections for each item in the Bill of Materials structure.

<a id="svg_2"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           

Note:

Recommendations for subcomponents anticipate that you will be selling these components to customers.

## Build to Order {#bridgehead_N2296658}

Jones Computers sells their product to customers through their website and they use a Build to Order supply strategy.

With a Build to Order model, Jones computers are not readily available to consumers during sales order entry. Only after a customer places an order for a product, Jones assembles the item that will be delivered to the customer.

The Jones strategy does not require keeping large quantities of stock on hand, and having surplus stock is rare. Therefore, money is not tied up in idle inventory on shelves. However, customers must wait the two-week lead time necessary to build the product before they receive it.

Jones determines replenishment ordering requirements for components based on the forecast of existing sales for the item.

The following shows the member items in a Jones Laptop Assembly. When a customer places an order for a Jones Laptop Assembly, demand for these items increases.

<a id="svg_3"></a>

                                                                                                                 

To deploy a Build to Order model, the following are rsuggested demand source selections for each item in the Bill of Materials structure.

<a id="svg_4"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               

Note:

Recommendations for subcomponents anticipate that you will be selling these components to customers.

## Distribution Resource Planning {#bridgehead_4060805059}

The Distribution Resource Planning feature is available to facilitate resource planning across multiple locations and subsidiaries within a network. You can transfer items and materials between warehouses, factories, and retail stores when you establish networks to encompass locations that contribute to meeting demand. For more information, see [Distribution Resource Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4049498070.html).

### Related Topics

-   [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html)
-   [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html)
-   [Calculating Item Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html)
-   [Monitoring the Demand Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291615.html)
-   [Viewing, Editing, and Deleting a Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291961.html)
-   [Manually Entering an Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2292418.html)
-   [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html)
-   [Monitoring the Supply Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293790.html)
-   [Viewing, Editing, and Deleting a Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294140.html)
-   [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html)
-   [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html)
-   [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html)
-   [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html)
-   [Time Fences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3848058018.html)
-   [Planning Action Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3865354301.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); svgPanZoom('#svg\_2', { zoomEnabled: true, controlIconsEnabled: true }); svgPanZoom('#svg\_3', { zoomEnabled: true, controlIconsEnabled: true }); svgPanZoom('#svg\_4', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); svgPanZoom('#svg\_2').resize(); svgPanZoom('#svg\_2').fit(); svgPanZoom('#svg\_2').center(); svgPanZoom('#svg\_3').resize(); svgPanZoom('#svg\_3').fit(); svgPanZoom('#svg\_3').center(); svgPanZoom('#svg\_4').resize(); svgPanZoom('#svg\_4').fit(); svgPanZoom('#svg\_4').center(); },false);
