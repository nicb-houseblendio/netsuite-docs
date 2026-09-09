---
id: "section_N2101379"
type: "section"
title: "Comparative Balance Sheet Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Balance Sheets > Comparative Balance Sheet Report"
parent: "section_N2098170"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2101379.html"
anchors: ["bridgehead_N2101833"]
sha256: "9cbeb705a017e6d95110773e7a8c4b17bdd219753d9440581a693e7e5a20c7b7"
---

The Comparative Balance Sheet report compares the category and worth of each account across two or more specified time periods. You can use this report to compare your company's performance with previous years. This comparison helps you to measure your company's progress and to make future projections.

This report includes an Amount column that defaults to the current date range or period, and a Comparison Amount column that defaults to the last year or last fiscal year. You select a value in the As Of list in the report footer to change the date or period for Amount column data. The date of the Comparison Amount column changes automatically because it's defined by a alternate range that is relative to the Amount column date. For more information about comparison columns, see [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html).

The standard Comparative Balance Sheet includes the following rows:

-   **ASSETS (header row)**
    
    -   Current Assets (header row)
        
        -   Bank (financial section)
            
        -   Accounts Receivable (financial section)
            
        -   Unbilled Receivable (financial section)
            
        -   Other Current Asset (financial section)
            
    -   Total Current Assets (summary row)
        
    -   Fixed Assets (financial section)
        
    -   Other Assets (financial section)
        
-   **Total ASSETS (summary row)**
    
-   **LIABILITIES & EQUITY (header row)**
    
    -   Current Liabilities (header row)
        
        -   Accounts Payable (financial section)
            
        -   Credit Card (financial section)
            
        -   Other Current Liability (financial section)
            
    -   Total Current Liabilities (summary row)
        
    -   Long Term Liabilities (financial section)
        
    -   Equity (header row)
        
        -   Equity (financial section)
            
        -   Retained Earnings (header row)
            
        -   Total Retained Earnings (summary row)
            
        -   Net Income (referenced row from Income Statement)
            
        -   Cumulative Translation Adjustment (financial section)
            
            (OneWorld accounts with multi-currency enabled only)
            
    -   Total Equity (summary row)
        
-   **Total LIABILITIES & EQUITY (summary row)**
    

Header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. Standard section data are selected based on account type and are grouped by accounts. The date you select in the footer is used to filter the column you want to compare.

## To see the Comparative Balance Sheet report: {#bridgehead_N2101833}

Go to _Reports > Financial > Comparative Balance Sheet_.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from lists to refilter report data. You can also select from the Column list to display report amounts by an additional dimension, including class, department, location, or if you're using NetSuite OneWorld, subsidiary. Click the More arrow button to display all footer lists. After you change values in the lists, click Refresh to see the changes. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html). The Allow Web Query option isn't available for this report.

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Report by Period user preference determines whether report data is calculated by date range or by period. This preference is available at _Home > Set Preferences_ on the Analytics subtab. To display this report's data by date range, set this preference to Never. To display this report's date range by period, set this preference to All Reports, or to Financials Only. For more information, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).

Click Customize to open the Financial Report Builder. Using the Financial Report Builder, you can add, reorder, and change the hierarchy of rows. You can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can set formatting options for each row. To change the date for your comparison column, select the column in the Edit Columns view and select a different Alternate Period Range. For example, to use the previous period in the comparison column, select Last Period for the Alternate Period Range. For more information about customizing the report, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html).

### Related Reports

-   [Generating an Insight on a Comparative Balance Sheet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0217070850.html)
-   [Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2098310.html)
-   [Balance Sheet Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2100658.html)
-   [Multi-Book Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495037141.html)
-   [Multi-Book Balance Sheet Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495119693.html)
-   [Multi-Column Balance Sheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2102164.html)

### Related Topics

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
