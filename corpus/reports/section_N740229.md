---
id: "section_N740229"
type: "section"
title: "Adding Formula Fields to Reports"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Adding, Removing, or Reordering Report Columns > Adding Formula Fields to Reports"
parent: "section_N738669"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N740229.html"
anchors: ["procedure_N740425"]
sha256: "bbfc69a44590fb4458b730a9c6e9cc1ddaf28790ddd612b08b58045cada81939"
---

Important:

For financial statements, use the Financial Report Builder to edit columns. See [Financial Report Builder Edit Columns Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106822.html).

You can click **Add Formula Field** in the Add Fields pane to add formula-based columns to your report.

![Add formula Field button](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/add1.png)

Then you can select the formula type and the components (the **x** and the **y**) in the Report Preview pane.

![Formula type and components in the Report Preview pane.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/add2.png)

NetSuite provides six predefined formulas in the Formula Type field:

-   Sum: x+y
    
-   Difference: x-y
    
-   Percent Difference of X: ((x-y)/x)\*100
    
-   Percent Difference of Y: ((x-y)/y)\*100
    
-   Ratio: x/y
    
-   Percent Ratio: (x/y)\*100
    
-   Multiply: x\*y
    

In the fields provided, you can select columns to use for the X and Y values in the preceding formulas.

You also can choose whether to include a grand total field for the formula column in subtotal rows, and specify how the grand total is calculated:

-   Apply the formula to the subtotal row's X and Y values. This is the default.
    
-   Sum the formula column values from rows in the subtotal group. To use this method, clear the Apply Formula to Grand Total box.
    

Note:

Reports currently don't support fields based on more complex formulas, like those using SQL functions. Searches support these types of formulas for results and criteria fields. See [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html).

#### To add formula fields to reports: {#procedure_N740425}

1.  On the Reports page, click **Customize** next to the report you want to add formula fields to.
    
2.  In the Add Fields pane, click **Add Formula** Field.
    
3.  In the **Formula Type** field, select a formula to use to calculate values in the selected column.
    
4.  In the **X** and **Y** fields, select the columns to use as X and Y in the formula. For each row, the **X** and **Y** columns calculate the value for the formula field column.
    
5.  If needed, check the **Add Grand Total** box to add formula column grand totals in subtotal rows.
    
6.  If you want formula grand totals to be sums of formula column values, clear the **Apply Formula to Grand Total** box.
    
7.  Click **Preview** or **Save**.
    

Note:

Formula column values in report results are rounded to the currency precision set by the company currency format. If you're using NetSuite OneWorld, the rounding is set by the format of the subsidiary base currency.

### Related Topics

-   [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html)
-   [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html)
-   [Adding Matrix Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N741181.html)
-   [Tips for Adding Matrix Columns to a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1013122637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
