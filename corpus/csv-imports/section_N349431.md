---
id: "section_N349431"
type: "section"
title: "Required Fields on Records"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Four Field Mapping > Required Fields on Records"
parent: "section_N347418"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349431.html"
anchors: ["procedure_N349455", "procedure_N349478"]
sha256: "d7c271fc19de723b29867c29b10c8d82e1811cd8473bcf4f753ec89fc38973cf"
---

Some NetSuite fields are required, so you have to give them a value or the import won't work. You can map these fields to your CSV columns or set default values for them on the Field Mapping page.

Required NetSuite fields show up in the NetSuite Fields column with (Req) after their name. Usually, they're listed automatically in the mapping pane to remind you to map them. But if a required field is hidden in a tree node on the right, you'll need to click it and map it yourself. Required fields for sublists work a bit differently; for information see [Required Fields for Sublist Import Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html).

#### Mapping a Required Field {#procedure_N349455}

1.  On the Field Mapping page, click the required NetSuite field on the right if it is not already in the mapping column.
    
2.  Click the matching field from your CSV on the left to map it to the NetSuite required field.
    

#### Providing a Default Value for a Required Field {#procedure_N349478}

1.  Click the edit icon next to your field.
    
2.  Enter a default value for this field.
    
    For more information, see [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).
    

Even if you set a default value for fields in a sublist, no sublist data gets imported unless you map at least one field for that sublist. For more information about working with sublists, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Note:

If Marketing Automation is enabled and you choose the 'Add' data handling option on the Import Assistant's Import Options page, you will be required to map the Unsubscribe field on the Field Mapping page, even if this field is not displayed on your preferred form for the record type. If the Unsubscribe field has not been mapped to a value, an error is thrown and you must go back and rectify the error.

### Related Topics

-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
-   [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html)
-   [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html)
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
-   [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html)
-   [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
