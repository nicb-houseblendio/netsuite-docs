---
id: "section_N379537"
type: "section"
title: "Imports Using Multiple Price Levels and Quantities Example"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Pricing Data for Items > Imports Using Multiple Price Levels and Quantities Example"
parent: "section_N377331"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N379537.html"
anchors: ["bridgehead_N379680", "bridgehead_N380502", "bridgehead_3705045418"]
sha256: "6dc47badf29da3e83c740b2299bc6dc219467f0e4b76b31dad5fed38c651949e"
---

If both Multiple Prices and Quantity Pricing are enabled, the sublist area of the item record form includes a row for each price level, and a column for each quantity.

You can view this form at _Lists > Accounting > Items > New_ > Inventory Item (or any item type that uses pricing), and looking at the Sales / Pricing subtab.

Whenever you try to save a record of this type, the system enforces the following rule: A price level row that contains **any** values must include values for **all** defined quantity columns (all columns that have a number in the Qty field). Similarly, if a quantity column contains any values, it must include values for **all** price level rows that contain any other values.

For example, the following data could not be saved because two prices are missing in one row.

![Sales/Pricing subtab with two prices missing in one row.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ItemPricing_MissingPrices_2014_2.png)

Similarly, the following data could not be saved because two prices are missing in one column.

![Sales/Pricing subtab with two prices missing in one column.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ItemPricing_MissingPrices2_2014_2.png)

By contrast, the following record has fully populated pricing data and could be saved. Note that it is acceptable for the Alternate Price 3 row to be empty. A row can be empty, but if it contains any data, it must be fully populated.

![Sales/Pricing subtab with Alternate Price 3 row empty.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ItemPricing_CompletePrices_2014_2.png)

This rule also applies to your CSV import. If the Import Assistant can't create fully populated pricing rows and columns as shown in the third of the preceding screenshots, an error like the following occurs: 'Please enter missing price(s).' If you see this error and you believe that all required prices exist in your CSV file, the problem is likely that the file or the mapping were not set up correctly.

The 'enter missing price(s)' error can occur in the following situations:

-   During an import with update data handling that does either of the following:
    
    -   Adds a new quantity threshold for an item
        
    -   Adds a price to a previously unused pricing level
        
-   During an import that creates a new item that uses multiple quantities and price levels
    

To avoid problems, make sure that your CSV data is formatted and mapped correctly. Two approaches are supported - multiple-file and single-file. For the purposes of the following examples, assume you're trying to create the pricing data pictured in the preceding figure.

## Multiple Files Import {#bridgehead_N379680}

If you're using multiple CSV files, you should include one file for the body data and a second file for the pricing data.

The primary file should include required body fields such as the item's name and the tax schedule, plus any account data you want to include, as shown here:

| ExternalId | Item Name/Number | Cost of Goods Sold (COGS) Account | Asset Account | Income Account | Tax Schedule |
| --- | --- | --- | --- | --- | --- |
| item100 | Widget | 1000 COGS | 1000 Asset | 1000 Income | S1 |

The secondary file containing pricing data must repeat one row for **each** required quantity/price-level/price combination. Further, each of these rows must include a unique identifier for the item record, such as the repeating ExternalId values shown here:

| ExternalId | Currency | Price | Price Level | Quantity |
| --- | --- | --- | --- | --- |
| item100 | USA | 160 | Base Price | 0 |
| item100 | USA | 180 | Alternate Price 1 | 0 |
| item100 | USA | 200 | Alternate Price 2 | 0 |
| item100 | USA | 135 | Base Price | 12 |
| item100 | USA | 155 | Alternate Price 1 | 12 |
| item100 | USA | 180 | Alternate Price 2 | 12 |
| item100 | USA | 110 | Base Price | 24 |
| item100 | USA | 140 | Alternate Price 1 | 24 |
| item100 | USA | 170 | Alternate Price 2 | 24 |

When you do your mapping, you match the price columns to a single instance of the Item Pricing sublist fields.

![Field Mapping page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ItemPricing_MappingExampleMulti.png)

## Single File Import {#bridgehead_N380502}

If you're using a single CSV file for item body data and pricing data, all pricing fields for each item must be included in a single row. Each of the pricing groups should be represented by quantity, price level, price, and currency columns (unless you prefer to create a default value for some of these, such as currency, on the mapping page). The following example illustrates the first several columns for an item that includes nine pricing groups. Note that the columns for Item Pricing 4 through Item Pricing 9 are not pictured here.

| Item ID | Item Pricing 1: Quantity | Item Pricing 1: Price Level | Item Pricing 1: Price | Item Pricing 2: Quantity | Item Pricing 2: Price Level | Item Pricing 2: Price | Item Pricing 3: Quantity | Item Pricing 3: Price Level | Item Pricing 3: Price |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| item111 | 0 | Base Price | 160 | 12 | Base Price | 135 | 24 | Base Price | 110 |

On the Import Assistant Field Mapping page, each of these groups maps to a separate instance of the Item Pricing sublist. The following illustration shows how the first part of this mapping would look.

![Field Mapping page showing the first part of the mapping.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ItemPricing_MappingExample.png)

## Considerations when Data Handling is Set to Update {#bridgehead_3705045418}

When you're setting Data Handling to Update, be aware of the following:

-   If you want to update a single price on an item record, you must identify both the price level and the quantity associated with that price.
    
-   Remember that if you're doing an update that adds a new quantity to the record, you must identify a price for that quantity at every price level. Otherwise, the system generates an error about missing prices.
    
-   If you're doing an update that adds a price for a new or previously unused price level, you must identify prices for that price level for every quantity that's already used by the item record. Otherwise, the system generates an error about missing prices.
    

### Related Topics

-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Imports Using Quantity Pricing Schedules Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N380976.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
