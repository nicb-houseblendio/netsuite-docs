---
id: "section_N349148"
type: "section"
title: "General CSV Field Mapping Tips"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Four Field Mapping > General CSV Field Mapping Tips"
parent: "section_N347418"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html"
anchors: []
sha256: "db36dc9ffd26b1bbe7b03fd43e739d7b0f3e21da5256f832c372bd7f468b023d"
---

-   If you're using NetSuite OneWorld, you have to map the Subsidiary field for these record types: Chart of Accounts, Contacts, Customers, Employees, Jobs (Projects), Leads, Partners, Prospects, and Vendors. If you try to import or update records without a subsidiary, the import will fail.
    
-   The NetSuite fields you see in the right pane depend on what's available on your preferred form for that record type. If your form doesn't allow access to certain fields, you won't see them for mapping.
    
    If you use a custom form for data entry in the user interface, you can select that form as an advanced option on the Import Options page to make sure the right fields are available for mapping. By default, the standard form is used. For more info, see .
    
-   You can map one CSV field to multiple fields in the same NetSuite record or sublist.
    
-   If you don't map any fields for a sublist, no sublist data gets imported, even if you set a default value for some sublist fields. For more info about sublist data and the Import Assistant, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).
    
-   If you want to create your own CSV import templates that map to NetSuite fields automatically, check the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html) for field details by record type. For information about working with this tool, see the help topic [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).
    
-   To ensure a successful import, verify that the values in each field of your CSV file match the format required by the corresponding NetSuite fields in the UI, which may vary depending on the record type being imported.
    

### Related Topics

-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
-   [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html)
-   [Required Fields on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349431.html)
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
-   [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html)
-   [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
