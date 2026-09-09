---
id: "section_N3194671"
type: "section"
title: "Inventory Detail"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Inventory Detail"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3194671.html"
anchors: ["bridgehead_1492721830", "bridgehead_1492721957", "bridgehead_N3194712"]
sha256: "0fc9ddbab20ae51bfe6215da91bdc33aab0e5f836d0f2a29c36797890d69052d"
---

The inventory detail subrecord is available when the Advanced Bin / Numbered Inventory Management feature is enabled. This type of record stores values relating to bin numbers and serial/lot numbers for items, including line items on transactions. This data includes the quantity on hand and quantity available per bin number, or per serial/lot number, or when both are in use, per bin number/serial lot number combination.

In the UI, the inventory detail subrecord displays as a popup when you click the Inventory Detail body field or sublist field.

For help working with this record in the UI, see [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html).

The internal ID for this subrecord is `inventorydetail`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/inventorydetail.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492721830}

The inventory detail record is scriptable in client SuiteScript. Server scripts must access through the parent record.

## Supported Functions {#bridgehead_1492721957}

The inventory detail record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3194712}

Inventory Detail is scriptable from both the body field and the line item.

Inventory Detail is considered a subrecord in SuiteScript. For details on working with this subrecord type, see [Creating an Inventory Detail Sublist Subrecord Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4687606595.html). For general details on working with subrecords, see [SuiteScript 2.x Scripting Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623115.html).

### Related Topics

-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
