---
id: "section_N617699"
type: "section"
title: "Defining KPI Scorecard Date Ranges or Periods"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > KPI Scorecards > Creating a KPI Scorecard > Defining KPI Scorecard Date Ranges or Periods"
parent: "section_N612318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N617699.html"
anchors: ["procedure_N617795"]
sha256: "973bfb463fe9fd86f1ad6c1a92fc48b6b9affe298d22cbcee7fc0d4546dbc658"
---

You can define the date ranges to use in KPI data calculations when you're creating a new scorecard or editing an existing scorecard.

-   To create a new KPI scorecard, go to _Customization > Centers and Tabs > KPI Scorecards > New_. For more information, see [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html), and [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html).
    
-   To edit an existing KPI scorecard, go to _Customization > Centers and Tabs > KPI Scorecards_ and click Edit next to the KPI scorecard you want to edit.
    

Note:

If you've checked the **Use Periods** box on a KPI scorecard, you need to define periods rather than date ranges, and the name of the **Date Ranges** subtab is changed to **Periods**. Please note that you can't clear the **Use Periods** box after the KPI scorecard has been saved.

#### To define date ranges for a KPI scorecard: {#procedure_N617795}

1.  On the **Date Ranges** subtab of the **Content** subtab, in the **Range** column, specify date ranges to be applied to all KPI scorecard data.
    
2.  In the **Compare Value to** field, select a date range to compare to the first range you selected.
    
3.  Check **Compare with Previous** if you want to compare the results for this comparison to the date ranges listed above this one.
    
4.  Select one of the following comparison types:
    
    -   **Variance (Percent)**: 100\*(B-A)/A
        
    -   **Variance (Absolute)**: B-A
        
    -   **Ratio (Percent)**: 100\*B/A
        
    -   **Ratio (Absolute)**: B/A
        
    -   **Sum**: A + B
        
5.  Check the box in the **Invert Comparison** column if you want to invert the operation used to calculate the comparison type.
    
6.  Enter a **Label** for this date range. This label appears as a column or row header in the portlet.
    
7.  Click **Add**, if you're adding a new KPI to the scorecard, or **OK**, if you're editing an existing KPI entry).
    

If you select multiple relative date ranges, such as 2 months ago, you can display the explicit dates in the KPI Scorecard portlet, by checking the Show Date Row box in the KPI Scorecard Setup dialog. See [Adding a KPI Scorecard Portlet to a Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612018.html).

Warning:

KPI scorecards don't support results that are unions of two comparisons. If you enter a KPI comparison as a row on the **KPIs** subtab and also enter a date range comparison on the **Date Ranges** subtab, that KPI comparison displays a result of N/A in the KPI Scorecard portlet. To work around this limitation, try defining the comparison as a formula instead. For example, instead of entering **Quota** for **KPI**, **Sales** for **Compare Value To**, and **Variance (Percent)** for **Comparison Type**, enter **Formula (Percent)** for **KPI** and **{SALES}/{QUOTA}** for **Formula**. See [Defining KPI Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html).

### Related Topics

-   [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html)
-   [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html)
-   [Defining KPI Scorecard Comparisons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612785.html)
-   [Defining KPI Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html)
-   [Highlighting KPI Scorecard Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624192.html)
-   [Sharing a Custom KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624688.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
