---
id: "section_N612785"
type: "section"
title: "Defining KPI Scorecard Comparisons"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > KPI Scorecards > Creating a KPI Scorecard > Defining KPI Scorecard Comparisons"
parent: "section_N612318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612785.html"
anchors: ["procedure_N612824"]
sha256: "84a8c6d9a8e41ba612d90060a98cc4e96ea055cd3a868d2fb4a3ede1eaa2bf38"
---

You can define KPI scorecard comparisons when you're creating a new scorecard or editing an existing scorecard.

-   To create a new KPI scorecard, go to _Customization > Centers and Tabs > KPI Scorecards > New_. For more information, see [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html), and [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html).
    
-   To edit an existing KPI scorecard, go to _Customization > Centers and Tabs > KPI Scorecards_ and click Edit next to the KPI scorecard you want to edit.
    

#### To define KPI scorecard comparisons: {#procedure_N612824}

1.  Click **Customize** from the KPI scorecard portlet dropdown list.
    
2.  On the **KPIs** subtab of the **Content** subtab, select a KPI from the **KPI** list.
    
3.  In the **Compare Value to** list, select a KPI to compare to the first KPI you selected.
    
4.  If you selected a custom KPI from either dropdown list, go to the **Custom** subtab, and in the corresponding custom KPI list there, select the saved search to be used as the basis for the custom KPI.
    
    Only saved searches with a date field defined under **Available Filters** are available for use as custom KPIs in scorecards. The exception is if you enable the **Use Periods** option for a scorecard. Then only saved searches with a **Period** filter defined under **Available Filters** are available.
    
    Note that KPI scorecard custom KPI definitions are different from Key Performance Indicators portlet custom KPI definitions. For more information, see [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).
    
5.  Check **Compare with Previous** if you want to compare the results of this comparison to the comparison defined in the row above this one on the **KPIs** subtab.
    
6.  Select one of the following comparison types:
    
    -   **Variance (Percent)** : 100\*(B-A)/A
        
    -   **Variance (Absolute)** : B-A
        
    -   **Ratio (Percent)** : 100\*B/A
        
    -   **Ratio (Absolute)** : B/A
        
    -   **Sum** : A + B
        
7.  Check **Invert Comparison** if you want to invert the operation used to calculate the comparison type.
    
8.  Enter a **Label** for the KPI if you want something other than the KPI name to display as a row or column header in the portlet.
    
9.  Click **Add**, if you're adding a new KPI to the scorecard, or **OK**, if you're editing an existing KPI entry).
    

Warning:

KPI scorecards don't support results that are unions of two comparisons. If you enter a KPI comparison as a row on the **KPIs** subtab and also enter a date range comparison on the **Date Ranges** subtab, that KPI comparison displays a result of N/A in the KPI Scorecard portlet. To work around this limitation, try defining the comparison as a formula instead. For example, instead of entering **Quota** for **KPI**, **Sales** for **Compare Value To**, and **Variance (Percent)** for **Comparison Type**, enter **Formula (Percent)** for **KPI** and **{SALES}/{QUOTA}** for **Formula**. See [Defining KPI Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html).

### Related Topics

-   [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html)
-   [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html)
-   [Defining KPI Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html)
-   [Defining KPI Scorecard Date Ranges or Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N617699.html)
-   [Highlighting KPI Scorecard Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624192.html)
-   [Sharing a Custom KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624688.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
