---
id: "section_N612318"
type: "section"
title: "Creating a KPI Scorecard"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > KPI Scorecards > Creating a KPI Scorecard"
parent: "chapter_N610592"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html"
anchors: ["procedure_N612342"]
sha256: "314a25461b00e73b4ed7b4d3802d4499a24127fd786c358ca18dc134347629a0"
---

NetSuite enables you to create custom scorecards that can be displayed in the KPI Scorecard dashboard portlet.

#### To create a new KPI scorecard: {#procedure_N612342}

1.  Go to _Customization > Centers and Tabs > KPI Scorecards > New_.
    
    If this menu option is not available, the KPI Scorecards feature may not be enabled. See [Enabling the KPI Scorecards Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N611007.html). Check with your account administrator to ensure you have the KPI Scorecards permission.
    
2.  At the top of the page, you can enter basic scorecard information. See [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html).
    
3.  On the **KPIs** subtab of the **Content** subtab, you can add KPIs and define their comparisons, and add formulas and define formula expressions.
    
    ![KPIs subtab on the KPI Scorecard page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/kpi_scorecard1.png)
    -   Scorecards can intermingle KPIs and formulas and compare them to each other, so you define KPIs and formulas in the same place using some slightly different fields on the subtab.
        
        -   For KPI steps, see [Defining KPI Scorecard Comparisons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612785.html).
            
        -   For formula steps, see [Defining KPI Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html).
            
    -   If you define custom KPIs to be used in scorecards, you need to define their underlying saved searches on the **Custom** subtab of the **Content** subtab.
        
        Only saved searches with a date field defined under **Available Filters** are available for use as custom KPIs in scorecards. The exception is if you enable the **Use Periods** option for a scorecard. Then only saved searches with a **Period** filter defined under **Available Filters** are available.
        
    -   After you've entered KPIs and formulas, you can reorder them by dragging and dropping or using the **Move** buttons.
        
4.  On the **Date Ranges** (or **Periods**) subtab of the **Content** subtab, you can define multiple date ranges (or periods). These date ranges apply to all scorecard data. See [Defining KPI Scorecard Date Ranges or Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N617699.html).
    
    After you've entered date ranges, you can reorder them by dragging and dropping or using the **Move** buttons.
    
5.  On the **Highlighting** subtab of the content subtab, you can set highlighting options to make results more visible in KPI Scorecard portlets. See [Highlighting KPI Scorecard Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624192.html).
    
6.  On the **Audience** subtab, you can define who has access to your scorecard, meaning who can place it in their KPI Scorecard portlet. You can base this definition on roles, departments, subsidiaries, groups, employees, or partners. See [Sharing a Custom KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624688.html).
    
7.  When you've completed all steps to define the scorecard, click **Save**.
    

You can use SuiteCloud Development Framework (SDF) to manage KPI scorecards as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). You can use the Copy to Account feature to copy an individual KPI scorecard to another of your accounts. Each KPI Scorecard page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

### Related Topics

-   [KPI Scorecards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N610592.html)
-   [Enabling the KPI Scorecards Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N611007.html)
-   [Adding a KPI Scorecard Portlet to a Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612018.html)
-   [Editing a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624476.html)
-   [Financial Ratios Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624824.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
