---
id: "section_N464759"
type: "section"
title: "Extracting Data from NetSuite"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Additional Import and Export Options > Extracting Data from NetSuite"
parent: "chapter_N463253"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464759.html"
anchors: ["bridgehead_N464855", "bridgehead_N464892"]
sha256: "c279edf6b5ea8241f4fe753bca0c0e590904e6ae8dd3c20f05f42053003f771f"
---

NetSuite provides an export function at _Setup > Import/Export > Export Tasks > Full CSV Export_, described in [Exporting Selected Lists and Reports as CSV Files (CSV Export)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464443.html).

If this export functionality doesn't meet your needs, you can use a combination of the following options to extract detailed data from NetSuite:

-   Exporting saved search results to CSV files. For information, see [Exporting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N663983.html).
    
-   Exporting report results as CSV files. For information, see [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html).
    
-   Writing a SOAP web services program to query record data. For information, see [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html).
    
-   Using SuiteAnalytics Connect to access NetSuite data through an ODBC, JDBC, or ADO.NET driver and an external application such as Microsoft Excel or Crystal Reports. For information, see [SuiteAnalytics Connect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3963845427.html). Note that ODBC access is an additional service with an associated fee.
    

You can use the detailed records that you obtain from these approaches to create spreadsheets of relevant information. All of these approaches can preserve the relational aspects of data, if you export the Internal ID with each data row.

## Best Practices for Financial Data Extraction {#bridgehead_N464855}

Reports can be more useful than saved searches for getting transaction information, since they provide easier matching of totals.

-   One way to organize things is to place purchase transactions in one spreadsheet and sales transactions in another.
    
-   You can customize the Transaction Detail report to filter by transaction type and include columns like transaction number and memo before exporting.
    
-   Sometimes you'll need to set date range filters to keep reports from running too long, and run the same report multiple times to get data from different date ranges.
    

## Best Practices for CRM Data Extraction {#bridgehead_N464892}

You can use saved searches to pull CRM data from NetSuite.

-   Saved searches are organized by record type, such as contact, customer, and vendor; and you should organize extracted information by record type as well.
    
-   Notes field data on entity records (such as customers and vendors) can be extracted through a separate type of search, either System Note or User Note. In some cases, you may need to run separate searches and combine their data into an aggregated spreadsheet. In other cases, you can access notes data through a search for Contacts, Customers, or Vendors.
    
    For information about saved searches, see [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html).
    

### Related Topics

-   [Additional Import and Export Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N463253.html)
-   [Importing a Peachtree CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N463422.html)
-   [Exporting Selected Lists and Reports as CSV Files (CSV Export)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464443.html)
-   [Replacements for smbXML](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N464943.html)
-   [Emailing or Faxing NetSuite Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N465450.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
