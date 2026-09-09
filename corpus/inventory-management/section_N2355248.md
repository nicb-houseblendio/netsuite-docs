---
id: "section_N2355248"
type: "section"
title: "Current Inventory Snapshot Report"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Reporting > Current Inventory Snapshot Report"
parent: "chapter_N2353200"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2355248.html"
anchors: ["bridgehead_N2355411"]
sha256: "38df53c08af9dec600a8fa1db85635a2a698453c4334892beb51bd3fe57666fd"
---

The Current Inventory Snapshot report provides the latest inventory data at the time of report generation. You can use it to monitor inventory levels and determine ordering schedules.

The Current Inventory Snapshot report can help you pinpoint which items are low on stock and place orders accordingly.

For each inventory item, this report lists the item name, description, and preferred vendor. This report shows the following amounts for each location and in total:

-   **Reorder Point** - the stock level at which a new order for the item needs to be placed.
    
    When an item reaches its Reorder Point, a reminder is generated to purchase the item.
    
-   **Quantity On Hand** - the number of units of an item in stock.
    
-   **Quantity On Order** - the number of units of an item pending receipt from a vendor.
    
-   **Quantity Committed** - the number of units of an item reserved by unfulfilled sales orders.
    
-   **Quantity To Order** - the number of units of an item you need to order to maintain stock.
    
-   **Preferred Stock Level** - the optimum quantity to maintain in stock of an item.
    
    Along with the reorder point, this quantity is used to determine your replenishment needs on the Order Items page.
    

You can also choose to filter the report to show only items whose stock levels are at or below their Reorder Point.

Note:

If you use the Multi-Location Inventory feature, this report returns values that are grouped per location for most, but not all, fields. The values shown on this report are for each item's preferred location for the following fields:

-   **Average Cost** - total units available during a period divided by the starting inventory cost plus the cost of additions to inventory.
    
-   **Last Purchase Price** - the most recent transaction price at any location.
    
-   **Last Transaction Date** - the most recent transaction date at any location.
    
-   **Preferred Stock Level** - the optimum quantity to maintain in stock of an item. The ideal quantity is the amount you need to fulfill orders in a timely manner without either running out or overstocking.
    
-   **Reorder Point** - the stock level at which a new order for the item needs to be placed.
    
    When an item reaches its Reorder Point, a reminder is generated to purchase the item.
    
-   **In Transit** - items are in the process of being transported.
    

Also, a value does not display for these fields for items that do not have a preferred location set.

## To see a current inventory snapshot report: {#bridgehead_N2355411}

Go to _Reports > Inventory/Items > Current Inventory Snapshot_.

A message appears indicating that your report is loading. The status bar indicates the progress as your report loads. You can click **Cancel Report** to stop the report from loading.

On the filter toolbar, you can select the subsidiary and location or check the **At or Below Reorder Point** box.

The information in this report is similar to the information shown on the Order Items page. For more information, read [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html).

Note:

This report does not support reporting by period even when the Report by Period preference is set to All Reports. The Report by Period preference can be configured at _Home > Set Preferences_, on the Analytics subtab.

### Related Topics

-   [Drilling Down to Records or Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719130.html)
-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N698474.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
