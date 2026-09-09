---
id: "section_N3184256"
type: "section"
title: "Project Task"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Activities > Project Task"
parent: "chapter_N3184006"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184256.html"
anchors: ["bridgehead_3794203351", "bridgehead_3794203419", "bridgehead_3794203456", "bridgehead_3794203514", "bridgehead_3802781776"]
sha256: "4ac55022892de3286ec91852af7f6ed78267435e8075927cd25632a1f155480d"
---

The project task record can be used to keep track of specific activities and milestones associated with a project.

The internal ID for this record is `projecttask`.

The project task record is available when the Project Management feature is enabled at _Setup > Company > Enable Features_, on the Company subtab. When the feature is enabled, you can access the project task record in the UI by going to an existing project and clicking the New Project Task or New Milestone button.

For help working with this record in the user interface, see [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html).

Project task records cannot be created as standalone records. Rather, you create a project task for a specific project record, and the task remains attached to that record. For information about working with the project record in SuiteScript, see [Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185758.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/projecttask.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Project Tasks Versus Milestone Tasks {#bridgehead_3794203351}

Every project task record is designated as either a project task or a milestone task. A project task is used to represent an activity, whereas a milestone task is used to represent a checkpoint in the overall progress of the project.

Although they are the same type of record, a milestone task cannot have values in the estimatedwork body or sublist fields. Therefore, if you create a project task record and do not include any estimated work, the record is automatically saved as a milestone task. If you do include estimated work, the record is saved as a project task.

These same rules apply to the updating of records as well. In other words:

-   To convert a project task into a milestone task, clear the estimatedwork body field and all values from the Assignees sublist.
    
-   To convert a milestone task into a project task, add a value to the estimatedwork body field or add at least one record to the Assignees sublist, with a positive value of estimated work.
    

Note that the estimatedwork body field is populated by the sum of estimated work listed for Assignees. If you explicitly set a value for the estimatedwork body field, and you also include Assignees, the value you specify for the body field is overwritten based on the sublist's estimatedwork values. If you do not include Assignees, you can explicitly assign a value to the estimatedwork body field.

## Supported Script Types {#bridgehead_3794203419}

The project record is scriptable in server SuiteScript only.

All three user events are supported: `beforeLoad`, `beforeSubmit`, and `afterSubmit`.

## Supported Functions {#bridgehead_3794203456}

The project record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript.

## Field Definitions {#bridgehead_3794203514}

When creating new project tasks you must set the Project (_company_) field to the project/job ID. Project tasks are not standalone records, and therefore must be associated with a specific project.

For other details on body fields and sublist fields, See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/projecttask.html), which lists all internal IDs associated with this record. For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

## Code Sample {#bridgehead_3802781776}

The following example shows how you might create both a project task and a milestone task.

          `// create a project var project = record.create({     type: record.Type.JOB,     isDynamic: true }); project.setValue({     fieldId: 'companyname',     value: 'Reconstruction' }); project.setValue({     fieldId: 'subsidiary',     value: 1 }); var projectId = project.save();  // create a project task var task = record.create({     type: record.Type.PROJECT_TASK }); task.setValue({     fieldId: 'estimatedwork',     value: 2 }); task.setValue({     sublistId: 'title',     value: 'Remove old furniture' }); task.setValue({     sublistId: 'company',     value: projectId }); var task1Id = task.save();  // create another task depending on the first one with Finish-To-Start dependency task = record.create({     type: record.Type.PROJECT_TASK }); task.setValue({     fieldId: 'estimatedwork',     value: 5 }); task.setValue({     fieldId: 'title',     value: 'Paint walls' }); task.setValue({     fieldId: 'company',     value: projectId }); task.selectNewLine({     sublistId: 'predecessor' }); task.setCurrentSublistValue({     sublistId: 'predecessor',     fieldId: 'task',     value: task1Id }); task.setCurrentSublistValue({     sublistId: 'predecessor',     fieldId: 'type',     value: 'FS' }); task.commitLine({     sublistId: 'predecessor' }); var task2Id = task.save();  // create a milestone task = record.create({     type: record.Type.PROJECT_TASK,     isDynamic: true }); task.setValue({     fieldId: 'estimatedwork',     value: 0 }); task.setValue({     fieldId: 'title',     value: 'Verify painting after the walls dry out' }); task.setValue({     sublistId: 'company',     value: projectId }); task.selectNewLine({     sublistId: 'predecessor' }); task.setCurrentSublistValue({     sublistId: 'predecessor',     fieldId: 'task',     value: task2Id }); task.setCurrentSublistValue({     sublistId: 'predecessor',     fieldId: 'type',     value: 'FS' }); task.commitLine({     sublistId: 'predecessor' }); var milestoneId = task.save();` 
        

### Related Topics

-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Enabling Project Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4740572949.html)
-   [Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3650400.html)
-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185758.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
