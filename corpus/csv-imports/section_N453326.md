---
id: "section_N453326"
type: "section"
title: "General CSV File Conventions"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > General CSV File Conventions"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html"
anchors: []
sha256: "6abb7b0b17c49d7e605d330e90ccd477a4864490a4953e6e15ea433fc93e8857"
---

To be successfully imported, CSV files must contain values separated by **commas** or other supported column separators, such as the **semicolon**, **pipe**, **space**, and **tab**.

CSV files typically include a top row with column names as headers, and multiple rows of data below.

Review the following tips as you're setting up CSV files for the Import Assistant:

-   The Import Assistant has a limit of 25,000 records or 50 MB per import job. For a multiple file upload, all files combined must be under these limits.
    
    **You should break large import jobs into smaller chunks to improve performance.**
    
-   The Import Assistant attempts to map each CSV file's column headers to field names for the selected NetSuite record type, so that data can be imported into the appropriate NetSuite fields. The Assistant includes a Field Mapping page where you can review and edit its mappings, and define mappings for columns that the Assistant was unable to map.
    
    If a file contains fields of data without column headers, the Import Assistant doesn't import the trailing fields' data.
    
-   Blank lines at the end of an imported CSV file are not included in the import.
    
-   You can specify name references in a CSV file, but reference types such as External ID or Internal ID are preferable. Data values for fields used as reference types must be written exactly as they appear in dropdown lists in the NetSuite record form. For more information, see [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html), [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html), and [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html).
    
-   If your account is using NetSuite OneWorld, the Subsidiary field is a required field for the following record types: Chart of Accounts, Contacts, Customers, Employees, Jobs, Leads, Partners, Prospects, and Vendors. For imports of these record types, you must include in your CSV file a field that can be mapped to the NetSuite Subsidiary field. If the import attempts to add or update records in a OneWorld account without identifying the subsidiary, the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.
    
-   If your system's regional settings designate commas as decimal separators, CSV files that you generate with Microsoft Excel use semi-colons as CSV value separators. To learn more about the number formats supported for CSV imports, see [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html).
    
-   Go to _Home > Set Preferences_. On the General subtab, scroll down to Formatting. Make sure that the CSV Column Delimiter option is set to the column separator used in the CSV files you're planning to import.
    
-   If you're importing CSV data in a language different from your NetSuite language preferences, the data import might be slow. To improve the import speed, change your NetSuite language settings at _Home > Set Preferences_ before importing CSV data, so that your language settings match the language of the CSV file you're importing.
    

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html)
-   [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html)
-   [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html)
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
