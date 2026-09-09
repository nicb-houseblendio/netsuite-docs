---
id: "section_N3188833"
type: "section"
title: "Assembly Item"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Items > Assembly Item"
parent: "chapter_N3188218"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3188833.html"
anchors: ["bridgehead_1493306035", "bridgehead_1493306053", "bridgehead_1501522568", "bridgehead_1493305711"]
sha256: "12727a5c336af58e1ff0d672768e5064bacadffce1663d207160218e5784a749"
---

An assembly item is an inventory item made of several components, but identified as a single item. Assemblies are manufactured by combining raw materials you stock.

You create assembly item records to define the members of an assembly, then NetSuite enables you to track both the raw materials and the assembled items separately.

For example, an Wolfe Electronics sells a computer called Creativo 2400 that they assemble in-house. The Creativo 2400 computer is assembled from these inventory components: one Superion 2 GHz processor, one Creativo 2400 motherboard, 1 GB RAM, 80 GB Hard Drive, one Superion sound card, and one power supply.

NetSuite tracks the stock of the Creativo 2400 and each component item separately. Then, Wolfe can track the stock level of Creativo 2400 in inventory and available to ship to customers, and the quantity of materials available to assemble more.

For help working with this record in the UI, see [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html).

The internal ID for this record is `assemblyitem`. This record is also sometimes referred to as Build/Assembly.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/assemblyitem.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493306035}

The assembly item record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1493306053}

The assembly item record is fully scriptable - it can be created, updated, copied, deleted, and searched using server SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_1501522568}

The taxschedule field of the Members sublist is visible only in the UI when the Advanced Taxes feature is enabled.

The assembly item record includes the [Pricing Sublist / Pricing Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502207768.html).

## Code Samples {#bridgehead_1493305711}

The following sample changes the item name of an assembly.

          `var assembly = record.load({     type: record.Type.ASSEMBLY_ITEM,     id: 123 }); assembly.setValue({     fieldId: 'itemid',     value: 'new name' }); var recordId = assembly.save();` 
        

### Related Topics

-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3188218.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
