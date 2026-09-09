---
id: "section_N3191993"
type: "section"
title: "Assembly Unbuild"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Assembly Unbuild"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3191993.html"
anchors: ["bridgehead_1492704608", "bridgehead_1492704636"]
sha256: "36e797a6b9690087920d68b5175a1fa378009a95dc06ea54cb4976b4c5adb462"
---

An assembly item is an inventory item made of several components, but identified as a single item. This type of item lets you define the members of an assembly and to separately track both the component items and the assembled items in inventory.

An assembly unbuild transaction records the physical taking apart of an assembly item back into its component items and the related inventory level changes. For each assembly unbuild, the assembly item stock level decreases and the member items' individual stock levels increase.

For details about this type of transaction, see [Building Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321340.html). For details about this type of item, see [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html).

For help working with this record in the UI, see [Unbuilding Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321882.html).

The internal ID for this record is `assemblyunbuild`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/assemblyunbuild.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492704608}

The assembly unbuild record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1492704636}

The assembly unbuild entry record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

### Related Topics

-   [Unbuilding Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321882.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
