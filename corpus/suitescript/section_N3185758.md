---
id: "section_N3185758"
type: "section"
title: "Project"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities > Project"
parent: "chapter_N3184398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185758.html"
anchors: ["bridgehead_3795842216", "bridgehead_3795842146", "bridgehead_3795845358", "bridgehead_1502829553", "bridgehead_3795903477", "bridgehead_4544339815"]
sha256: "019190d1c4caf23eac121dae52807cc58f6036729a57862284b8e64ced692c91"
---

Use the project record to manage company initiatives.

To use the project record, you must have the Projects feature enabled at _Setup > Company > Enable Features_, on the Company subtab. If you plan to do advanced project tracking, you must also enable Project Management. If you do not see the Project Management box, your company must first purchase the Project Management add-on from NetSuite.

To access the project record in the UI, choose _Lists > Relationships > Projects_(or Jobs).

For help working with this record in the user interface, see [Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3714107248.html).

The internal ID for this record is `job`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/job.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_3795842216}

The project record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_3795842146}

The project record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Field Definitions {#bridgehead_3795845358}

Note that the datecreated body field is a system-generated field that marks the date the record was created in NetSuite. You cannot change or override this field. If you need to capture 'date created' information that is not related to the date the record was created in NetSuite, create a custom field and set it to auto-default to today's date.

For more details on available fields, see the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/job.html), which lists all internal IDs associated with this record. For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

## Usage Notes {#bridgehead_1502829553}

The Time Tracking sublist is included with the project (job) record. It is an inline editor sublist.

Important:

If any case, task, or event record has more than 9500 time entries in the Time Tracking sublist, all cases include a static list of time entries. These static lists are not accessible to scripting. Attempts to script on Time Tracking sublists that are static lists of time entries will not return accurate results.

## Adding a Resource With Multiple Roles {#bridgehead_3795903477}

When using SuiteScript, the behavior of the Resources sublist differs slightly from the behavior in the UI. Specifically, in the UI, each line must have a unique value in the Name field. Further, in the UI, you can specify more than one role for each resource.

![The Resource Details tab showing three roles.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptRecordsGuide/ProjectResources.png)

With SuiteScript, if you want to add a resource that has two different roles, you set up your code as if you are adding two sublist records for that resource -- one for each role. The jobresource values are not required to be unique. The following example illustrates this technique. In this example, only two unique resources are being added, but because one resource has two roles, that resource is represented twice.

          `proj = record.create({     type: record.Type.JOB }); proj.setValue({     fieldId: 'companyname',     value: 'Launch' });  proj.setValue({     fieldId: 'subsidiary',     value: '1' });  proj.selectNewLine({     sublistId: 'jobresources' });  proj.setCurrentSublistText({     sublistId: 'jobresources',     fieldId: 'jobresource',     text: 'Employee Resource 1' });  proj.setCurrentSublistText({     sublistId: 'jobresources',     fieldId: 'role',     text: 'Staff' });  proj.commitLine({     sublistId: 'jobresources' });   proj.selectNewLine({     sublistId: 'jobresources' });  proj.setCurrentSublistText({     sublistId: 'jobresources',     fieldId: 'jobresource',     text: 'Employee Resource 1' });  proj.setCurrentSublistText({     sublistId: 'jobresources',     fieldId: 'role',     text: 'Project Manager' });  proj.commitLine({     sublistId: 'jobresources' });   var id = proj.save();  var savedProj = recordload ({     type: record.Type.JOB,     id: id }); savedProj.selectLine({     sublistId: 'jobresources',     line: '1' });  savedProj.setCurrentSublistText({     sublistId: 'jobresources',     fieldId: 'jobresource',     text: 'Employee Resource 2' });  savedProj.commitLine({     sublistId: 'jobresources' });  savedProj.save();` 
        

Note that after you complete the add operation, the Resources sublist in the UI looks the same as it would if you had manually added one line for the resource, with multiple roles specified on that line, as shown in the illustration above.

## Scripting Projects with Advanced Revenue Management {#bridgehead_4544339815}

The following table lists the scriptable fields associated with the Project record and advanced revenue management.

| **Field** | **Type** | **Internal ID** |
| --- | --- | --- |
| Accounting Period | List/Record | `accountingperiod` |
| Comments | Text Area | `comments` |
| Percentage Complete | Percent | `percent` |

Before you begin working with advanced revenue management programmatically, see [Setup for Advanced Revenue Management (Essentials)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4328435754.html).

For help working with this record in the user interface, see [Advanced Revenue Management (Essentials) for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4356983516.html).

### Related Topics

-   [Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3714107248.html)
-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Creating a Project Resource Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
