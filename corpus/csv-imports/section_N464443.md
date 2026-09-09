---
id: "section_N464443"
type: "section"
title: "Exporting Selected Lists and Reports as CSV Files (CSV Export)"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Additional Import and Export Options > Exporting Selected Lists and Reports as CSV Files (CSV Export)"
parent: "chapter_N463253"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464443.html"
anchors: ["bridgehead_3849042757", "procedure_N464656", "bridgehead_3710505956"]
sha256: "00cba8d5887b5b47e4fc5d151af0eaec164d46c3d27ac7fb1f27eedc2afb0c06"
---

The Full CSV Export option in NetSuite does not currently export **all** data as CSV files.

This menu option exports the following data:

-   Accounting Lists
    
-   Classes
    
-   Contacts
    
-   Customers
    
-   Departments
    
-   Employees
    
-   Expense Categories
    
-   Items
    
-   Memorized Transactions
    
-   Notes
    
-   Other Names
    
-   Partners
    
-   Saved Reports (that you own)
    
-   Ship Items
    
-   Solutions
    
-   Tasks
    
-   Topics
    
-   Transaction Detail Report
    
-   Vendors
    

Note:

On record lists such as Customer and Item, the export mechanism exports the data based on the view you have selected for each list. For more information about options for exporting from record lists, see [Exporting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html).

## Known Excel Limitation for Values with More Than 16 Digits {#bridgehead_3849042757}

When opening a CSV file directly, Excel treats long numeric sequences as numbers and displays them using scientific notation. This treatment leads to a loss of precision when the number has more than 16 digits and to loss of information when digits at 16+ position are truncated. Even if apostrophes or double quotes are used as text qualifiers, the text within them is still recognized by Excel heuristics as a number and an additional formatting hint must be provided. This heuristics is known in Excel as the "General" format. One way to work around this limitation is to always open CSV files using the Excel's multistep Text Import Wizard. The wizard enables you to set column formatting in the last step ("Text" format). Alternatively, you can use a different Office suite, for example LibreOffice, which always displays the import wizard when opening a CSV file.

**For suggestions of other methods to export data from NetSuite, see** [Extracting Data from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464759.html) **.**

#### To export selected data as a CSV file: {#procedure_N464656}

1.  Go to _Setup > Import/Export > Export Tasks > Full CSV Export_.
    
2.  Click **Submit**.
    
    A progress bar will appear.
    
    When progress is complete, the **File Download** window appears.
    
    Note:
    
    If the export times out, you can export smaller sets of data by opening pages for the lists or reports listed above and clicking the Export - CSV button.
    
3.  In the **File Download** window, select **Save** this file to disk and then **OK**.
    
    The **Save As** window appears with **File Name** highlighted.
    
4.  In the **Save As** window, enter a file name that means something to you, like your company name and 'listsandrecords', with the extension ZIP.
    
    For example, you might name your file **WOLFELISTSANDRECORDS.ZIP**.
    
5.  Click **Save**.
    
6.  Open the ZIP file to see the titles of the generated CSV files.
    
    For example, when you unzip the exported file, you can choose the file **custjobs.csv**.
    
7.  Open the CSV file in a spreadsheet or text editor program.
    

Note:

The CSV Export function runs your saved searches and saves the results in a CSV file. A saved search that fails may cause the export to fail. So if you encounter errors during the export, review your saved searches to find the problem.

## Permissions {#bridgehead_3710505956}

Only users who have the Administrator role can use the CSV Export function.

### Related Topics

-   [Additional Import and Export Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N463253.html)
-   [Importing a Peachtree CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N463422.html)
-   [Extracting Data from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464759.html)
-   [Replacements for smbXML](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464943.html)
-   [Emailing or Faxing NetSuite Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N465450.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
