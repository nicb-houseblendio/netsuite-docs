---
id: "section_N362626"
type: "section"
title: "Class Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Classification Import Type > Class Import"
parent: "section_N360930"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362626.html"
anchors: []
sha256: "a83a79caec7cbd722e60a08421f4c01efe7af15b8ad5295f6a6016d0c0fd8038"
---

Classes are type definitions that can be used to categorize records such as financials, transactions, and employees. Classes can provide more generalized categories than departments or locations. For more information, see [Creating Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261769.html).

You can use the Import Assistant to set up and update class records in your NetSuite account.

Before you can import classes, an administrator, or another user with permission to enable features, must go to _Setup > Company > Enable Features_, and on the Company subtab, check the Classes box, and click Save.

Class fields for which data can be imported include Name, External ID, Subclass of (the parent class, if any), and whether the class is inactive. If you're using NetSuite OneWorld, these additional fields also are available: Subsidiaries (the subsidiaries associated with a class), and Include Children (a indicating whether to associate a class with all child subsidiaries of those specified in the Subsidiaries field).

For details about fields that can be mapped in the Class record, see the SOAP Schema Browser's [class](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/classification.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

After you have imported class records successfully, you can review them at _Setup > Company > Classes_.

Note:

If you plan to import other record types that include fields referencing class values, complete the import of classes first.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Classification Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N360930.html)
-   [Custom Segment Value Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358372117.html)
-   [Department Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362786.html)
-   [Location Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362936.html)
-   [Merchandise Hierarchy Node Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530005074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
