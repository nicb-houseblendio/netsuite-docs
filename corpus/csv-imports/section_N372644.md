---
id: "section_N372644"
type: "section"
title: "Notes about Items Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Notes about Items Imports"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html"
anchors: ["bridgehead_N372739", "bridgehead_N372768", "bridgehead_N372811", "bridgehead_N372857", "bridgehead_N372898", "bridgehead_1493368236", "bridgehead_1203070955"]
sha256: "f3345a0046e7e053bdde374a2ce9089b7715b27191f7d0137cf66eea71902bbc"
---

The following information may apply to your items imports:

-   [Import of Inventory Detail Data Currently Not Supported](#bridgehead_N372739)
    
-   [Unique Item Lookups by Internal ID and External ID](#bridgehead_N372768)
    
-   [Updating Inventory with Imported Items Data](#bridgehead_N372811)
    
-   [Updating Vendors on Items](#bridgehead_N372857)
    
-   [Updating Locations on Items](#bridgehead_N372898)
    
-   [SaaS Metric Tracking in Items Import](#bridgehead_1203070955)
    

## Import of Inventory Detail Data Currently Not Supported {#bridgehead_N372739}

When the Advanced Bin / Numbered Inventory Management feature is enabled, the following types of items include an Inventory Detail subrecord in the user interface: Assembly/BOM Item (when Use Bins is set to True), Lot Numbered Assembly/BOM Item, Serialized Assembly/BOM Item, Inventory Item (when Use Bins is set to True), Lot Numbered Inventory Item, and Serialized Inventory Item.

The Inventory Detail subrecord includes quantity on hand and quantity available values per bin number and per serial/lot number. Import of this subrecord's data is not currently supported. If you enable the Advanced Bin / Numbered Inventory Management feature, CSV import of the types of items listed above may result in incomplete data. For details about this feature, see [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html).

## Unique Item Lookups by Internal ID and External ID {#bridgehead_N372768}

To help eliminate ambiguous or missed lookups, the Import Assistant lets you reference an Item's Internal ID or External ID.

-   The Internal ID can be obtained by performing an Item saved search and exporting the results to CSV.
    
-   The External ID is similar to handle, and can be set to any string during add, but must be unique across all items.
    

For more information, see [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html).

## Updating Inventory with Imported Items Data {#bridgehead_N372811}

After you have completed an import of items, you can use the Adjust Inventory Worksheet to update inventory levels. For more information, see [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).

## Updating Vendors on Items {#bridgehead_N372857}

You can use the Import Assistant to update Vendor sublist information for items. For these updates, depending on your setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option, you can overwrite items' existing vendors sublists, or you can selectively update based on a key of Vendor name.

You also can use an alternate method to set preferred vendors for items through a CSV import. The Import Assistant supports the addition of a Preferred Vendor column to an Items CSV file. If the vendor specified in this field currently is on the vendor list, the import marks it as preferred; if it is not on the list, the import adds it. This method is available even if the Multiple Vendors feature isn't enabled.

Important:

If your CSV file defines more than one vendor as preferred for an item, the last vendor listed is the one that is marked as preferred by the import.

## Updating Locations on Items {#bridgehead_N372898}

You can use the Import Assistant to update location sublist information for items, when the Multi-Location Inventory feature is enabled. The fields that are updatable per location are Preferred Stock Level, Quantity on Hand, and Reorder Point. Also, if the Demand Planning feature is enabled, additional demand planning fields are available for items where the Time Phased replenishment method is used. See [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html).

After you have completed an import of items for multiple locations, you can use the Transfer Inventory form or Transfer Orders to move inventory among locations as necessary. For information, see [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html).

The Location sublist is a keyed sublist, based on Internal ID, External ID, or Location name. Updates of this sublist vary depending on your setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option.

## Importing Default ATP Method Data {#bridgehead_1493368236}

As of 2017.1, you can use the Import Assistant to import default available to promise (ATP) methods when you import inventory items, and you have the Available to Promise feature enabled in your account. For information about the Available to Promise feature, see [Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300269.html).

## SaaS Metric Tracking in Items Import {#bridgehead_1203070955}

The Items Import also supports the following software-as-a-service (SaaS) fields for accounts with the SaaS Metric Reporting feature enabled.

-   **SaaS Metric Tracking** - It is a field, and if the value is set to true, then the next two fields are also made available.
    
-   **SaaS Metric Start Date** - Required field. Here you set up the date you want to start tracking SaaS metrics.
    
-   **SaaS Metric End Date** - Optional field. Here you can set a date to stop the tracking. This way you can avoid errors in reporting, as you have better control of the range of data included in the report.
    

For more information about this fields, see [SaaS Metric Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5162432206.html).

The fields are supported for the import of the following Item types.

-   Non-inventory Item for Sale
    
-   Non-inventory Item for Resale
    
-   Service Item for Sale
    
-   Service Item for Resale
    
-   Inventory Item
    
-   Lot Numbered Inventory Item
    
-   Serialized Inventory Item
    
-   Kit/Package Item
    
-   Matrix Items
    

For more information about the Item types, see [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html). For more information about importing Items, see [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html).

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html)
-   [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html)
-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
