---
id: "section_N371212"
type: "section"
title: "Item Sublists Available for Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Item Sublists Available for Import"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html"
anchors: []
sha256: "3207f9c44f64e1cf310571368496cb041894f4008510806f6c124588d47c2c5a"
---

Item sublist data supported for import varies according to the type of item data to be imported, and the related features enabled. The following table indicates these limitations:

| Sublist | Notes |
| --- | --- |
| Bills of Materials | Available for the following import types:
-   Assembly Item
-   Serialized Assembly Item
-   Lot Numbered Assembly Item

Available if the Advanced Bill of Materials feature is enabled at _Setup > Company > Setup Tasks > Enable Features (Administrator)_, on the Items & Inventory subtab. |
| Bin Numbers | When Bin Management feature or Advanced Bin/Numbered Inventory Management enabled. Selectively updatable based on Bin Number key field. For Assembly/BOM Item and Inventory Item imports. Note: If you're importing bin records, you should complete this import before you import items with associated bin numbers. See [Bin Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394777.html). |
| Locations | When Multi-Location Inventory feature enabled.

Selectively updatable based on Internal ID, External ID, or Location.

(See [Updating Locations on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html#bridgehead_N372898).)

For Assembly/BOM Item and Inventory Item imports. |
| Members | For Assembly/BOM Item, Item Group, and Kit/Package Item imports. |
| Merchandise Hierarchy | Available for the following item types:

-   Inventory Item
-   Lot Numbered Inventory Item
-   Serialized Inventory Item

Available if the Merchandise Hierarchy feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Items & Inventory subtab. |
| Pricing | When any of Multiple Prices, Quantity Pricing, or Multiple Currencies feature enabled. Selectively updatable based on fields of Currency, Quantity, and Level, depending on enabled features (See [Keys for Item Pricing Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html#bridgehead_N377525).) |
| Related Items | When Web Site feature enabled. Not available for Non-Inventory Item for Purchase, Service Item for Purchase, Other Charge Item imports. For more information, see [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html). |
| Site Category | When Web Site feature enabled. Not available for Non-Inventory Item for Purchase, Service Item for Purchase, Other Charge Item imports. |
| Task Templates | When Project Management feature enabled. For Service Item for Sale imports. |
| Translation | When Multi-Language feature enabled. Selectively updatable based on Language key field. |
| Vendors | When Multiple Vendors feature enabled. Selectively updatable based on Vendor key field. For Inventory Item, Non-Inventory Item for Resale or Purchase, Service Item for Resale or Purchase, and Other Charge Item for Resale or Purchase imports, and Assembly/BOM Item when Allow Purchase of Assembly Items preference is enabled. Note that if multiple vendors are defined as preferred, the last one listed is the only one marked preferred by the import. See [Updating Vendors on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html#bridgehead_N372857). |

Every sublist on each record can optionally have a separate file. For imports that update existing Item records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html)
-   [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html)
-   [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html)
-   [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html)
-   [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
