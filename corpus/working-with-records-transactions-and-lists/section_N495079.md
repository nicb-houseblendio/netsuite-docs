---
id: "section_N495079"
type: "section"
title: "Exporting Lists"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Lists > Exporting Lists"
parent: "section_N494311"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html"
anchors: ["bridgehead_3849049845"]
sha256: "112c195fd5f4bcd8e5e8257f22e877e546008f8afc06acddcdfb503e1745d7b2"
---

You can export NetSuite lists as files that you can open in external applications. The toolbar at the top of the list has icon buttons to support the following file export types:

-   Click ![Export CSV icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/ExportCSV.png) (Export - CSV) to export results to a CSV file.
    
-   Click ![Export Excel icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/ExportExcel.png) (Export - Microsoft® Excel) to export results to anXLSX file.
    
-   Click ![Export PDF icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/ExportPDF.png) (Export - PDF) to export results to a PDF file.
    

Note:

If your account administrator enabled the Tableau® Workbook Export feature and assigned you the corresponding permission, your list toolbar also contains the Export to Tableau Workbook icon ![Export to Tableau Workbook icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/ExpIconTableau.png).

For results exported to a CSV orXLSX file, you may save the file or open it immediately in Microsoft Excel. For results exported to a PDF file, the file opens immediately.

NetSuite generates Internal ID values for each record. These values, which serve as unique identifiers, are always included as a results column in the list to be exported.

Each export format has advantages and limitations. Review the limitations before selecting a preferred format. The format you select can affect data accuracy and report readability. For details on the export formats and their limitations, see [Comparing Export Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html#bridgehead_N575409).

Note:

If exported lists and files are marked as encrypted or read-only, you need to know your password for such files.

## Known Excel Limitation for Values with More Than 16 Digits {#bridgehead_3849049845}

When you open a CSV file directly, Excel treats long numeric sequences as numbers and displays them using scientific notation. This causes a loss of precision when the number has more than 16 digits and to lost information when digits beyond position 16 are truncated. Even when the text is qualified by apostrophes or double quotes, it's recognized by Excel as a number. To avoid this limitation, open CSV files using the Excel multistep Text Import Wizard. The wizard enables you to set column formatting in the last step ("Text" format).

### Related Topics

-   [Working with Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N494311.html)
-   [Using Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html)
-   [Using the Recent Records Menu](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495728.html)
-   [Working with List Views, Sublist Views, and Dashboard Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495842.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
