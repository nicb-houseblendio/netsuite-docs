---
id: "section_N3196058"
type: "section"
title: "Item Supply Plan"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Item Supply Plan"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3196058.html"
anchors: ["bridgehead_1492787094", "bridgehead_1492787149", "bridgehead_N3196128", "bridgehead_N3196148"]
sha256: "e79ab79d3e04f0fed74747555cb5d0201ded4887e9c872b56f0d3ead5b9bb348"
---

The internal ID for this record is `itemsupplyplan`.

This record includes the Orders sublist.

For help working with this record in the UI, see [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html) and [Item Supply Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N417879.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/itemsupplyplan.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492787094}

The item supply plan is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492787149}

The item supply plan record is fully scriptable - it can be created, copied, updated, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3196128}

The item, location, and units body fields cannot be changed in update operations.

An item supply plan's receiptdate cannot be earlier than the orderdate.

The ordercreated field is read-only. It is set to True when an order is generated from an item supply plan.

## Code Samples {#bridgehead_N3196148}

The following sample creates an item supply plan.

          `function createItemSupplyPlanMinimal() {     var itemsupplyplan = record.create({         type: record.Type.ITEM_SUPPLY_PLAN,         isDynamic: true     })      itemsupplyplan.setValue({         fieldId: 'subsidiary',         value: 1     });      itemsupplyplan.setValue({         fieldId: 'location',         value: 1     });      itemsupplyplan.setValue({         fieldId: 'item',         value: 165     });        itemsupplyplan.setValue({         fieldId: 'memo',          value: 'memotest'     });      itemsupplyplan.setValue({         fieldId: 'unit',         value: 3     });          itemsupplyplan.selectNewLine({         sublistId: 'order'     });     itemsupplyplan.setCurrentSublistValue({         sublistId: 'order',         fieldId: 'orderdate',         value: '05/05/2012'     });      itemsupplyplan.setCurrentSublistValue({         sublistId: 'order',         fieldId: 'receiptdate',         value: '5/8/2012'     });      itemsupplyplan.setCurrentSublistValue({         sublistId: 'order',         fieldId: 'quantity',         value: 1     });      itemsupplyplan.setCurrentSublistValue({         sublistId: 'order',         fieldId: 'ordertype',         value: 'PurchOrd'     });        itemsupplyplan.commitLine({         sublistId: 'order'     });       var id = itemsupplyplan.save(); }` 
        

The following sample updates an existing item supply plan.

          `function updateItemSupplyPlan() {     var itemsupplyplan = record.load({         type: record.Type.ITEM_SUPPLY_PLAN,         id: 3     });       itemsupplyplan.setValue({         fieldId: 'memo',         value: 'memotest2'     });              itemsupplyplan.setSublistValue({         sublistId: 'order',         fieldId: 'receiptdate',         line: 4,         value: '11/3/2012'     });        var id = itemsupplyplan.save();  }` 
        

### Related Topics

-   [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html)
-   [Item Supply Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N417879.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
