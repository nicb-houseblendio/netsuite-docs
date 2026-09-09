---
id: "section_N2103273"
type: "section"
title: "Cash Flow Statement Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Cash Statements > Cash Flow Statement Report"
parent: "section_N2103136"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103273.html"
anchors: ["bridgehead_N2103623"]
sha256: "fcadf3c517a842e0af604fdbe761cfbccb7ad17a2b5a82c91d85ddc7c5aea2f3"
---

The Cash Flow Statement report shows how your company's cash position has changed over a period of time. This helps you assess your company's current financial position and set goals for its future. This report is also useful for investment and credit decisions.

This report includes activities that affect the cash balance during the selected time period, including operating, investing, and financing activities. Operating activities begin with the net income amount referenced from the Income Statement, and include adjustments for changes in account balances that affect available cash. Amounts for all of the activities are summed to arrive at the net change in cash for the period. Cash amounts at the beginning and end of the period are referenced from the [Cash Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2104490.html).

The standard Cash Flow Statement includes the following rows:

-   Operating Activities (header row)
    
    -   Net Income (referenced row from Income Statement)
        
    -   Adjustments to Net Income (header row)
        
        -   Accounts Receivable (financial section)
            
        -   Unbilled Receivable (financial section)
            
        -   Inventory Asset (financial section)
            
        -   Other Current Asset (financial section)
            
        -   Accounts Payable (financial section)
            
        -   Payroll Liabilities (financial section)
            
        -   Sales Tax Payable (financial section)
            
        -   Other Current Liabilities (financial section)
            
    -   Total Adjustments to Net Income (summary row)
        
-   Total Operating Activities (summary row)
    
-   Investing Activities (header row)
    
    -   Fixed Asset (financial section)
        
    -   Other Asset (financial section)
        
-   Total Investing Activities (summary row)
    
-   Financing Activities (header row)
    
    -   Long Term Liabilities (financial section)
        
    -   Opening Balance Equity (financial section)
        
    -   Other Equity (financial section)
        
-   Total Financing Activities (summary row)
    
-   **Net Change in Cash for Period (formula row)**
    
-   **Cash at Beginning of Period (referenced row from Cash Statement)**
    
-   Effect of Exchange Rate on Cash (financial section)
    
    (OneWorld accounts with multi-currency enabled only)
    
-   **Cash at End of Period (formula row)**
    

Header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. Standard section data are selected based on account type and are grouped by accounts.

For NetSuite OneWorld with multi-currency enabled, consolidated cash flow statement reports include an Effect of Exchange Rate on Cash row. This row adjusts for the effects of rate differences in cash flow statement accounts for the period. This adjustment ensures the cash flow statement's Cash at End of Period is consistent with the balance sheet's Bank or cash equivalent. This row is a calculated amount that accounts for the related amount in the Cumulative Translation Adjustment (CTA) account used in the consolidated balance sheet. Generally no postings are made for exchange rate adjustment amounts included in this row. Exchange rate adjustment postings, when they do occur, are made to the CTA account. The adjustment calculated for the Effect of Exchange Rate on Cash row adds or subtracts any CTA amount as necessary.

You can customize the Cash Flow Statement in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can use dynamic criteria other than account type for section data, including account name, account number, class, department, location, and if you're using NetSuite OneWorld, subsidiary. In addition to account type, you can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can set formatting options for each row. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). Be aware that the Allow Web Query option isn't available for this report.

## To see the Cash Flow Statement: {#bridgehead_N2103623}

Go to Reports > Financial > Cash Flow Statement.

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from filter lists to refilter report data. You can also select from the Column list to display report amounts by an additional dimension, including time period, class, department, location, or, if you're using NetSuite OneWorld, subsidiary. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

The Report by Period user preference determines whether report data is calculated by date range or by period. This preference is available at _Home > Set Preferences_, on the Analytics subtab. To display this report's data by date range, set this preference to Never. To display this report's date range by period, set this preference to All Reports, or to Financials Only. For more information, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).

The Net Cash Flow and Operating Cash Flow key performance indicators (KPIs) can be added to your dashboard to provide at-a-glance views of totals from the Cash Statement report. For more information about KPIs, see [Setting Up the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N596767.html).

Note:

If you create a custom Cash Flow Statement that includes custom sections, its value for the Cash at Beginning of Period row is likely to be incorrect. To avoid this, create a custom Cash Statement that shares these custom sections and make that custom Cash Statement the referenced report for the Cash at Beginning of Period row. See [Customizing Cash Flow Statement Account Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103948.html).

### Related Reports

-   [Generating an Insight on a Cash Flow Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0217072307.html)
-   [Cash Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2104490.html)

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
