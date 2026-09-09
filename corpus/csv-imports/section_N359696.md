---
id: "section_N359696"
type: "section"
title: "Phone Calls Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Activities Import Type > Phone Calls Import"
parent: "section_N359586"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N359696.html"
anchors: ["bridgehead_N359983", "bridgehead_3705039378", "bridgehead_3705040002"]
sha256: "b32211b0937f93011f5a35a5900442617c14645a4d951be0a07fc303a5617b99"
---

A phone call record stores details about a business call, such as its organizer, its subject, and its date and time. A phone call can be linked to another record type such as customer or contact. After a phone call is linked to another record type, the phone call appears on the Activities subtab of that record.

The phone call data that you can import depends on the fields available on either your preferred Phone Call form, or the custom phone call form selected on the Import Assistant Import Options page. For details about specifying a custom form, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).

For details about fields that can be mapped in the Phone Call record, see the SOAP Schema Browser's [phone call](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/phonecall.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Be aware of the following:

-   Required phone call fields for import are: Organizer, Status, Subject, and Date.
    
-   You need to understand the use of the Date and End Date fields on phone call records, and to exercise care when you format values for them in your CSV files. To avoid errors, review and follow the guidelines in [Setting Date Field Values for Phone Calls Imports](#bridgehead_N359983).
    
-   Unlike in the user interface, the Organizer field doesn't default to be the logged in user. You need to include values for this field in your CSV file or set up a default on the Import Assistant Field Mapping page. See [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).
    
-   The Phone Calls import supports the import of the following sublist data:
    

| Sublist | Notes |
| --- | --- |
| Contacts | Selectively updatable based on Participant(Entity) or Contact key field. Maps to Companies and Contacts subtab on Related Records subtab of Phone Call record, can include other records, such as customers and contacts, that are related to each phone call. |
| Time Tracking | When Time Tracking feature is enabled. |

For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

-   If you're doing a phone calls import for the addition of new phone calls, select the **Add** data handling option, rather than **Add or Update**.
    
-   If you need to use an import to update existing phone call records, you must map either the Internal ID or External ID field to uniquely identify records. This requirement is enforced when you select the **Update** data handling option and when you select the **Add or Update** data handling option.
    

## Setting Date Field Values for Phone Calls Imports {#bridgehead_N359983}

Before you set up a CSV file for a phone calls import, you need to understand how Date and End Date fields are used, and you need to be aware of formatting requirements for their values.

## Understanding Date and End Date Fields {#bridgehead_3705039378}

You can review the standard Phone Call form to understand the use of the Date and End Date fields in phone call records, to properly specify their values in your CSV files.

-   Reserve Time - Indicates whether to schedule a time for the phone call on the organizer's calendar. How the Start Date and End Date fields are used depends upon whether Reserve Time is enabled (set to True). By default, Reserve Time isn't enabled (set to False).
    
-   Date - The date when a phone call is started, in the field labeled **Date** on the standard Phone Call form, number 1 in the following screenshot. If Reserve Time is enabled, the Date value should also include a time that is the beginning of reserved time on the organizer's calendar, as shown in the field labeled **Start Time**, number 2 in the following screenshot.
    
-   End Date - If Reserve Time is enabled, the time that is the end of reserved time on the organizer's calendar, as shown in the field labeled **End Time** on the standard Phone Call form, number 3 in the following screenshot. The date isn't shown, and is assumed to be the same as the date in the Date field.
    

![Date and time fields on the Phone Call page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/PhoneCallDateFields_2014_2.png)

## Formatting Guidelines for Phone Call Date Field Values {#bridgehead_3705040002}

Follow these guidelines when you enter values for date fields in CSV files used for phone calls imports.

-   For Date fields:
    
    -   If Reserve Time is set to False, a Date value requires only a date, for example: **04/12/2010**. If a time is included, it's ignored.
        
    -   If Reserve Time is set to True, Date requires both a date and a time, for example: **04/12/2010 09:00 AM**.
        
-   For End Date fields:
    
    -   If Reserve Time is set to False, no End Date value is required.
        
    -   If Reserve Time is set to True, End Date requires both a date, that should be the same as the date set for Date, and a time, for example: **04/12/2010 11:00 AM**.
        
-   For both Date and End Date fields, values should be specified according to the NetSuite Date Format, and if applicable, Time Format, set at _Home > Set Preferences_ for the user doing the import. The following are example formats:
    
    -   Date Format is **MM/DD/YYYY**.
        
    -   Time Format is **hh:mm AM/PM**.
        
    -   For a Date field that includes both date and time, a space should be included between them, for example: **04/12/2010 10:00 AM**.
        
-   To avoid Excel formatting errors for Date and End Date values, right-click the column and choose Format Cells to explicitly select a format that matches the Date Format (and if applicable, Time Format) set up in NetSuite.
    
    ![Format Cells window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TaskDateFormats.png)

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Working with Phone Calls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509876.html)

### Related Topics

-   [Activities Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N359586.html)
-   [Events Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3743314536.html)
-   [Resource Allocations Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1536261544.html)
-   [Tasks Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N360296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
