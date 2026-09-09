---
id: "section_N350094"
type: "section"
title: "Assign Null Values during Field Mapping"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Four Field Mapping > Assign Null Values during Field Mapping"
parent: "section_N347418"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html"
anchors: []
sha256: "6c6c272b995eb5021bd18324e8a0d19062df4306d63f24b4f5176fdcbf956624"
---

It is possible to assign null values to fields on the Import Assistant's Field Mapping page. This assignment causes the value for any existing fields to be set to an empty value.

-   Null values are useful when a field has been assigned a default value that you do not want to propagate across all of the records that you are importing.
    
    For example, if you're a sales rep and add a lead in the UI, the Sales Rep field defaults to you. The Import Assistant does the same thing. So, if you import 10,000 leads, they'll all have you as the Sales Rep by default. That's probably not what you want for a big import.
    
-   Null values also are useful for fields with no values in CSV files. For imports that update NetSuite data, you can set fields with no values in CSV files to null instead of enabling the Overwrite Missing Fields advanced option. For more information, see [Overwrite Missing Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751050565.html).
    

To set a field to null, click the edit icon in its row on the Field Mapping page and pick Set Value to Null. This only works for fields that allow null values.

### Related Topics

-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
-   [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html)
-   [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html)
-   [Required Fields on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349431.html)
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
-   [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
