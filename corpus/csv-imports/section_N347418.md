---
id: "section_N347418"
type: "section"
title: "Step Four Field Mapping"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Four Field Mapping"
parent: "chapter_N343158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html"
anchors: []
sha256: "dc35f3e2e6e11d909873cefd450a55c813541cb00a4bd2cc103e27cd81a45522"
---

Step four of the Import Assistant shows how your CSV fields are automatically mapped to NetSuite fields. For details on what to do in this step, see [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html).

-   You see your CSV fields in the left pane.
    
-   The center pane shows your field mappings. Blank spaces mean you still need to map those fields.
    
    Required fields are marked with **(** Req **)**. You must map these fields or set default values for them.
    
-   NetSuite fields are listed in the right pane.
    
    -   Fields that have already been mapped appear dimmed.
        
    -   Fields you can still map are in darker text.
        
    -   Custom fields are marked with a special icon. (![Custom fields icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/custmarker.png))
        
    -   Key fields are marked with a special icon. (![Key fields icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/01CSVImportProcedures.png))
        

Note:

You can only map NetSuite fields that are editable on your preferred form for that record type.

![Import Assistant Step 4 Field Mapping.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/Step4ImpAsst.png)

To get a better understanding of the NetSuite fields, you can do the following:

-   Carefully review the NetSuite user interface form for the selected record type. You can click the field label for help that describes the field.
    
-   See the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html) for more descriptions of each field. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).
    

By default, you can map any NetSuite fields that are on your preferred form and not hidden or disabled. If you need more fields, pick a custom form with the fields you want in Advanced Options. This will update the list of NetSuite fields you can map. See [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).

To manually map fields:

1.  Click the first empty row in the center pane. The arrows on each side show which row you're editing.
    
2.  Click the CSV file field you want to map in the left pane.
    
3.  Click the NetSuite field in the right pane to map it with the CSV file field.
    

![Import Assistant Mapping page with numbering on each pane, showing the steps for manual mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/NSN_Import_Mapping.png)

For help with step four, review these guidelines.

-   [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html)
    
-   [Required Fields on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349431.html)
    
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
    
-   [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html)
    
-   [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html)
    

Note:

If you make mistakes during mapping, click the Reset button to go back to the automatic or the last saved mappings.

When you have completed field mapping, click Next to go to [Step Five Save Mapping & Start Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350233.html).

-   If you haven't mapped all fields, you'll see an error popup and the problem fields will get a red X. Add the missing mappings and click Next again.
    
-   If there are mapping errors, you get an error page. You can download a ZIP of your CSV files with an extra column showing the errors. Fix them, then relaunch the Import Assistant and upload your files again.
    

### Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
