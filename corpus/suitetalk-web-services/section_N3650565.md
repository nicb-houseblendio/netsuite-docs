---
id: "section_N3650565"
type: "section"
title: "Events (CalendarEvent)"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Activities > Events (CalendarEvent)"
parent: "chapter_N3650400"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650565.html"
anchors: ["bridgehead_N3650586", "bridgehead_N3650838", "bridgehead_N3650876", "bridgehead_N3650927", "bridgehead_N3650954", "bridgehead_N3650975", "procedure_N3650987", "bridgehead_N3651042", "procedure_N3651257", "procedure_N3651320", "bridgehead_N3651369", "bridgehead_N3651394", "bridgehead_4296986898", "procedure_N3651440", "bridgehead_4296989144", "bridgehead_N3651477", "bridgehead_N3651566", "bridgehead_N3651581", "bridgehead_N3651606", "bridgehead_N3651621"]
sha256: "f42031c33f299253ff92a4a95f6b50c3320faa87a705fa0a12847bb98df7d003"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Event](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161013672126.html).

Events are scheduled activities that are automatically added to your calendar when created. For more information, see [Working with Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N501214.html).

The event record is defined in the [actSched (scheduling)](https://webservices.netsuite.com/xsd/activities/v2025_2_0/scheduling.xsd) XSD.

## Supported Operations {#bridgehead_N3650586}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3650838}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, refer to the SOAP Schema Browser's [calendar event](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/calendarevent.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3650876}

Events can be scheduled as one-time events that are set to occur on a specific day at a specific time. Events can also be designated as recurring events, which recur over a period of several days, weeks, months, or years. See the following sections for more information:

-   [Non-Recurring (One-Time) Events](#bridgehead_N3650927)
    
-   [Recurring Events](#bridgehead_N3650954)
    

## Non-Recurring (One-Time) Events {#bridgehead_N3650927}

A non-recurring event takes place one time during a single day. Note that a non-recurring event cannot extend beyond midnight in a user's specified time zone. Both the _startDate_ and _endDate_ fields must contain the same date.

## Recurring Events {#bridgehead_N3650954}

Recurring events recur on a daily, weekly, monthly, or yearly basis. You can schedule events to automatically recur in your calendar in both basic and advanced patterns.

## Basic Recurrence Patterns {#bridgehead_N3650975}

A basic event recurrence pattern includes events such daily departmental status meetings. These events begin and end on the same day, and they recur in a Monday through Friday pattern. An event with a basic recurrence pattern does not require that you set the recurrenceDow, recurrenceDowim, or recurrenceDowMaskList fields.

#### To set a basic recurrence pattern: {#procedure_N3650987}

1.  Set the **frequency** field.
    
2.  Set the **period** field.
    
3.  Set the **startDate** field.
    
4.  Set the **endDate** field only if there is a known date by which you want to end the recurring event. Events that recur indefinitely do not require that you set the **endDate** field.
    

## Advanced Recurrence Patterns {#bridgehead_N3651042}

Events that are scheduled with advanced recurrence patterns may include some of the following types of patterns:

-   A certain number of days apart, such as every 3 days
    
-   The same day of the week with weeks off in between, such as Tuesday every 2 weeks
    
-   The same date of every month
    
-   The same date in a month with months off in between, such as every 3 months on the 20th
    
-   The same day of the week every month, such as the first Friday of every month
    
-   The same day of the week every few months, such as the first Tuesday every other month
    

To set an advanced recurrence pattern for an event, you must set the following fields, in addition to setting the _frequency, period_, and _startDate_ fields:

-   recurrenceDow
    
-   recurrenceDowim
    
-   recurrenceDowMaskList
    

The recurrenceDow, recurrenceDowim, and recurrenceDowMaskList fields do not have corresponding field labels in the UI. These fields represent a collection of functions which are shown in the figure below.

Note:

The recurrenceDow, recurrenceDowim, and recurrenceDowMaskList fields are hidden fields in SuiteScript. These fields are currently supported in server-side SuiteScript development; they are not supported in client development.

The following screenshot represents the scheduling of a monthly event that contains an advanced recurrence pattern.

![An example of setting the recurrence of an event.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/advEventRecurrence.png)

The preceding screenshot shows the equivalent of the following settings.

| Callout | Description |
| --- | --- |
| 1 | The _frequency_ field is set to **\_month**. |
| 2 | The _recurrenceDowim_ field is set to **\_first**. |
| 3 | The _recurrenceDow_ field set to **\_wednesday**. |
| 4 | The _period_ field is set to **1**. |

The next screenshot represents the scheduling of a weekly event that contains an advanced recurrence pattern.

![A weekly event with an advanced recurrence pattern.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/dowMaskList.png)

The preceding screenshot shows the equivalent of the following settings.

| Callout | Description |
| --- | --- |
| 1 | The _frequency_ field is set to **\_week**. |
| 2 | The _recurrenceDowMaskList_ field is set to **\_tuesday** and **\_thursday**. |

#### To set an advanced recurrence pattern that recurs monthly or yearly: {#procedure_N3651257}

1.  Set the **frequency** field to indicate how often the event will recur. The value specified for **frequency** dictates the values that will be set for the **recurrenceDow** and **recurrenceDowim** fields.
    
2.  Next, set the **period** field.
    
3.  Set the value for **recurrenceDow**.
    
4.  Set the value for **recurrenceDowim**.
    

#### To set an advanced recurrence patterns that recurs weekly: {#procedure_N3651320}

1.  Set the **frequency** field to indicate how often the event will occur. The value specified for **frequency** dictates the value that will be set for the **recurrenceDow** MaskList.
    
2.  Next, set the **period** field.
    
3.  Finally, set **recurrenceDowMaskList**.
    

## Updating a Series of Events that Include Advanced Recurrence Patterns {#bridgehead_N3651369}

When updating a record in SOAP web services, generally you submit only the values you intend to change. However, when updating an event record that includes advanced recurrence patterns, you must use nullFieldList to explicitly remove the values that were previously set.

For example, to update a **monthly** or a **yearly** event from a specific day of the week in a month to a specific day of the month, use nullFieldList to explicitly remove the values in recurrenceDowim and recurrenceDow.

## Updating a Single Instance of a Recurring Event {#bridgehead_N3651394}

A recurring event can be modified to change or delete an individual event in the series. In SOAP web services, this is handled using the **ExclusionDateList** type.

## Deleting individual events in a series {#bridgehead_4296986898}

To delete individual events in a series, update the recurring event with a list of exclusions (in the form of dates) in the ExclusionDateList type. The ExclusionDateList type sets a list of timestamps of individual events that have been excluded from the series.

Important:

After an event has been excluded, it is separated from the rest of the events in the series, and it can NOT be associated with the event series.

#### To update an individual instance of a recurring event {#procedure_N3651440}

1.  Update the recurring event with a list of exclusions (in the form of dates) in the **exclusionDateList** field.
    
2.  For each exclusion, add a new event that contains the updated data.
    
    The original event and the new modified event have different internal ID values and the new updated event is no longer associated with the event series.
    

## Retrieving excluded events from a series {#bridgehead_4296989144}

To retrieve excluded events from a series, submit a get operation for the desired event series and return the values listed in the ExclusionDateList type.

## Working with Event Lists {#bridgehead_N3651477}

The SOAP Schema Browser includes all lists (sublists) associated with the Event record. See the following information for usage notes regarding specific Event lists. Note that usage notes are not provided for every list type.

-   [AttendeeList](#bridgehead_N3651566)
    
-   [ExclusionDateList](#bridgehead_N3651581)
    
-   [ResourceList](#bridgehead_N3651606)
    
-   [TimeItemList](#bridgehead_N3651621)
    

## AttendeeList {#bridgehead_N3651566}

This list is used to identify each attendee for the event.

## ExclusionDateList {#bridgehead_N3651581}

This list is used to denote individual events in a series that have been modified or deleted. For detailed information, see [Updating a Single Instance of a Recurring Event](#bridgehead_N3651394).

## ResourceList {#bridgehead_N3651606}

This list is used to schedule available resources for the event.

## TimeItemList {#bridgehead_N3651621}

This list, available when the Time Tracking feature is enabled, is used to track employee time associated with the event, including payroll, billing, and project fields.

### Related Topics

-   [Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3650400.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
