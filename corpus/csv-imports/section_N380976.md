---
id: "section_N380976"
type: "section"
title: "Imports Using Quantity Pricing Schedules Example"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Pricing Data for Items > Imports Using Quantity Pricing Schedules Example"
parent: "section_N377331"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N380976.html"
anchors: ["bridgehead_N381003", "bridgehead_N382438"]
sha256: "df44d4ede0d9c7956edb0f27021f985408d808b7a0fa2891c02ae69f3d4bf9b6"
---

Quantity pricing schedules are templates that allow you to automatically apply quantity discounts to an item. For example, a schedule defined as Schedule 1 might automatically create a 10 percent discount when a customer buys 15 of your items. For more on quantity price schedules, including how to create them, see [Quantity Pricing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183677.html).

When an item to be imported uses a quantity pricing schedule, note that your CSV file should define a price only for a quantity of zero for that item. The pricing schedule creates the additional quantities. If you try to define a price for any quantity besides 0 for an item associated with a schedule, your import fails.

## Multiple Files Import {#bridgehead_N381003}

If you're using multiple CSV files, you should create one file for the body data and a second file for the pricing data.

The primary file should include body fields such as the item's name, the tax schedule, any account data you want to use, and the quantity pricing schedule for any items that should use a schedule, as shown here:

| ExternalId | Item Name/Number | Quantity Pricing Schedule | Cost of Goods Sold (COGS) Account | Asset Account | Income Account | Tax Schedule |
| --- | --- | --- | --- | --- | --- | --- |
| item101 | Widget 1 | Schedule 1 | 1000 COGS | 1000 Asset | 1000 Income | S1 |
| item102 | Widget 2 | Schedule 2 | 1000 COGS | 1000 Asset | 1000 Income | S1 |
| item103 | Widget 3 | \- | 1000 COGS | 1000 Asset | 1000 Income | S1 |

The pricing file must include a separate row for each price level being created for each item. Two price levels can't be represented on the same row. For example, if you're importing two items and you want to define two price levels for each for Quantity 0, your file must include four rows.

Again, you don't define any quantities besides zero because you're relying on your pricing schedule to create them. If you try to define other quantities for an item associated with a schedule, the import fails. However, note that it is permissible to define different quantities in the file for item records that are **not** associated with a pricing schedule, as is the case with item103, below.

| ExternalId | Currency | Price | Price Level | Quantity |
| --- | --- | --- | --- | --- |
| item101 | USA | 125 | Base Price | 0 |
| item101 | USA | 100 | Alternate Price 1 | 0 |
| item102 | USA | 1999 | Base Price | 0 |
| item102 | USA | 1699 | Alternate Price 1 | 0 |
| item103 | USA | 550 | Base Price | 0 |
| item103 | USA | 525 | Alternate Price 1 | 0 |
| item103 | USA | 475 | Base Price | 5 |
| item103 | USA | 400 | Alternate Price 1 | 5 |

## Single File Import {#bridgehead_N382438}

To import similar data using one file only, you should include one row for each item. All of that item's data must be on the same row. (Note that the example below omits the item's name, which would be required if the Add data handling option was selected.)

| **ExternalId** | Quantity Pricing Schedule | Item Pricing 1: Currency | Item Pricing 1: Quantity | Item Pricing 1: Price Level | Item Pricing 1: Price | Item Pricing 2: Currency | Item Pricing 2: Quantity | Item Pricing 2: Price Level | Item Pricing 1: Price |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| item101 | Schedule 1 | USA | 0 | Base Price | 125 | USA | 0 | Alternate Price 1 | 100 |
| item102 | Schedule 2 | USA | 0 | Base Price | 1999 | USA | 0 | Alternate Price 1 | 1699 |
| item103 | \- | USA | 0 | Base Price | 1999 | USA | 0 | Alternate Price 1 | 1699 |

### Related Topics

-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Imports Using Multiple Price Levels and Quantities Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N379537.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
