---
id: "section_N3196212"
type: "section"
title: "Manufacturing Operation Task"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Manufacturing Operation Task"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3196212.html"
anchors: ["bridgehead_1492794284", "bridgehead_1492794467", "bridgehead_N3196238", "bridgehead_N3196473"]
sha256: "4127149442d06a95f0a137428aa5bec8a03b0c562918f08ada2b0b481ca1693f"
---

The Manufacturing Routing and Work Center feature lets you specify a sequence of tasks required for the completion of a Work In Process (WIP) work order. This record represents a job that must be completed by a specific employee group. In the UI, generally these records are created automatically when you save a WIP work order that references a specific routing record - each step described in the routing record becomes an operation task record, viewable on the work order's Operations subtab. You can also manually create an operation task record by clicking the New Operation Task button on the work order's Operations subtab. You can view all existing manufacturing operation task records by going to _Transactions > Manufacturing > Manufacturing Operation Tasks_.

For help working with this record in the UI, see [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html).

The internal ID for this record is `manufacturingoperationtask`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/manufacturingoperationtask.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492794284}

The manufacturing operation task record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492794467}

The manufacturing operation task record is partially scriptable - it can be created, updated, deleted, and searched using SuiteScript. It cannot be copied.

## Usage Notes {#bridgehead_N3196238}

To work with the manufacturing operation task record, the Manufacturing Routing and Work Center feature must be enabled at _Setup > Company > Enable Features_, on the Items & Inventory subtab.

In the UI, the manufacturing operation task record is accessed by going to _Transactions > Manufacturing > Manufacturing Operation Tasks_. Alternatively, you can go to the Operations subtab of a WIP work order that uses the routing feature. The Operations subtab lists existing operation task records for that work order and allows you to create new operation task records.

Note these additional details:

-   This record supports client and server scripting.
    
-   All three user events are supported: beforeLoad, beforeSubmit, and afterSubmit.
    

-   To create a new manufacturing operation task record, you must reference a valid existing WIP work order, as shown in the [Code Samples](#bridgehead_N3196473) below.
    

## Code Samples {#bridgehead_N3196473}

When creating a manufacturing operation task record, you must use initValues to reference a valid existing WIP work order. For example:

          `var initValues = new Array(); initValues.workorder = '65'; var task = record.create({     type: record.Type.MANUFACTURING_OPERATION_TASK,     defaultValues: initValues }); task.setValue({     fieldId: 'title',     value: 'Some title' }); task.setValue({     fieldId: 'operationsequence',     value: 6 });  task.setValue({     fieldId: 'setuptime',     value: 30 }); task.setValue({     fieldId: 'runrate',     value: 20 }); task.setValue({     fieldId: 'manufacturingcosttemplate',     value: '1' }); task.setValue({     fieldId: 'manufacturingworkcenter',     value: '113' });                  var recId = task.save();` 
        

### Related Topics

-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
