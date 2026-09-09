---
id: "section_N377331"
type: "section"
title: "Importing Pricing Data for Items"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Pricing Data for Items"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html"
anchors: ["bridgehead_N377525", "bridgehead_N379333"]
sha256: "14bf54ff542700b06106aeaeb7b413a503f0c706c36ab845c0d0216eb25f021b"
---

The way you import prices varies depending on the features enabled in your account. If your account uses Multiple Prices, Quantity Pricing, or Multiple Currencies, you use the Item Pricing sublist. Otherwise, your pricing data is fairly simple, and you map prices using the Purchase Price body field. This topic deals primarily with the Item Pricing sublist.

When using the sublist, be aware of the following:

-   The preferred column headers for item pricing in CSV files vary, depending on whether you plan to upload a single file or multiple files. For more information, see [Formatting for Item Pricing CSV Files](#bridgehead_N379333).
    
-   The Item Pricing sublist can be selectively updated based on key field values. The key fields vary depending on the pricing-related features that are enabled. For more information, see [Keys for Item Pricing Sublist](#bridgehead_N377525).
    
-   For multiple pricing levels, if the CSV file data includes a base price for an item, all discount or markup price levels are always calculated during import. You don't need to supply discount or markup price values, because the import process overrides any values specified in the CSV files.
    
-   If you're using both multiple price levels and quantity-based pricing, every quantity must have a price defined at every price level. For more details, including examples of how to set up your CSV files to accommodate these fields, see [Imports Using Multiple Price Levels and Quantities Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N379537.html).
    
-   For any items that have quantity pricing schedules applied to them, you need to specify only a price for quantity zero for the price levels that you're using. The import process calculates other quantity prices. If you try to specify a price for any quantity besides zero for an item with a pricing schedule, the import fails. For more details, including examples of how to set up your CSV files, see [Imports Using Quantity Pricing Schedules Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N380976.html).
    
-   For CSV updates to items with quantity-based pricing, base price updates don't result in updates to other price levels, unless import data specifies a quantity pricing schedule or schedules.
    
-   For multiple currencies, the Import Assistant calculates price levels for the base currency specified. The Currency field is required to be mapped for item pricing imports in accounts where the Multiple Currencies feature is enabled.
    
-   You shouldn't enable the Overwrite Sublists option for imports that include item pricing data. Enabling this option may result in errors when imported sublist data overwrites existing sublist values driven by body field values such as pricing schedule.
    
-   When multiple item-pricing fields (price level, currency, quantity, and price) are mapped for an import job, and a row has values for some of these fields but not for others, none of the values for pricing fields are imported for the row. The assumption is that the populated values for pricing fields are defaults, and the empty values in other pricing fields indicate that complete pricing data isn't available and so pricing field values should not be imported at all.
    

## Keys for Item Pricing Sublist {#bridgehead_N377525}

The import of pricing sublist data for items is supported when one or more of the following features are enabled: Multiple Currencies, Multiple Prices, or Quantity Pricing.

The Import Assistant can selectively update existing NetSuite records that match CSV file key field values. The key for this sublist's records is based on a unique field value or a unique combination of field values, depending on the enabled features. The following table describes possible key combinations.

| Enabled Features | Key Fields |
| --- | --- |
| Multiple Currencies only | Currency |
| Multiple Currencies, Multiple Prices | combination of Currency, Level |
| Multiple Currencies, Quantity Pricing | combination of Currency, Quantity |
| Multiple Currencies, Multiple Prices, Quantity Pricing | combination of Currency, Level, Quantity |
| Multiple Prices only | Level |
| Multiple Prices, Quantity Pricing | combination of Level, Quantity |
| Quantity Pricing Only | Quantity |

## Formatting for Item Pricing CSV Files {#bridgehead_N379333}

The formatting of CSV import files differs for multiple file and single file uploads of item pricing data. It may also vary depending on the features enabled in your account. To see how you might set up your files, refer to [Imports Using Multiple Price Levels and Quantities Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N379537.html) and [Imports Using Quantity Pricing Schedules Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N380976.html).

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html)
-   [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html)
-   [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html)
-   [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
