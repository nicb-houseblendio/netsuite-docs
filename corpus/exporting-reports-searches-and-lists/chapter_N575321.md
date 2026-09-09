---
id: "chapter_N575321"
type: "chapter"
title: "Exporting Reports, Searches, and Lists"
branch: "exporting-reports-searches-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Exporting Reports, Searches, and Lists"
parent: "book_N473219"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html"
anchors: ["bridgehead_N575409", "bridgehead_N575422", "bridgehead_N575467", "bridgehead_N575542", "bridgehead_N575608", "bridgehead_4374700795"]
sha256: "f70982a0a79b7c9848fc1494cecaaefaa40e988f0c31f4c9ac586ea06c21e622"
---

You can export reports, searches and lists into various formats. Exporting provides you with more flexibility to review and analyze your business's data.

For information about exporting, see the following sections.

-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
    
-   [Exporting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N663983.html)
    
-   [Exporting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html)
    

## Comparing Export Formats {#bridgehead_N575409}

Each export format has its own advantages and limitations, listed below:

-   [Exporting to Word](#bridgehead_N575422)
    
-   [Exporting to PDF](#bridgehead_N575467)
    
-   [Exporting to Excel](#bridgehead_N575542)
    
-   [Exporting to CSV](#bridgehead_N575608)
    
-   [Exporting to Tableau](#bridgehead_4374700795)
    

## Exporting to Word {#bridgehead_N575422}

-   **Supported Versions** - Reports are exported in Word 97 - 2003 format.
    
-   **Expand/collapse** - Settings are maintained. The report will be displayed as it is currently viewed on the screen. If you have collapsed a section of the report (hiding some rows), then those rows won't be available in the word document. You won't be able to expand and view hidden rows.
    
-   **Company Logo** - The logo will display in the exported Word report if you've set it as a preference in the Analytics subtab at _Home > Set Preferences_.
    

## Exporting to PDF {#bridgehead_N575467}

-   **Expand/collapse** - Settings are maintained. The report will be displayed as it is currently viewed on the screen. If you have collapsed a section of the report (hiding some rows), then those rows won't be available in the word document. You won't be able to expand and view hidden rows.
    
-   **Company Logo** - The logo will display in the exported Word report if you've set it as a preference in the Analytics subtab at _Home > Set Preferences_. However, the uploaded image is not resized to fit the PDF layout, it's used as is.
    
-   **Formatting** - By default, a PDF of an exported report/search has a font size of 8 and a portrait orientation. You can change these settings by updating the PDF Page Orientation and PDF Font Size preferences on the Analytics subtab at _Home > Set Preferences_. See [Setting Formats for Reports Exported to PDF](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N717175.html).
    
-   **Size Limitations** - Exported PDFs currently have some output limitations. You may encounter issues if your report results include a large number of rows or columns, or extremely long field values. You can't export reports with more than 30 columns and NetSuite limits records for reports with more than 10 columns. To get around these issues, try adding criteria to reduce the number of rows and columns, or remove fields with long values. For details, see [Limitations on Exports to PDF](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N575781.html).
    

## Exporting to Excel {#bridgehead_N575542}

-   **Supported Versions** - NetSuite exports files in XLSX format.
    
-   **Expand/collapse** - Settings aren't maintained. All rows in the report will be exported, any collapsed rows will appear fully expanded in Excel.
    
-   **Company Logo** - The company logo is not displayed in Excel exports, even if you've enabled the Print Company Logo option on the Analytics subtab at _Home > Set Preferences_.
    
-   **Unicode** - Supported.
    
-   **Decimal precision** - Excel keeps the same high decimal precision you see in the report or search.
    
-   **Limitations** - For item records with the Detailed Description field, the length of this field is limited to 1,300 characters in search results.
    

## Exporting to CSV {#bridgehead_N575608}

-   **Expand/collapse** - Settings aren't maintained. All rows in the report will be exported, any collapsed rows will appear fully expanded in Excel.
    
-   **Company Logo** - The company logo isn't exported.
    
-   **Unicode** - Not supported.
    
-   **Decimal precision** - All decimal numbers are limited to 2 decimal places. If you need more precision, you should export to Excel first, then save it as a CSV file.
    
-   **Handling Special Characters** - If you open a CSV file in Excel that has data in languages other than English, some special characters may not show correctly. If that happens, export to Excel instead, then save it as a CSV file. For more information, see [Limitations on CSV Exports of Data with Special Characters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N576068.html).
    

## Exporting to Tableau {#bridgehead_4374700795}

-   **Supported Versions** - Tableau Desktop 8.3 or later.
    
-   **Expand/collapse** - Settings aren't maintained. All rows included in the report or search results will be exported.
    
-   **Company Logo** - The company logo is not displayed when the report or search is exported as a Tableau workbook.
    
-   **Unicode** - Supported.
    
-   **Decimal precision** - Tableau Desktop keeps the same precision you see in each report or search.
    
-   **Limitations** - Sort settings may not be kept when you export search or report results as a Tableau workbook.
    

See the following topics for export limitations:

-   [Limitations on Exports to PDF](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N575781.html)
    
-   [Limitations on CSV Exports of Data with Special Characters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N576068.html)
    

### Related Topics

-   [NetSuite Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N473219.html)
-   [NetSuite Basics Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N473387.html)
-   [Getting Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N336026.html)
-   [Navigating NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474404.html)
-   [Logging in to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1492022011.html)
-   [Logging out of NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158801369869.html)
-   [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html)
-   [Using SuiteAnalytics Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7112240791.html)
-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)
-   [Working with Your Calendar and Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N499702.html)
-   [Working with Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N512006.html)
-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Permission to Export Report & Search Results](https://suiteanswers.custhelp.com/app/answers/detail/a_id/34121)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
