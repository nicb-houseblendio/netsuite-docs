---
id: "section_N373888"
type: "section"
title: "Importing Demand Planning Data for Items"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Demand Planning Data for Items"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html"
anchors: []
sha256: "f21b18c221eed0ac5272ea08a9f44f34e03a7f59b04e7f15b05d784b6ed5041e"
---

The Demand Planning feature supports the use of demand plan and supply plan records to track anticipated supply and demand for inventory and assembly/BOM items. When this feature is enabled, you can include demand planning data in inventory items imports. If the Work Orders feature is also enabled, you can include demand planning data in assembly/BOM items imports.

Note:

You also can import data from Item Demand Plan transactions. See [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html).

The Import Assistant supports the import of values for the following fields related to demand planning. Review the notes in the following table before setting up your CSV files and mapping these fields on the Import Assistant Field Mapping page. You should read [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html) and review details about other items record fields in the SOAP Schema Browser.

| Field | Notes |
| --- | --- |
| Replenishment Method | **Reorder Point** is the default value for this field. You must set a value of **Time Phased** for each item you want to use with Demand Planning. When this value is set:
-   Orders are created based on item demand plans instead of the Advanced Inventory Management settings.
-   The Alternate Source Item, Demand Source, Fixed Lot Size, and Lot Size Method fields are available for writing if this value is used.
-   Other fields on the record that are used by Advanced Inventory Management to calculate demand are not writable. These unavailable fields are: Seasonal Demand, Build Point/Reorder Point, Preferred Stock Level Days, Safety Stock Level Days.
-   The Auto-Calculate settings are set to False and can't be changed for Build Point/Reorder Point, Preferred Stock Level.

 |
| Alternate Source Item | An alternate item to be used as the source of historical sales data used for demand planning. When this field is left blank, the source for historical data is the original item. Note: You can select only an item that is of the same item type to be an alternate source. For example, if the original item is an inventory item, the alternate source item must also be an inventory item. |
| Lead Time | The average number of days between ordering this item from the vendor and receiving it. If no value is set, the default value from the Inventory Management Preferences page is used. Note: To set a value for this field, you must set Auto-Calculate Lead Time to False. |
| Auto-Calculate Lead Time | indicating whether lead time is auto-calculated or based on a value set in the Lead Time field. By default set to True. |
| Safety Stock Level | The amount of an item that should be kept in stock at all times. When the Replenish Method field is set to Time Phased, this value can only be defined as a quantity of items, not as several days supply. If no value is set, the default value from the Set Up Inventory Management page is used. |
| Expected Demand Change | Used when an item's demand plan forecast method is set to Seasonal Change. The percentage used to augment the forecasted amount according to seasonal variations in demand. Format is numeric; you don't need to include the % sign, for example: **32.5**. |
| Lot Sizing Method | Possible values are:

-   **Lot For Lot** - Orders are suggested for procurement based on the exact projections for that day. The suggested order quantity may vary from day to day depending on demand calculations.
-   **Fixed Lot Size** - Orders are suggested for procurement based on a fixed amount or a multiple of the fixed amount.
-   **Periods of Supply** - Select this option to generate aggregated purchase orders or work orders based on the overall demand requirements extended over a designated period, such as weekly or monthly.

Note: If the Multi-Location Inventory feature is enabled, this field is in the Locations sublist on the Field Mapping page, and can have different values per location. |
| Fixed Lot Size | Used when Lot Sizing Method is set to **Fixed Lot Size**. The quantity that procurement of this item is always based on, regardless of demand projections. Note: If the Multi-Location Inventory feature is enabled, this field is in the Locations sublist on the Field Mapping page, and can have different values per location. |
| Periodic Lot Size Type | If you selected Periods of Supply as the lot sizing method, then make a selection in the Periodic Lot Size Type field:

-   Interval - Order aggregation starts when a requirement is established and continues for a fixed period defined in the Interval field.
-   Monthly - Order aggregation starts at the beginning of each month. The requirement date is always the first day of each month.
-   Weekly - Order aggregation starts at the beginning of each week. The requirement date is always the first day of the week as defined under Company Settings.

 |
| Periodic Lot Size Increment | In the Periodic Lot Size Increment field, enter a number from 1 to 90. The increment starts on the first day an order is required. From the first day, NetSuite aggregates all orders in the increment. Orders are placed on the first day of the period. |
| Supply Type | This field's value can only be set for assembly items when the Allow Purchase of Assembly Items preference is enabled at _Setup > Accounting > Accounting Preferences_. In this case, the value can be either **Build** or **Purchase**. Note: If the Multi-Location Inventory feature is enabled, this field is in the Locations sublist on the Field Mapping page, and can have different values per location. In the following cases, this field isn't available for import mapping:

-   When this preference isn't enabled, the value for assembly items is always **Build**.
-   The value for inventory items is always **Purchase**.

 |
|  |  |
| Demand Source | Determines where demand data is sourced for an item. Possible values are:

-   **Forecast from Demand Plan** - Demand is sourced only from the item's demand plan record.
-   **Select Entered and Planned Orders** - Demand is sourced from open orders and the expected ship date is used as the demand date. (If the item is a member of an assembly, demand for the assembly is included in demand calculations for the item.)

Note: If the Multi-Location Inventory feature is enabled, this field is in the Locations sublist on the Field Mapping page, and can have different values per location. |
| Preferred Stock Level | The Demand Source field determines where demand data is sourced for an item. Possible values are: **Forecast from Demand Plan** - Source only the item's demand plan record. **Entered and Planned Orders** - Source open orders and use the expected ship date as the demand date. If the item is a member of an assembly, demand for the assembly is included demand calculations for the item. **Order and Forecast** - Calculates demand for an item by including both the forecast amount and the amount on orders that have been entered.

-   Forecast demand for an item is calculated by combining the following: (Quantity forecast over time) + (quantity on sales orders and invoices entered)
-   The total forecast includes the forecast demand and the demand order quantities from transfer orders, work orders, and sales orders.

**Forecast Consumption** - Calculates demand for an item by subtracting from the forecast quantity any item quantities on orders entered. This removes duplication if an order is already included as part of a forecast.

-   Demand for an item is calculated as follows: (Quantity forecast over time) - (Quantity on sales orders and invoices entered)

Note: If the Multi-Location Inventory feature is enabled, this field is in the Locations sublist on the Field Mapping page, and can have different values per location. |

### Additional Information

-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html)
-   [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html)
-   [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
