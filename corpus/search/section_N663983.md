---
id: "section_N663983"
type: "section"
title: "Exporting Search Results"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Exporting Search Results"
parent: "chapter_N643948"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N663983.html"
anchors: []
sha256: "afe3df8df85df543b381f45bdefb55272d33b85456301afbc191b826bea80dda"
---

Note:

You can use SuiteAnalytics Workbook to query your NetSuite data using the analytics data source, which offers advanced query capabilities. For more information about SuiteAnalytics Workbook and how you can recreate your existing saved searches to workbooks, see the following topics:

-   [Getting Started with SuiteAnalytics Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158874665729.html)
    
-   [Analytics Data Source Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543418431.html)
    

You can export most NetSuite search results as files that you can open in external applications. (Popup searches and their results pages don't have the Export option.)

-   On most search pages, click **Export** to save your search results to a .csv file instead of displaying them in a NetSuite page. The **Export** button also lets you export data only.
    
-   From most search and saved search results pages:
    
    -   Click **Export - CSV** to export results to a CSV file.
        
    -   Click **Export - PDF** to export results to a PDF file.
        
    -   Click **Export - Microsoft® Excel** to export results to an XLSX file.
        

![Export search icons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/ExportIcons.png)

Note:

If your account administrator enabled the Export to Tableau® Workbooks feature for your account and assigned you the Tableau Workbooks Export permission, your search results page will also contain the Export to Tableau Workbook icon ![Export to tableau icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/ExpIconTableau.png). For more information, see [Enabling Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N232138.html) and [Permissions for Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N664557.html).

For CSV or .XLSX files, you can save the file or open it right away in Microsoft® Excel. For PDF files, they open immediately.

You can keep the relational aspects of your data by adding the Internal ID as a results column in the search to be exported.

Exported search results can help to connect NetSuite tasks with tasks in different applications. For example, if you use cash sales without Advanced Shipping and ship your items to customers through UPS, you can use the search export function to transfer shipping information from NetSuite to UPS WorldShip®. You can:

-   Create a transaction search to find all cash sales with UPS shipping items within a certain date range.
    
-   On the **Results** subtab, select the information you want exported and in what order.
    
-   Click **Submit**, and on the results page, click **Export**.
    
-   You can then open the .csv file in UPS WorldShip®.
    

If you don't see an Export button on your search results, your account administrator may not have given you the Export Lists and Perform Search permissions. You need these permissions for exporting search results. See [Permissions for Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N664557.html).

If your search takes a long time to run and you want to export results to a CSV file, try persisting search results. For more information, see [Persisting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1029112142.html).

Exports of each saved search are recorded in its execution log. This log is available to users with at least Create level of the Publish Search permission. See [Audit Trail for Saved Searches, Reports and Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688127.html).

Warning:

Users can export all address search result fields on the customer record to Excel or CSV, including the following fields: addressee, address (returns the entire address string), address1, address2, city, state, zip code, and country.

Each export format has advantages and limitations. Get to know these limitations before selecting a format, since the wrong choice can affect data accuracy and report readability. For details on all export formats and their limitation see [Comparing Export Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html#bridgehead_N575409).

### Related Topics

-   [Simple and Advanced Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N643948.html)
-   [Searchable Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N644265.html)
-   [Defining a Simple Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N645582.html)
-   [Defining an Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646177.html)
-   [Emailing Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N664260.html)
-   [Permissions for Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N664557.html)
-   [Known Excel Limitations when Exporting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3849040081.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
