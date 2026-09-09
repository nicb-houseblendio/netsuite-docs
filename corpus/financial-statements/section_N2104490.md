---
id: "section_N2104490"
type: "section"
title: "Cash Statement Report"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Cash Statements > Cash Statement Report"
parent: "section_N2103136"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2104490.html"
anchors: ["bridgehead_N2104587"]
sha256: "b369c7c5657d4371462b67c92dfc8675ac2fac65dbc4cda792ed4a71c922d27a"
---

The Cash Statement report lists available cash as of a selected time period. Cash Statement data can be useful for providing reference data for other financial statements, like the [Cash Flow Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103273.html).

The standard Cash Statement includes cash in bank accounts as well as undeposited funds. It includes the following rows:

-   Cash Accounts (header row)
    
    -   Bank Accounts (financial section)
        
    -   Undeposited Funds (financial section)
        
-   Total Cash (summary row)
    

The header and summary rows are linked. Each summary row is calculated either through a sum of child row amounts or through a specified formula. Standard section data are selected based on account and are grouped by accounts.

You can customize the Cash Statement in the Financial Report Builder. You can add, reorder, and change the hierarchy of rows. You can use dynamic criteria other than account type for section data, including account name, account number, class, department, location, and if you're using NetSuite OneWorld, subsidiary. In addition to account type, you can group section data by class, department, location, and if you're using NetSuite OneWorld, subsidiary. You can set formatting options for each row. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). Be aware that the Allow Web Query option isn't available for this report.

## To see the Cash Statement report: {#bridgehead_N2104587}

Go to _Reports > Banking/Budgeting > Cash Statement_.

A message will appear indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

In the footer of the report, you can select from filter lists to refilter report data. You can also select from the Column list to display report amounts by an additional dimension, including time period, class, department, location, or, if you're using NetSuite OneWorld, subsidiary. Click the More arrow button to display all footer lists. For more information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html).

Note:

Inactive classes, departments, locations, and subsidiaries are available as filters to provide historical reporting and to avoid unbalanced totals.

The Report by Period user preference determines whether report data is calculated by date range or by period. This preference is available at _Home > Set Preferences_, on the Analytics subtab. To display this report's data by date range, set this preference to Never. To view a daily report, for example, this preference must be set to Never. To display this report's date range by period, set this preference to All Reports, or to Financials Only. For more information, see [Choosing a Date or Period Range for a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N725800.html).

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

Note:

If you create a custom Cash Flow Statement that includes custom sections, its value for the Cash at Beginning of Period row is likely to be incorrect. To avoid this, create a custom Cash Statement that shares these custom sections and make that custom Cash Statement the referenced report for the Cash at Beginning of Period row. See [Customizing Cash Flow Statement Account Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103948.html).

### Related Reports

-   [Cash Statement Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2104917.html)
-   [Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2093552.html)
-   [Cash Flow Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103273.html)

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
