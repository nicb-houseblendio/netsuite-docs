---
id: "section_N439220"
type: "section"
title: "Tips for Successful CSV Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports"
parent: "chapter_N356211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html"
anchors: []
sha256: "2e52fc8f104405dc3ff6f442806af7cffc01214732108d974bac84566214b2f3"
---

To set up your CSV files correctly before importing:

-   Review guidelines for the specific record type of data you want to import, in the [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html) section.
    
-   Review information about the sublist data that can be imported for the record type you want to import, meaning the related data, for example pricing data for item records. For a complete list of sublists supported for import, and identification of which sublists are keyed for selective updates, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).
    
-   Review information about the subrecord data that can be imported for the record type you want to import, meaning a specialized set of important related data, for example item inventory details for sales order records. For information and a complete list of subrecords supported for import, see [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html) and [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html).
    
-   Determine whether auto-generated numbering is enabled for the record type of imported data, and review the related effects, in [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html).
    
-   Review general requirements and limitations for imported CSV files, in [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html) and related topics.
    
-   If your CSV file contains numbers, see [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html).
    
-   For imports that include values for check boxes and radio button fields, see [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html).
    
-   Ensure that your CSV file doesn't contain extra, unneeded characters. See [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html).
    
-   If you're importing records that contain hierarchical relationships, review the delimiters that you have used in [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html).
    
-   Ensure that name references duplicate how the name is displayed in the NetSuite user interface. For information, see [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html).
    
-   State and province names should use the short name values set up for your site. For information, see [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html).
    
-   Replace any country codes with names, in [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html).
    
-   If your file contains two columns with the same header, the import assistant ignores the value of the first column and imports only the value of the second column. If the second column has no value, the Import Assistant leaves the field empty.
    

### Additional Information

-   [CSV Imports Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html)
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)

### Related Topics

-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
