---
id: "section_N2304534"
type: "section"
title: "Distributing Inventory"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Management Setup > Distributing Inventory"
parent: "chapter_N2249539"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html"
anchors: []
sha256: "f474cd1e16813fca131efb938eba8133831f1e837c9ef83e63fc60337f5996e9"
---

As part of your Multi-Location Inventory setup, distribute any unallocated inventory before you can enter them on inventory transactions. After you enable the Multi-Location Inventory feature, unallocated inventory items are considered to be in a null location. The Inventory Distribution transaction allocates inventory from its original, unassigned state to one or more locations on your account. It updates item details and quantities for all affected locations.

Note:

Because an item's inventory level should be zero or positive prior to distribution, you should run the Reviewing Negative Inventory report before distributing inventory. See [Reviewing Negative Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2268458.html).

On the Inventory Distribution form, an item shows in the list for distribution if:

-   The item has not already been distributed.
    
-   The distribution is dated after the last inventory-affecting transactions.
    
-   The item has a non-zero quantity on hand.
    
-   It is an inventory item or assembly item.
    
-   The item is active.
    

Note the following guidelines before you distribute inventory:

Warning:

Do not delete or change inventory transactions dated prior to an inventory distribution, as this can cause difficulties maintaining accurate inventory data.

-   You should distribute inventory during non-peak business hours.
    
-   Your data is most accurate if you distribute all unassigned inventory at one time and make no changes to transactions dated before the distribution. If you change earlier transactions and then return to Distribute Inventory, the Undistributed column may show an incorrect or negative quantity. To correct for this error, you can submit an adjustment by going to _Transactions > Inventory > Adjust Inventory_.
    
-   Inventory is distributed only if the stock level is 0 or greater.
    

You can choose from the two ways to enter an inventory distribution:

-   [Simple Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304987.html) - Distribute inventory to a single location.
    
-   [Manual Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305248.html) - Specify the quantity you want to distribute to each of your locations.
    

### Related Topics

-   [Inventory Setup with Locations and Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2252794.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Multi-Location Inventory Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html#bridgehead_162032472912)
-   [Non-Available Inventory Settings for Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307648.html)
-   [Returned-Item Costing Using Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307937.html)
-   [Item Settings and Stock Levels for Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305626.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
