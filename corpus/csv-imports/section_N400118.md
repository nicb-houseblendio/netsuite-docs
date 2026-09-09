---
id: "section_N400118"
type: "section"
title: "Prerequisite Records for Routing Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Routing Import > Prerequisite Records for Routing Import"
parent: "section_N399906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400118.html"
anchors: ["bridgehead_N400200", "bridgehead_N400561", "bridgehead_N400593", "bridgehead_N400618"]
sha256: "6ed2d01399e593b1d94434e9eefe2a138d67a15bbd8b637e92c206bc2e07cd95"
---

When you create a routing record, you rely on certain prerequisite records that must already exist in NetSuite. Specifically, you need at least one record of each of the following types:

-   [Assembly Item](#bridgehead_N400200)
    
-   [Manufacturing Work Center](#bridgehead_N400561)
    
-   [Default Calendar](#bridgehead_N400593)
    
-   [Manufacturing Cost Template](#bridgehead_N400618)
    

You can't import routings until you have created these records.

## Assembly Item {#bridgehead_N400200}

An assembly item is an item built from member components - other items that exist in your system. It is not possible to create a routing record without naming a specific assembly item to which the routing can be applied. If necessary, you can import routing records that name one particular assembly item and update the routing records later to name different assembly items.

You can import assembly item records or create them manually using the New Assembly/Bill of Materials form, available at _Lists > Accounting > Items > New_ > Assembly/Bill of Materials. For details on manually creating assembly records, see [Assembly Item](#bridgehead_N400200). For details on the import process, see [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html).

## Manufacturing Work Center {#bridgehead_N400561}

A manufacturing work center is a static group of employees that has been flagged as a manufacturing work center on the group record. For each operation you create on any routing record, you also must identify a value for manufacturing work center. This value identifies the group responsible for completing the operation.

You can create a work center by using the Create Group form, which is available at _List > Relationships > Groups_ > New. The group you create should be a static group made up of employees. Further, on the group record, you must select the box labeled Manufacturing Work Center. If you don't do this, the group is not recognized as a valid entry on a routing record.

For more details, see [Creating Manufacturing Work Centers or Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344727.html).

## Default Calendar {#bridgehead_N400593}

NetSuite uses the default work calendar to schedule the operations associated with work centers. The calendar can affect the time required to complete an assembly. If appropriate, you can create a different default calendar, at _Lists > Employees > Work Calendars > New_. To ensure that your routings use this calendar, select the Default Calendar box on the calendar record. For more details, see [Setting Up a Work Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190013.html).

NetSuite uses the default work calendar to schedule the operations associated with work centers. The calendar can affect the time required to complete an assembly. If appropriate, you can create a different default calendar, at Lists > Employees > Work calendars. Click New. To ensure that your routings use this calendar, select the Default Calendar box on the calendar record. For more details, see [Setting Up a Work Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190013.html).

## Manufacturing Cost Template {#bridgehead_N400618}

A manufacturing cost template defines the rates used to calculate the cost of an operation. For each operation you create on any routing record, you also must identify an existing cost template record.

For details on manually creating cost templates, see [Creating Manufacturing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344013.html). For details on importing cost templates, see [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html).

### Related Topics

-   [Manufacturing Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399906.html)
-   [Routing Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400811.html)
-   [Routing CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N401643.html)
-   [Common Errors When Importing Routing Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404433.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
