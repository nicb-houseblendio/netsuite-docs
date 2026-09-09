---
id: "section_N369952"
type: "section"
title: "Employees Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Employees Import Type > Employees Import"
parent: "section_3743324177"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N369952.html"
anchors: []
sha256: "b1b8f98ac2deac43f9e06ce45d684e5cf5a474d1881d5e00039b41af7153110c"
---

The Employees import adds employees to the Employee list.

-   Starting from version 2017.1, you can only import employee records if you're logged in with a role that has the Employees permission assigned to it.
    
-   When you import employee records, you can flag employees as sales representatives. This flagging is important if you plan to use CSV import to assign sales representatives to customer records.
    
-   If your account is using NetSuite OneWorld, and if the subsidiary is not set as a default value on the employee record, the Subsidiary field is required for Employees imports when you're creating new records. You must map the NetSuite Subsidiary field to a field in your CSV file, or the import will fail. The CSV file value for subsidiaries should be the name of the subsidiary.
    
-   The Employees import supports the import of the following sublist data:
    

| Sublist | Notes |
| --- | --- |
| Payroll Accrued Time | Selectively updatable based on Payroll Item key field. When Payroll feature enabled. |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Payroll Contributions | Selectively updatable based on Payroll Item key field. When Payroll feature enabled. |
| Payroll Deductions | Selectively updatable based on Payroll Item key field. When Payroll feature enabled. |
| Payroll Earnings | Selectively updatable based on Payroll Item key field. When Payroll feature enabled. |
| Direct Deposit | Selectively updatable based on Internal ID key field. When Direct Deposit feature enabled. |
| Education | \- |
| Emergency Contacts | \- |
| Roles | \- |
| Subscriptions | Selectively updatable based on Subscription key field. |
| HCM Position | Available when the HRIS module is enabled. By default, the fields on this list are read-only. The following fields are writable: Position, Primary Position, and Position Allocation. You must map a value for the workAssignment field to distinguish between a job and a position. By default, the workAssignment field is set to job. This sublist doesn't support the import of multiline sublist data. For more information, see [Importing Sublist Data in a Single File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493384282.html). |

For imports that update existing Employee records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

For details about fields that can be mapped in the Employee record, see the SOAP Schema Browser's [employee](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/employee.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

### Related Topics

-   [Employees Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3743324177.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
