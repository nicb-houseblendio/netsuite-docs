---
id: "section_N3202625"
type: "section"
title: "Item Revision"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Lists > Item Revision"
parent: "chapter_N3200673"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3202625.html"
anchors: ["bridgehead_1492454531", "bridgehead_1492454553", "bridgehead_N3202679"]
sha256: "1b666659d187e6d962c614adb79a4ed4bc6d3c12c59ddf6c4232eade73d2cd7d"
---

For help working with this record in the UI, see [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html).

The internal ID for this record is `itemrevision`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/itemrevision.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492454531}

Client SuiteScript is not supported for this record. It is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1492454553}

The item revision record is fully scriptable, which means that it can be created, updated, copied, deleted, and searched using SuiteScript.

## Code Sample {#bridgehead_N3202679}

The following sample shows how to create an item revision record:

          `function afterSubmit(type){                                              var itemRev = record.create({         type: record.Type.ITEM_REVISION     });     itemRev.setValue({         fieldId: 'name',         value: 'revision name 222'     });     itemRev.setValue({         fieldId: 'item',         value: '109'     });     itemRev.setValue({         fieldId: 'memo',         value: 'revision memo'     });     itemRev.setValue({         fieldId: 'effectivedate',         value: new Date('3/4/2012')     });     var id = itemRev.save();  }` 
        

### Related Topics

-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3200673.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
