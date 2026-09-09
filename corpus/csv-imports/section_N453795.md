---
id: "section_N453795"
type: "section"
title: "Tips for Using Numbers in CSV Files"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Tips for Using Numbers in CSV Files"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html"
anchors: ["bridgehead_4341191260"]
sha256: "4924ba469a64ab19502c867285201b6a7056797ef768fc22b38f061ecbb419cb"
---

Note the numbering format when you enter numbers in a CSV file. By default, many spreadsheet programs don't permit or don't show leading zeros, which can be a problem if your data needs those leading zeros. You can resolve this issue by formatting the cells in the spreadsheet program as text rather than numbers.

If you plan to import a CSV file created in Excel, be aware that Excel uses scientific notation to save long numbers to CSV files. Long numbers will be imported into NetSuite in rounded form, resulting in incorrect values. You can work around this issue by formatting long numbers such as UPC codes as 'Text' in Excel before doing a CSV import.

## Commas Used as Decimal Marks {#bridgehead_4341191260}

If you use commas as decimal marks in your CSV files, you should specify this choice in the Advanced Import Options of the Import Assistant. If appropriate, you can make it the default format for all CSV imports. To learn how to do that, see [General Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N475661.html) and [Setting CSV Import Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355760.html). If you want to set this format as the default for a subsidiary, see [Editing Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273122.html).

If the decimal mark is the same character that's used as the CSV column separator, you should add quotation marks around any floating point numbers in the CSV file you import. To learn more, see [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html).

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)
-   [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html)
-   [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html)
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
