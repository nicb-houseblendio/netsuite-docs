---
id: "section_N613116"
type: "section"
title: "Defining KPI Scorecard Formulas"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > KPI Scorecards > Creating a KPI Scorecard > Defining KPI Scorecard Formulas"
parent: "section_N612318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html"
anchors: ["procedure_N613195"]
sha256: "8b080525a4ee8d57083c70621f86cc7b419a1e6211491817d1bdc6037e321530"
---

You can define formulas to calculate KPI comparisons when you're creating a new scorecard or editing an existing scorecard. These formulas are similar to those used in Excel, and can include functions and KPI IDs. A Formula popup page, available from the KPI scorecard record, offers dropdown menus that you can use to build formula expressions.

-   To create a new KPI scorecard, go to _Customization > Centers and Tabs > KPI Scorecards > New_. For more information, see [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html), and [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html).
    
-   To edit an existing KPI scorecard, go to _Customization > Centers and Tabs > KPI Scorecards_ and click Edit next to the KPI scorecard you want to edit.
    

Warning:

KPI scorecards don't support results that are unions of two comparisons. If you enter a KPI comparison as a row on the **KPIs** subtab and also enter a date range comparison on the **Date Ranges** subtab, that KPI comparison displays a result of N/A in the KPI Scorecard portlet. To work around this limitation, try defining the comparison as a formula instead. For example, instead of entering **Quota** for **KPI**, **Sales** for **Compare Value To**, and **Variance (Percent)** for **Comparison Type**, enter **Formula (Percent)** for **KPI** and **{SALES}/{QUOTA}** for **Formula**. See [Defining KPI Scorecard Comparisons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612785.html).

#### To define KPI scorecard formulas: {#procedure_N613195}

1.  Click **Customize** from the KPI scorecard portlet dropdown list.
    
2.  On the **KPIs** subtab of the **Content** subtab, select a formula from the **KPI** list. The following choices are available:
    
    -   **Formula (Currency)**
        
    -   **Formula (Numeric)**
        
    -   **Formula (Percent)**
        
3.  Enter the formula's expression in the **Formula** column. Click the **Set Formula** icon to open the Formula popup. In this popup, you can:
    
    -   Select from the **Function** list to add functions to the formula.
        
    -   Select from the **KPIs** dropdown list to add KPI IDs to the formula. For a list of IDs and their corresponding KPI names, see [KPI IDs Available for Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613450.html).
        
    -   Edit the formula directly in the **Formula** field.
        
    
    When you've finished entering the expression, click **Set**.
    
4.  If you included a custom KPI in a formula, go to the **Custom** subtab, and in the corresponding custom KPI list, select the saved search to be used as the basis for the custom KPI.
    
    Only saved searches with a date field defined under **Available Filters** are available for use as custom KPIs in scorecards. The exception is if you enable the **Use Periods** option for a scorecard. Then only saved searches with a **Period** filter defined under **Available Filters** are available.
    
    KPI scorecard custom KPI definitions are independent of the custom KPIs selected for display in the Key Performance Indicators portlet. For more information, see [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).
    
5.  If lower values are preferable for this formula's results, check the box in the **Less is More** column. When this option is enabled, downward arrows are green and upward arrows are red in the KPI scorecard portlet. (The default is the reverse.)
    
6.  If you don't want this formula's results to display in the scorecard, check the **Hidden** box. This option is available so you can use a formula as the basis for another displayed comparison.
    
7.  Enter a **Label** for the formula. This label appears as a row or column header in the portlet.
    
8.  Click **Add**, if you're adding a new KPI to the scorecard, or **OK**, if you're editing an existing KPI entry).
    

### Related Topics

-   [Creating a KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612318.html)
-   [Entering Basic Scorecard Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612623.html)
-   [Defining KPI Scorecard Comparisons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N612785.html)
-   [Defining KPI Scorecard Date Ranges or Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N617699.html)
-   [Highlighting KPI Scorecard Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624192.html)
-   [Sharing a Custom KPI Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624688.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
