---
id: "section_N2286205"
type: "section"
title: "Lead Time and Safety Stock Per Location"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Setting Up Advanced Inventory Management > Lead Time and Safety Stock Per Location"
parent: "section_N2285514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286205.html"
anchors: ["subsect_0420092639", "bridgehead_N2286674", "bridgehead_N2286694", "bridgehead_N2286709", "bridgehead_N2286755", "bridgehead_N2286770"]
sha256: "c5566b84d874144055e46f4d83f0841b6cad9080ccbdc0e7f2885032b079efcc"
---

You can choose to set a lead time and safety stock level for each location on an item record.

Safety stock is an additional quantity of an item held in the inventory to reduce the risk that the item will be out of stock. It acts as a buffer stock when sales are greater than planned or the supplier cannot deliver more items in the expected time.

Setting a lead time and safety stock level helps you track your inventory more accurately by allowing the following:

-   Account for lead times that vary between locations. For example, it takes the vendor 5 days to deliver to Location A, but 10 days to deliver to Location B.
    
-   Turnover in Location A is low, so only 3 units are required for safety stock. Location B sells two times as many and the safety stock level is 6 units.
    

Note:

To use this preference, enable Multi-Location Inventory and Advanced Inventory Management. It affects items with all replenishment methods: Reorder Point, Time-Phased, Material Requirements Planning, and Master Production Scheduling.

The lead time is calculated based on receipt lines that show a location pulled from the purchase order.

If you use Advanced Inventory Management and auto-calculate lead times, the lead time is calculated based on item receipts for each specific location. This lead time is calculated **for the receipt location**. It is based on the time elapsed between the date of the purchase order and the date of the item receipt.

For example, you enter the following:

-   A purchase order dated 1/1 for item #1234 in Location A.
    
-   A receipt dated 2/1 to receive the purchase order in Location B.
    

The lead time for Location B is calculated as 31 days. The lead time for Location A is not calculated from these transactions.

To use the new preference, go to _Setup > Accounting > Inventory Management Preferences_. Check the Lead Time Per Location box and then click Save.

Note:

This preference is unavailable if you use the preference to Centralize Purchasing in a Single Location.

The the Lead Time Per Location preference reorders items based on the lead time, safety stock, and the reorder point set for each location. Then, NetSuite functions as follows:

-   NetSuite automatically calculates item reorder point and time phased replenishment for each location.
    
-   NetSuite determines the lead time by location by referencing the three most recent purchase orders and receipt sets for purchase orders for a location.
    

Important:

To use the Lead Time Per Location preference, you must specify a location for each line item of a purchase order you enter. If a purchase order line does not identify a location, the lead time is not populated.

For example, transactions with the following data are entered:

| **PO** | **Location** | **PO Date** | **Receipt** | **Location** | **Receipt Date** |
| --- | --- | --- | --- | --- | --- |
| 1 | Location A | 4/1/2011 | 111 | Location A | 5/1/2011 |
| 2 | <blank> | 5/1/2011 | 121 | Location A | 6/25/2011 |
| 3 | Location A | 6/1/2011 | 131 | Location A | 7/23/2011 |

The items received on receipt #121 are not used in lead time calculations for Location A because purchase order #2 does not have a location.

## Replenishment Methods {#subsect_0420092639}

For all replenishment methods, the Use Lead Time and Safety Stock per Location preference determines how items are replenished based on the lead time and safety stock. NetSuite can automatically calculate (along with other calculations) the location specific lead times and safety stock, based on pre-set time intervals in the [Inventory Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162488535703.html) . You can also trigger an ad-hoc calculation by pressing the **Submit & Calculate** button on the preference page.

-   **Reorder Point** replenishment: NetSuite automatically calculates replenishment based on the Reorder Point and the Preferred Inventory Level for each location. To learn more, see the [Advanced Inventory Management FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4401903074.html).
    
-   **Time-Phased** replenishment: NetSuite automatically calculates replenishment based on the Demand Planning feature setup. To learn more, see [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html).
    
    Note:
    
    The location safety stock level (quantity) is used. Safety Stock Level (Days) is not supported for time-phased preferences.
    
-   **Material Requirements Planning and Master Production Scheduling** NetSuite automatically calculates replenishment based on the supply planning setup. To learn more, see [Setting Up Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159172130393.html).
    

## Purchase Orders {#bridgehead_N2286674}

New purchase orders automatically populate the lead time based on the location lead time **only when location is identified on each line item**. The expected receipt date is calculated based on the lead time of the location on the purchase order.

Purchase orders with no location for a line item settle lead time for the location specified in the purchase order header. When a location is selected for both the transaction header and each line item, the location on the item line is used for calculations.

## Work Orders {#bridgehead_N2286694}

-   **Work Orders** - The Lead Time per Location preference functions differently for Reorder Point replenishment, than for the other replenishment methods.
    
-   **Reorder Point** - To determine the production start and end dates of the new work orders, NetSuite uses the Purchase Lead Time for the work order location.
    
-   **Time-Phased, Material Requirements Planning and Master Production Scheduling** replenishment - To determine the production start and end dates for new work orders, NetSuite uses location-specific work order lead times.
    

## Demand Planning {#bridgehead_N2286709}

If you use Demand Planning with Lead Time per Location, you can enter a work order lead time per location. Then, on the Generate Supply Plan page, the lead time is based on the lead time of the location that requires the goods.

When the Lead Time per Location is enabled, the following occurs:

-   A supply source purchase uses the location lead time.
    
-   A supply source work order uses the location work order lead time.
    
-   The location Safety Stock Level (Quantity) is used.
    
    Safety Stock Level (Days) is not supported for the Demand Planning feature.
    

## Time-Phased Replenishment Items {#bridgehead_N2286755}

If an item's replenishment method is time-phased, you can enter a work order lead time per location for an assembly item. However, you cannot enter a work order lead time per location for an assembly item with the reorder point replenishment method.

For example, a planned order of Deluxe Widgets is requested and these widgets use time-phased replenishment. The requirement date is 5/18. The order date is determined based on the lead time setting per location.

## Check Item Availability and Gross Requirement Inquiry {#bridgehead_N2286770}

The Lead Time per Location preference functions differently with the Multi-Location Inventory and Demand Planning features. NetSuite uses the setting in the Safety Stock field for the location to calculate lead times. This is true for both the Gross Requirements Inquiry and Check Item Availability data.

### Related Topics

-   [Inventory Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162488535703.html)
-   [Setting Up Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2285514.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
