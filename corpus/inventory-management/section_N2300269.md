---
id: "section_N2300269"
type: "section"
title: "Available to Promise"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Available to Promise"
parent: "chapter_N2285050"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300269.html"
anchors: ["subsect_163051931523", "subsect_163051959111"]
sha256: "424b83764e2c37067657e031df52bf5623208632ce0fe9a5e665c09637e53a3d"
---

The Available to Promise feature gives purchasing and sales departments visibility into the projected ship date of goods during the quote and order processes. It enables you to check item availability based on outstanding transfer orders, purchase orders, work orders, and sales orders.

For example, on April 1, your customer wants to place an order for 100 bicycles. You need to know how soon the order can be fulfilled. Using Available to Promise, you check item availability to find the earliest date that all 100 bicycles will be available in stock. According to NetSuite calculations, by April 15, only 50 bicycles will be available. However, by May 1, all 100 items on the order can be fulfilled. This information enables you guarantee the customer that they will receive the items they need by the promised date.

To determine availability, NetSuite reviews the following information:

-   The quantity of items expected to be received on purchase orders, work orders, and transfer orders based on their expected receive date.
    
-   The quantity of items expected to be fulfilled on sales orders and transfer orders based on their expected ship date.
    

Knowing the number of items that will move in and out of inventory each day provides you with a virtual available quantity calculation. This virtual quantity describes the number of items that are available to fulfill orders for that day. These calculations can also be used to track the available quantity for any date. This information helps you to find a date when the quantity to fill an order will be available. For more information, see [Available to Promise Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2301636.html).

Available to Promise differs from Demand Planning in the following way:

-   Demand Planning provides supply recommendations based on a forecast or sales orders in a Build to Order or a Build to Stock environment.
    
-   Available to Promise provides demand date recommendations based on available firmed supply.
    

The Available to Promise feature is accessible only when you have enabled the Demand Planning feature. For more information, see [Enabling Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300611.html).

Important:

A user must have the Check Item Availability permission for their role to use the Available to Promise feature. The View setting is the default for this permission. For more information, see [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html).

After item records are set up, you can review item availability either on transaction lines or using the Check Item Availability page.

## Check Item Availability Page {#subsect_163051931523}

Use the Check Item Availability page to review the supply and demand of an item based on the projected receipt and ship date. You can review the item supply and demand on outstanding sales orders, work orders, and transfer orders.

For example, a customer requesting a quote or placing an order asks for a projected shipment date. The information about the Check Item Availability page provides the earliest date that the full item quantity will be available. You can then pass this information about to the customer. You can also review the projected inventory for handling projected stock shortages.

## Check Item Availability Popup Window {#subsect_163051959111}

You can access the Check Item Availability popup window from a quote, opportunity, or sales order. The popup window displays the same data as the Check Item Availability page. For more information, see [Checking Item Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2302738.html).

### Related Topics

-   [Available to Promise Earliest Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159250317916.html)
-   [Available to Promise in Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0929025924.html)
-   [Enabling the Advanced Inventory Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162488513759.html)
-   [Inventory and Assembly Item Support](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162212992098.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
-   [Distribution Resource Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4049498070.html)
-   [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html)
-   [Supply Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156424975823.html)
-   [Supply Chain Control Tower](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519947103.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
