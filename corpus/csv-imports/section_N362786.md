---
id: "section_N362786"
type: "section"
title: "Department Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Classification Import Type > Department Import"
parent: "section_N360930"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362786.html"
anchors: []
sha256: "04f31987ce87414eaa551d762f66b1d122bd0906bb9af0977bbb568470e4d448"
---

Departments can be used to categorize records, such as accounts, employees, and items. Departments usually indicate groupings of records according to management responsibility. For more information, see [Creating Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262248.html).

You can use the Import Assistant to set up and update department records in your NetSuite account. To import department records, select Classification as the import type, and Department as the record type.

Before you can import departments, an administrator, or another user with permission to enable features, must go to _Setup > Company > Enable Features_, and on the Company subtab, check the Departments box and click Save.

Department fields for which data can be imported include Name, External ID, Subdepartment of (the parent department, if any), and whether the department is inactive. If you're using NetSuite OneWorld, these additional fields also are available: Subsidiaries (the subsidiaries associated with a department), and Include Children (a indicating whether to associate a department with all child subsidiaries of those specified in the Subsidiaries field).

For details about fields that can be mapped in the Department record, see the SOAP Schema Browser's [department](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/department.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

After you have imported department records successfully, you can review them at _Setup > Company > Departments_.

Note:

If you plan to import other record types that include fields referencing department values, complete the import of departments first.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html), [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Classification Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N360930.html)
-   [Class Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362626.html)
-   [Custom Segment Value Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358372117.html)
-   [Location Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362936.html)
-   [Merchandise Hierarchy Node Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530005074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
