---
id: "section_N453857"
type: "section"
title: "Values in CSV Files"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Values in CSV Files"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html"
anchors: []
sha256: "dd62b2a3a14fc26f62957ebbc04afe8fdcc47e730315af399d7960592b589c52"
---

You should use only 'TRUE' or 'FALSE' as values for radio button fields to ensure that import of these fields is successful.

-   Currently, radio button fields don't accept any other values.
    
-   The Individual field for entities is an exception that accepts all forms of True or False. For information, see [Customers as Individuals or Companies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html#bridgehead_N385403).
    
-   Check boxes accept the following forms for true values: TRUE, YES, T, Y.
    
-   Check boxes accept the following forms for false values: FALSE, NO, F, N
    

When working with check boxes and radio buttons, note the following:

-   True and false values are case insensitive.
    
-   The Import Assistant doesn't honor localization. This means that true and false values aren't accepted in languages other than English.
    
-   The Import Assistant doesn't accept any other true or false value than the eight values listed.
    

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)
-   [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html)
-   [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html)
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
