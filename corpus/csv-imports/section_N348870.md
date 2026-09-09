---
id: "section_N348870"
type: "section"
title: "CSV Field Mapping Tasks"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Four Field Mapping > CSV Field Mapping Tasks"
parent: "section_N347418"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html"
anchors: []
sha256: "e870e3d6337952e0d80ca5bca551cd5bc477191ba7da24c0e5796adac5594205"
---

On the Field Mapping page of the Import Assistant, complete the following tasks:

-   To add a field to the mappings, highlight a line in the center pane and single-click a field in the right or left pane, or drag a field from the right or left pane to the center pane.
    
-   To provide a default value, null value, or reference type for a field, click its edit icon, and:
    
    -   Choose Provide Default Value, and select or enter a value. For more information, see [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).
        
    -   Choose the Set Value to Null option. This option is available only for fields that can have null values. You can set fields with no values in CSV files to null instead of enabling the Overwrite Missing Fields advanced option on updates. For more information, see [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html).
        
    -   Select a reference type. This option is available only for mapped fields that can have one or more list values, such as dropdown lists and multi-selects. For more information, see [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html).
        
    
    After you have made a selection, click Done to close the popup.
    
-   To delete a row in the center mappings pane, click the small X button.
    
-   If at any point you want to undo changes and return to auto or last saved mappings, click Reset.
    
-   You'll see available sublists at the bottom of the NetSuite Fields pane. Map sublist fields the same as other fields. At first, you get one instance per sublist, but you can add more by clicking Add New ( ![Add New sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/AddNew.png) ). Up to 99 instances are supported per sublist. Add New isn't available for sublists with linked files. For more information, see [Required Fields for Sublist Import Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html).
    
    ![Example of sublist field mapping.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/SublistFieldMap.png)
-   For some transaction imports, transaction item options may be included as a flat list under the Items sublist folder. Item options are custom fields that can be set up in your NetSuite account and may be included in transaction line items to represent item-specific choices. You can map item options to columns in your CSV file, and you can set default or null values for them. For more information, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).
    

### Related Topics

-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
-   [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html)
-   [Required Fields on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349431.html)
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
-   [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html)
-   [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
