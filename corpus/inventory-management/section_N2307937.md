---
id: "section_N2307937"
type: "section"
title: "Returned-Item Costing Using Multi-Location Inventory"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Multi-Location Inventory > Returned-Item Costing Using Multi-Location Inventory"
parent: "section_N2303574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307937.html"
anchors: []
sha256: "f26410ef555ca33b0e042e109a1f761b2b1e289baf686af33fb37293be986f69"
---

With the Multi-Location Inventory feature, the method for tracking costs for items returned by customers depends on when you started using NetSuite.

Important:

Using the new costing method can affect historical costing. For example, costing on some or all historical transactions may be recalculated using the new method in the following cases:

-   When you edit an existing transaction and save it
    
-   When NetSuite performs a requested inventory costing calculation correction
    

For more details on ways the new costing method may affect historical costing, please contact NetSuite Customer Support.

-   If you began using NetSuite with Version 2007.1.0, NetSuite uses the exact cost from the original sale for returns that are linked to the sale. This is true even if the sale is associated with a different location than it is returned to. If you are not restocking, NetSuite uses the average cost at the location you are returning to.
    
-   If you began using NetSuite _prior to Version 2007.1.0_, returned-item costing uses the cost identified for the location it is being returned to.
    

For example, costs for widgets at two locations are as follows:

-   Location A widget cost: $10
    
-   Location B widget cost: $12
    

If a widget is sold from Location A and is returned to Location B, what is the cost tracked for the returned widget?

-   If you began using NetSuite with Version 2007.1.0, the returned-item cost shows as $10.
    
-   If you began using NetSuite prior to Version 2007.1.0, the returned-item cost shows as $12.
    

If your account uses the older returned-item costing method but you prefer the new method, you can choose to activate exact costing by location for returned items in your account. For more information about changing returned-item costing in your account, please contact NetSuite Customer Support.

For serialized inventory, if the return is not linked to a sale or if the exact-cost preference is not set, NetSuite applies the average cost at that location for the serial number on the return. If the serial number has not been received at that location, then the cost applied is zero. In this case, you must use the Return Cost Override field on the item receipt to enter the correct cost.

For more information about item costing, see [Item Return Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html).

### Related Topics

-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Non-Available Inventory Settings for Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307648.html)
-   [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html)
-   [Item Settings and Stock Levels for Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305626.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)
-   [Setting the Inventory Level Warnings Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2254698.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
