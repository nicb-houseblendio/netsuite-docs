---
id: "section_N3192160"
type: "section"
title: "Bin Transfer"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Bin Transfer"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3192160.html"
anchors: ["bridgehead_1492705356", "bridgehead_N3192201"]
sha256: "bcaa9dd7dca8c766ccb4d2a5280d6bf11801112cea898048d0358eb57d71a864"
---

You can record a bin transfer to move items between bins within a warehouse.

For example, at your East Coast location, you stock item #AB123 in two bins: bin #3003 and #4004. There are currently 100 of the item in each bin. You can enter a bin transfer to record the transfer of 50 items out of bin #3003 and into bin #4004.

Recording a bin transfer does not post to your chart of accounts and has no financial impact. The transfer only updates the quantity on hand in each bin for the items transferred.

On the bin transfer record, identify the item, the bin the item is in, the bin the item will move into and the quantity to be moved.

For help working with this record in the UI, see [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html).

The internal ID for this record is `bintransfer`.

The bin transfer record contains a subrecord: [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3194671.html). For details about subrecords in SuiteScript, see [SuiteScript 2.x Scripting Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623115.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/bintransfer.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492705356}

The bin transfer is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_N3192201}

The bin transfer record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

### Related Topics

-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
