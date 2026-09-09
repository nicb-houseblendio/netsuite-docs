---
id: "section_N454355"
type: "section"
title: "Name References"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Name References"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html"
anchors: []
sha256: "0bb1b2d5683d6b699ef63ea645b56c62f8f5167ab943a8db9de080e03c62ba43"
---

Name references need to duplicate exactly the name displayed in the NetSuite user interface. Name references can be prone to error:

-   Name references may need specify a parent-child relationship between two objects using hierarchical delimiters, as described in [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html).
    
-   For names that contain spaces, HTML rendering can sometimes distort the number of spaces included, causing mismatches between CSV file values and existing records, that result in import errors. To verify the number of spaces in names, you can create a saved search with a list of names and export it.
    
-   Your preference for auto-generated numbering can affect the way that names display. For information, see [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html).
    

If you're unsure or unable to verify the name reference for a record, you should use the External ID field instead. For updates, you can use the Internal ID.

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)
-   [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html)
-   [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html)
-   [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html)
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
