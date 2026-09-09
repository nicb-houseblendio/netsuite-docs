---
id: "section_N3643925"
type: "section"
title: "Employee"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Employee"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3643925.html"
anchors: ["bridgehead_N3643946", "bridgehead_N3644217", "bridgehead_N3644254", "bridgehead_N3644262", "bridgehead_1495193087", "bridgehead_N3644309"]
sha256: "50e8a0e280c12c0517ff8399bde6cc94841ae6effd8d57e13f7bfe49520bffe4"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161886175135.html).

Employee records represent your employees. Use the employee record to store information for contact, login, payroll and human resources purposes. For more information, see [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html).

The employee record is defined in the [employees XSD](https://webservices.netsuite.com/xsd/lists/v2025_2_0/employees.xsd).

## Supported Operations {#bridgehead_N3643946}

The following operations can be used to modify employee records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3644217}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [employee](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/employee.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3644254}

## Entering Expense Reports in SOAP web services {#bridgehead_N3644262}

SOAP web services support for expense reports is different from user interface behavior. In the user interface, expense reports can only be entered for active employees. If an employee's release date is before the current date, expense reports are not supported. In SOAP web services, expense reports can be entered for employees that have a release date before the current date.

## Specifying Employee Jobs and Positions {#bridgehead_1495193087}

When you work with employee jobs and positions, you must submit a value for the workAssignment field to distinguish between a job and a position. By default, the workAssignment field is set to job. If you submit values for the hcmPosition sublist, you must override the value of the workAssignment field, otherwise the sublist values will not be used.

## EmployeeAddressbookList {#bridgehead_N3644309}

When you work with the addressbookList in the 2009.2 endpoint and beyond, be sure to use **internalId** as the key. Do not use **label**. For the 2009.1 and lower endpoints, the addressbookList is not a keyed sublist, but you can use label to identify records.

### Related Topics

-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
