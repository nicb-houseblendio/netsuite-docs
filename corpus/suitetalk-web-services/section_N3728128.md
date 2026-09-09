---
id: "section_N3728128"
type: "section"
title: "Serialized Inventory Item"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Serialized Inventory Item"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3728128.html"
anchors: ["bridgehead_N3728140", "bridgehead_N3728363", "bridgehead_N3728400", "bridgehead_N3728409", "bridgehead_N3728421", "bridgehead_N3728433", "bridgehead_1541691937", "bridgehead_N3728445"]
sha256: "555ea5b6a7a4ddf282cf37a0ed86a778d06a78322dcb3d90ecb3215006b55173"
---

Serialized inventory item records are used to track information about items which you maintain a stock of. Note that you must first enable serialized inventory items in your NetSuite account before you can access this record type. To enable serialized inventory items, go to _Setup > Company > Enable Features_. On the Items & Inventory subtab, under Inventory, check the Serialized Inventory box.

For more information, see [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html).

## Supported Operations {#bridgehead_N3728140}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3728363}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [serialized inventory item](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/serializedinventoryitem.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3728400}

## Working with Serialized Inventory Items Sublists {#bridgehead_N3728409}

The SOAP Schema Browser includes all sublists associated with the serialized inventory item record. See the following information for usage notes regarding specific serialized inventory item sublists. Usage notes are not provided for every sublist type.

## SerializedInventoryItemLocations {#bridgehead_N3728421}

To provide a locations list, the Multi-Location Inventory feature must be enabled at Setup > Company > Enable Features > Accounting. Otherwise, single entries for each corresponding field can be entered in the regular record fields.

## SerializedInventoryItemNumbers {#bridgehead_N3728433}

This list is read-only and displays the serial number and quantity on hand for the lot numbered inventory item.

## Merchandise Hierarchy Sublist {#bridgehead_1541691937}

This sublist is available if the Merchandise Hierarchy feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Items & Inventory subtab.

## Accessing Inventory Detail Data {#bridgehead_N3728445}

If the Advanced Bin / Numbered Inventory Management feature is enabled, serialized inventory items include data from a new [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord. This subrecord includes quantity on hand and quantity available values per serial number, and if applicable, per bin number.

If this feature is enabled, you must use the 2011.2 endpoint or later to access the newly supported subrecord and the most up to date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
