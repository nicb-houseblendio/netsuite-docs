---
id: "section_N609047"
type: "section"
title: "Custom KPIs"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Key Performance Indicators > Custom KPIs"
parent: "chapter_N595760"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html"
anchors: []
sha256: "baea63715bd0e34fed389b5ed43924e7dae251f5a662da7f4b3172fb454ceaf6"
---

NetSuite provides over 75 standard KPIs that you can display in a dashboard's Key Performance Indicators portlet, or use for calculations in a KPI scorecard. These standard KPIs provide quick summaries of standard NetSuite report data and enable you to drill down into the full reports for more detail.

You may have other important data that you would like to display as a KPI on your dashboard, that is not available from standard reports. In this case, you can find a preexisting saved search that compiles this data or create a new saved search for this purpose.

For information, see:

-   [Selecting an Existing Search to be a Custom KPI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609351.html)
    
-   [Creating a New Search to be a Custom KPI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609600.html)
    

After you have identified an appropriate saved search, you can define it as a data source for a custom KPI.

-   You can display up to ten custom KPIs in each Key Performance Indicators portlet. When a custom KPI is displayed in the portlet, you can click it to drill down to detailed results from its saved search, and click a Trend Graph icon to display its data in a popup trend graph. For information, see [Adding a Custom KPI to the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609834.html).
    
-   You can define up to ten custom KPIs to be used in each KPI scorecard portlet's calculations. For information, see [Using a Custom KPI in a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N610062.html).
    
-   Custom KPIs displayed in the Key Performance Indicators portlet are also available for display in KPI Meter portlets. You can display up to three KPI meters on a dashboard. For information, see [KPI Meters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N605338.html).
    
-   Custom KPI data can also be displayed in Trend Graph portlets. You can add up to five Trend Graph portlets. For information, see [Setting Up Trend Graph Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N606898.html).
    
-   Custom KPI definitions for individual KPI scorecards, the Key Performance Indicators portlet, and Trend Graph portlets are all independent of each other.
    

For a saved search to be used as a custom KPI that displays results for multiple date ranges in the Key Performance Indicators portlet, a KPI scorecard, a trend graph, or a KPI meter, the search definition must meet the following requirements:

-   Not include any date fields defined as filters on the Criteria subtab. See [Defining Standard Search Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646693.html).
    
-   Have exactly one field with a summary type (such as count, group, or sum) defined on the Results subtab. The rest of the fields on the Results subtab should not use any summary types. See [Defining Summary Types to Roll Up Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648820.html).
    
-   Have a date field defined as an available filter on the Available Filters subtab. See [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html).
    

### Related Topics

-   [Key Performance Indicators](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N595760.html)
-   [Setting Up the Key Performance Indicators Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N596767.html)
-   [KPI Meters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N605338.html)
-   [Trend Graphs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N605811.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
