---
id: "section_N3654609"
type: "section"
title: "Tasks"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Activities > Tasks"
parent: "chapter_N3650400"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3654609.html"
anchors: ["bridgehead_N3654629", "bridgehead_N3654885", "bridgehead_N3654922", "bridgehead_N3654934", "bridgehead_N3654946", "bridgehead_N3654958", "bridgehead_N3654978", "bridgehead_N3654994", "bridgehead_N3655010", "bridgehead_N28264961"]
sha256: "19b5fedb8c7dc65f8d5dec271aac0f5d3e11c1dea5dda46e108ce90a3563f41e"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161039060436.html).

Tasks are activities that need to be completed. Use the task record to add new tasks for individuals, companies or contacts and to modify those records. For information about working with tasks in the UI, see [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html).

The task record is defined in the [actSched (scheduling)](https://webservices.netsuite.com/xsd/activities/v2025_2_0/scheduling.xsd) XSD.

## Supported Operations {#bridgehead_N3654629}

The following operations can be used with task records.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3654885}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [task](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/task.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3654922}

In SOAP web services tasks are ordered by creation date. In the UI, tasks can be ordered by specifying an Insert Before parameter that places the current task before an existing task assigned to the same user. This functionality is NOT available through SOAP web services.

## Identifying Unique TaskContact List Records {#bridgehead_N3654934}

Entries in the TaskContact list are identified by unique combinations of the customer/contact pairing. Therefore, if you have multiple entries in the TaskContact list with the same customer, the contact is also needed to further identify the record. In the event that two or more entries have the same customer/contact pairing, these entries are treated as a single unit.

## Time Tracking Sublist {#bridgehead_N3654946}

When the Time Tracking feature is enabled, the TimeItemList sublist is available. This list is used to track employee time associated with the task, including payroll, billing, and project fields.

## Restricting Time Entry on Tasks {#bridgehead_N3654958}

Unless the SOAP web services user is an administrator or the employee specified on the task, the user will not be able to set the reminderType and reminderMinutes fields on a task record. If the user attempts to set these fields, the values specified will not be saved.

In the UI, you can set the **Check the Limit Time to Assignees** box to restrict time entry against this job. When you check this box, only assigned resources can enter time for this job's tasks.

## Setting Start and End Times for Timed Tasks {#bridgehead_N3654978}

In SOAP web services the startTime and endTime field are not exposed. Therefore, to set start and end times for a timed task, users must first set the timedEvent field to TRUE. Then the time component of the DateTime value that is specified in startDate will be set for startTime, and the time component of the DateTime value that is specified in endDate will be set for endTime.

Note that the fields reminderMinutes and reminderType are also only settable if timedEvent is set to TRUE.

## Contacts Sublist {#bridgehead_N3654994}

TaskContactList, which lists contacts and companies related to each task, does not have a unique key field, so it can include duplicated values.

If you set the ReplaceAll preference to True for a write to the sublist, and a value that you submit matches two nonunique existing values, an error is thrown, because it is not clear which existing value to match. If a value you submit matches a unique row, the row is preserved and no error is thrown.

## Code Sample {#bridgehead_N3655010}

The following sample shows how to add a task to a job record.

## Java {#bridgehead_N28264961}

          `public void addTaskToJob() throws RemoteException {                 this.login(true);                   RecordRef custRef = new RecordRef();                 custRef.setInternalId("95");                 custRef.setType(RecordType.job);                   Task task = new Task();                 task.setCompany(custRef);                 task.setTitle("Race Car Tuning");                 task.setMessage("Includes baseline dyno, 5 hours tuning session & turbo upgrade.");                   WriteResponse response = _port.add(task);                                  if (response.getStatus().isIsSuccess()) {                         _console.info("\nThe following task was added successfully: " + ((RecordRef) response.getBaseRef()).getInternalId());                 } else {                         _console.error("The task was not added:", true);                         _console.error(getStatusDetails(response.getStatus()));                 }         }` 
        

### Related Topics

-   [Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3650400.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
