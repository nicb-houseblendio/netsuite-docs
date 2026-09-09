---
id: "section_N576068"
type: "section"
title: "Limitations on CSV Exports of Data with Special Characters"
branch: "exporting-reports-searches-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Exporting Reports, Searches, and Lists > Limitations on CSV Exports of Data with Special Characters"
parent: "chapter_N575321"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N576068.html"
anchors: ["procedure_N576088"]
sha256: "6ff588549dffc9ed6dac72f5961b77f349d10248ed6273f8740e8516b45851f7"
---

If you export data in a language other than English to a CSV and open it in Excel, some special characters may not show correctly.

Exported CSV files are plain text and don't include any BOM (byte order marker) for encoding information. These files use UTF-8 encoding, but without a BOM, Excel uses a different encoding, so special (non-ASCII) characters may not show correctly.

This doesn't happen when you open an exported XLSX file in Excel, or when you open a CSV in Notepad or another text editor.

#### To avoid this issue: {#procedure_N576088}

1.  Export your data to Excel instead of CSV.
    
2.  Open the file in Excel.
    
3.  Save the file as a CSV if you want.
    
    Note that Excel adds a BOM character to the start of the CSV file.
    

### Related Topics

-   [Exporting Reports, Searches, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html)
-   [Limitations on Exports to PDF](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N575781.html)
-   [Comparing Export Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html#bridgehead_N575409)
-   [Exporting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Exporting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N663983.html)
-   [Exporting Account Registers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1511672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
