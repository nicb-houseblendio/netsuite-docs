---
id: "section_N2303574"
type: "section"
title: "Multi-Location Inventory"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Multi-Location Inventory"
parent: "chapter_N2250682"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html"
anchors: ["bridgehead_162032402081", "bridgehead_162032406853", "subsect_1006022628", "bridgehead_162032472912"]
sha256: "9d2220564019625f3811834da07b0922e02cd73424342838e31f07356e1ab20b"
---

If you stock, sell, and fulfill items in more than one location, you can use the Multi-Location Inventory feature to manage the inventory for your distinct locations. This feature lets you associate each item and transaction with a location. You can track the purchase, sale, stock level and value of items in your locations, as well as transfer inventory between locations.

## Serialized Inventory for Multiple Locations {#bridgehead_162032402081}

When you use multiple locations to track inventory, you track serial numbers by location. A serial number can be in stock at only one location. Make sure that transactions with serialized items must have the correct location selected.

For the purchase of new serialized items, you must select a location and enter the serial numbers you want to receive. The quantity of serial numbers entered must equal the quantity of received items.

For the sale of serialized items, you can only sell a serial number from the location where it is in stock. If you attempt to sell a serial number from an incorrect location, you get notified when you try to save the transaction. If you have customized your forms to select inventory locations per line item, entering a serial number automatically selects the correct location where the number is located.

## Fulfillments for Multiple Locations {#bridgehead_162032406853}

If you use the Intercompany Cross-Subsidiary Fulfillment feature, changing locations on partially fulfilled order lines can cause of out-of-sync inventory counts. You should split items into multiple lines on each order by location.

For example, you have an order line for Item #2345 with quantity of 30. Location A is selected on that line. You fulfill only 20 of the items from Location A and you want to fulfill the rest from Location B. Instead of changing the location on that fulfillment line, you should close that line on the sales order. Then, you can edit the order to add a new line for the remaining quantity of 10 and assign it to Location B. After you edit the order, you can fulfill it from Location B.

## Other Features for Multi-Location Inventory {#subsect_1006022628}

When you enable Multi-Location Inventory, you can enable these additional features for inventory management and related settings, depending on your business requirements:

-   [Item Settings and Stock Levels for Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305626.html)
    
-   [Returned-Item Costing Using Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307937.html)
    
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
    
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)
    
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
    
-   [Advanced Item Location Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503666392.html)
    
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
    

The following features required to enable Multi-Location Inventory provide capabilities for inventory-related processes:

-   **Advanced Receiving** - Enables you to receive single or multiple items without billing them at the same time. Also provides the **Restock?** option when you receive returned items. For more information and other capabilities, see the following topics:
    
    -   [Receiving a Purchase Orders With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2412119.html)
        
    -   [LIFO/FIFO Inventory Costing and Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html)
        
-   **Advanced Shipping** - Enables you to fulfill single or multiple orders without billing them at the same time. See [Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224089.html).
    

## Multi-Location Inventory Setup {#bridgehead_162032472912}

To set up Multi-Location Inventory, complete the procedures in the following topics:

Important:

Before you enable the Multi-Location Inventory feature, you must fully ship or otherwise close all open orders.

After you enable the **Multi-Location Inventory** feature and distribute items, you cannot turn the feature off without contacting Customer Support.

1.  [Enabling Features for Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161963741628.html)
    
2.  [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html)
    
    For more information about adding locations, see [Inventory Setup with Locations and Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2252794.html) and [Non-Available Inventory Settings for Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307648.html).
    
3.  [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html)
    
4.  Depending on your inventory requirements, you may enable additional settings for inventory per location. See [Setting the Inventory Level Warnings Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2254698.html) and [Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504284372.html).
    

### Related Topics

-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Inventory Management with Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162100850596.html)
-   [Bin Management by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4713998969.html)
-   [Purchasing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html#bridgehead_N2251155)
-   [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
