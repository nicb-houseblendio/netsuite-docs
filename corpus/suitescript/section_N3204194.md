---
id: "section_N3204194"
type: "section"
title: "Custom Record"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Customization > Custom Record"
parent: "chapter_N3203672"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3204194.html"
anchors: ["bridgehead_1490211709", "bridgehead_1489687013", "bridgehead_1489782262", "bridgehead_1490042615"]
sha256: "bcabd03d08a8058b3d990c05a68b68e045ff1454330b1446fc46954cbc34fa2d"
---

A custom record can be used to collect information specific to the needs of your business. For example, you may want to keep track of training courses your employees have taken. Since a record type specific for this purpose does not exist in NetSuite, you could create a custom record type, titled Employee Courses, specifically to store the training course data.

The NetSuite UI enables you to create custom record types and work with instances of those types. You cannot use SuiteScript to create a custom record type or make changes to an existing custom record type. However, you can use SuiteScript to interact with instances of an existing custom record type.

For example, suppose your system had a custom record type called Feature. Each instance of that record type would be a feature record. You could use SuiteScript to update an existing feature record, delete a feature record, or create a new feature record. However, you could not use SuiteScript to alter the Feature custom record type.

For help working with this record in the UI, see [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/customrecord.html) for all internal IDs associated with this record, which includes a list of fields commonly available on instances of all custom records.

To interact with fields that were created for a specific record custom type, use the IDs for those fields. These IDs have a prefix of `custrecord`. For help finding these IDs, see [Internal IDs for Standard and Custom Fields in Field Level Help Window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416043804.html#subsect_90131056744).

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with records in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    
-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    

## Custom Record IDs {#bridgehead_1490211709}

Each custom record has a unique ID. This value is shown in the ID field on the custom record. When creating or interacting with an instance of a custom record type, you must use this ID.

Every custom record ID is prefaced by `customrecord`. If the ID was entirely system generated, it ends with a number (for example, `customrecord100`). If the ID was customized when the record was created, the ID may be more descriptive. To view a list of all IDs, go to _Customization > Lists, Records, & Fields > Record Types_. The values are shown in the ID column.

![The Record Types page with the ID column highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptRecordsGuide/CustomRecordIDList.png)

You can also see the ID on the record that represents the custom record type.

![The Custom Record Type page with the ID field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptRecordsGuide/CustomRecordID.png)

In SuiteScript 2.x, you use this value to set the [Record.type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296706984.html) or [CurrentRecord.type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637576636.html) field. Note that this guidance differs from the way you set this field if you are working with a standard NetSuite record type. When working with a standard record type, you set this field by using either the [record.Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273205732.html) or [CurrentRecord.type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637576636.html) enum.

See the [Code Sample](#bridgehead_1490042615) for examples.

## Supported Script Types {#bridgehead_1489687013}

Custom records (instances of a custom record type) are scriptable in both client and server SuiteScript.

All three user events are supported: beforeLoad, beforeSubmit, and afterSubmit.

## Supported Functions {#bridgehead_1489782262}

Custom records are fully scriptable - they can be created, updated, copied, deleted, and searched using SuiteScript.

## Code Sample {#bridgehead_1490042615}

In SuiteScript 2.x, you use the [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html) and [N/currentRecord Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html) to interact with custom records, the same as you would with a standard record type. Note that you use the custom record type's string ID when setting the [Record.type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296706984.html) field, as shown in the following example. For help finding this ID, see [Custom Record IDs](#bridgehead_1490211709).

The following sample shows how to work with instances of a custom record type with the script ID `customrecord_feature`. This sample assumes that this custom record type has fields with the field IDs `custrecord_priority` and `custrecord_risklevel`.

          `/**  * @NApiVersion 2.x  * @NScriptType UserEventScript  */  define([ 'N/record' ], function(record) {     function afterSubmit (context) {               // Use a string internal ID to identify the custom record type.          var rec = record.create({             type: 'customrecord_feature',             isDynamic : true         });          rec.setValue({             fieldId: 'name',             value: 'entry form redesign'         });          rec.setValue({             fieldId: 'custrecord_priority',             value: 1         });          rec.setValue({             fieldId: 'custrecord_risklevel',             value: 3         });          try {             var callId = rec.save();                 log.debug('Call record created successfully', 'Id: ' + callId);             } catch (e) {                 log.debug('sigh');                 log.error(e.name);             }         }         return {             afterSubmit: afterSubmit         }; });` 
        

### Related Topics

-   [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3203672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
