---
id: "section_N453950"
type: "section"
title: "Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html"
anchors: []
sha256: "d4f9f67d97d0038353aac41a982f7f733df51f4cbe12194bad3db11df8b21d58"
---

The Import Assistant ignores extra trailing commas and other column separators repeated at the end of fields or rows.

If any of the fields in the CSV file you import contains characters that are also used as column separators in the file (comma, semicolon, pipe, space, or tab), errors might occur during the import. To avoid errors when importing these files, either remove these characters or enclose the content of such fields in quotation marks ('for example'). This applies also to spaces before or after the value in the field. When opening a CSV file with a simple text editor, there should be no other characters that are also used as column separators in it, unless you enclose them in quotation marks.

If the CSV file you import uses commas as both value separators and decimal marks, make sure that all floating point numbers are enclosed in quotation marks (for example, '1,42').

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)
-   [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html)
-   [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html)
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
