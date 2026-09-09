---
id: "section_N360296"
type: "section"
title: "Tasks Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Activities Import Type > Tasks Import"
parent: "section_N359586"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N360296.html"
anchors: ["bridgehead_N360596", "bridgehead_3705040959", "bridgehead_3705041487"]
sha256: "f05c8d61fae08c34ec977da9d33be00c1d2875e2990228c7deae7d8decefc52c"
---

A task record stores details about a unit of work to be completed. NetSuite supports the creation of two different types of tasks: CRM Tasks and Project Tasks. The Tasks import supports the import of CRM tasks, not project tasks. CRM tasks, usually labeled Tasks in the NetSuite user interface, don't have to be associated with projects.

Note:

Project tasks are available in accounts where the Project Management feature is enabled, and are used only in association with project records. For more information about importing project tasks, see [Project Tasks Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0804012344.html).

The CRM tasks data that you can import depend on the fields available on either your preferred Task form, or the custom task form selected on the Import Assistant Import Options page. For details about specifying a custom form, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).

For details about fields that can be mapped in the Task record, see the SOAP Schema Browser's [task](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/task.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Be aware of the following:

-   Required task fields for import are: Assigned To, Due Date, Priority, Start Date, Status, and Title.
    
-   You need to understand the use of the Start Date and End Date fields on task records, and to exercise care when you format values for the Start Date, End Date, and Due Date fields in your CSV files. To avoid errors, review and follow the guidelines in [Setting Date Field Values for Tasks Imports](#bridgehead_N360596).
    
-   Unlike in the user interface, the Assigned To field doesn't default to be the logged in user. You need to include values for this field in your CSV file or set up a default on the Import Assistant Field Mapping page. See [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).
    
-   The Send Email field isn't available for import mapping. Imports can't send email to task assignees.
    
-   The Tasks import supports the import of the following sublist data:
    

| Sublist | Notes |
| --- | --- |
| Contacts | Selectively updatable based on Company/Project(Entity) or Contact key field. Maps to Companies and Contacts subtab on Related Records subtab of Task record, can include other records, such as customers and contacts, that are related to each task. |
| Time Tracking | When Time Tracking feature is enabled. |

For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

-   If you're doing a tasks import for the addition of new tasks, select the **Add** data handling option, rather than **Add or Update**.
    
-   If you need to use an import to update existing task records, you must map either the Internal ID or External ID field to uniquely identify records. This requirement is enforced when you select the **Update** data handling option and when you select the **Add or Update** data handling option. The Title field isn't a key field and doesn't have to be unique.
    

## Setting Date Field Values for Tasks Imports {#bridgehead_N360596}

Before you set up a CSV file for a tasks import, you need to understand how Start Date and End Date fields are used, and you need to be aware of formatting requirements for Start Date, End Date, and Due Date field values.

## Understanding Start Date and End Date Fields {#bridgehead_3705040959}

You can review the standard Task form to understand the use of the Start Date and End Date fields in task records, to properly specify their values in your CSV files.

-   Reserve Time - Indicates whether to schedule time for the task on the assignee's calendar. How the Start Date and End Date fields are used depends upon whether Reserve Time is enabled (set to True). By default, Reserve Time isn't enabled (set to False).
    
-   Start Date - The date when a task is started, as shown in the field labeled **Start Date** on the standard Task form, number 1 in the following screenshot. If Reserve Time is enabled, the Start Date value should also include a time that is the beginning of reserved time on the assignee's calendar, as shown in the field labeled **Start Time**, number 2 in the following screenshot.
    
-   End Date - If Reserve Time is enabled, the time that is the end of reserved time on the assignee's calendar, as shown in the field labeled **End Time** on the standard Task form, number 3 in the following screenshot. The date is not shown, and is assumed to be the same as the date in the Start Date field.
    

![Date and time fields highlighted on the Task page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TaskDateFields_2014_2.png)

## Formatting Guidelines for Task Date Field Values {#bridgehead_3705041487}

Follow these guidelines when you enter values for date fields in CSV files used for tasks imports.

-   For Start Date fields:
    
    -   If Reserve Time is set to False, a Start Date value requires only a date, for example: **04/12/2010**. If a time is included, it is ignored.
        
    -   If Reserve Time is set to True, Start Date requires both a date and a time, for example: **04/12/2010 09:00 AM**.
        
-   For End Date fields:
    
    -   If Reserve Time is set to False, no End Date value is required.
        
    -   If Reserve Time is set to True, End Date requires both a date, that should be the same as the date set for Start Date, and a time, for example: **04/12/2010 11:00 AM**.
        
-   For Start Date, End Date, and Due Date fields, values should be specified according to the NetSuite Date Format, and if applicable, Time Format, set at _Home > Set Preferences_ for the user doing the import. The following are example formats:
    
    -   Date Format is **DD/MM/YYYY**.
        
    -   Time Format is **hh:mm AM/PM**.
        
    -   For a Start Date or End Date field that includes both date and time, a space should be included between them, for example: **04/12/2010 10:00 AM**.
        

Important:

If your tasks import returns date-related errors such as 'You have entered an Invalid Field Value' or 'Due Date occurs before Start Date', try removing leading zeros from date values in your CSV file, for example changing **08/01/2010** to **8/1/2010**.

-   To avoid Excel formatting errors for Start Date, End Date, and Due Date values, you should right-click the column and choose Format Cells to explicitly select a format that matches the Date Format (and if applicable, Time Format) set up in NetSuite.
    
    ![Format Cells window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TaskDateFormats.png)

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html)

### Related Topics

-   [Activities Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N359586.html)
-   [Events Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3743314536.html)
-   [Phone Calls Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N359696.html)
-   [Resource Allocations Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1536261544.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
