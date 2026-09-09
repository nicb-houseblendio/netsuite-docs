---
id: "section_N597713"
type: "section"
title: "Setting Up KPI Comparisons"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Key Performance Indicators > Setting Up the Key Performance Indicators Portlet > Setting Up KPI Comparisons"
parent: "section_N596767"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N597713.html"
anchors: ["procedure_N597763"]
sha256: "139f82efdbcc92d6fbaace30e479e604067778f33414aece2d6fe2c3739ee8c0"
---

A variety of date ranges are available for KPI comparisons, which allow you to compare results for two date ranges or periods.

Many additional date ranges and period ranges are available for comparisons in KPI scorecards. Each scorecard can include multiple lines of KPI data and comparisons for multiple data ranges or periods. If you want to display KPI results for more than two date ranges or periods, see [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html).

#### To set up KPI comparisons: {#procedure_N597763}

1.  Click **Set Up** in your Key Performance Indicators portlet's menu.
    
2.  In the Set Up Key Performance Indicators popup, if the KPI is not displayed, click **Add Standard KPIs** or **Add Custom KPIs**, select the KPI, and click **Done**.
    
3.  In the **Range** column for the KPI, choose the first period of time for which data should be included in the KPI.
    
4.  Check the box in the **Compare** column.
    
5.  In the **Compare Range** column, choose the second time period for which data should be included in the KPI (and compared with the first period's data).
    
6.  Repeat steps 2 through 5 for each indicator that you want to include a comparison.
    
7.  Click **Save**.
    

After these setup steps, the KPI in your Key Performance Indicators Portlet now displays columns for the current period's metric, the previous period's metric, and the percentage change.

If you've set up a comparison for a custom KPI and the results aren't showing up right, the saved search it's based on might not meet the requirements. The saved search definition must:

-   Not include any date fields defined as filters on the Criteria subtab
    
-   Have only one field with a summary type (such as group, sum, or count) defined on the Results subtab.
    
-   Have a date field defined as an available filter on the Available Filters subtab.
    
    For more information, see [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).
    

### Related Topics

-   [Setting Up the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N596767.html)
-   [Viewing Key Performance Indicator Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N597348.html)
-   [Highlighting KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N600850.html)
-   [Standard Key Performance Indicators Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N601098.html)
-   [Resolving Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1026010425.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
