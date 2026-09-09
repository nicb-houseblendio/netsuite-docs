---
id: "section_N2109173"
type: "section"
title: "Adding a Percent of Income Column to an Income Statement"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Report Builder Interface > Financial Report Builder Edit Columns Page > Adding a Percent of Income Column to an Income Statement"
parent: "section_N2106822"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html"
anchors: ["procedure_N2109275"]
sha256: "8dcc9421b18b2ac86b2013f317cbf5400565ddb9198acd10ba54710b4a4189af"
---

You can customize an income statement to include a column that displays the calculated percent of income for each total row in a selected amount column. This column is added to the right of the amount column.

The following formula is used to calculate % of Income:

**% of Income** = (`Amount` / `Total Income`) \* 100 \[rounded to the nearest 2 decimal places\]

By default, `Total Income` is the value of the original Income section of your Income Statement report, because an Income marker is set on this section. The default `Total Income` value excludes the Other Income section.

Note:

If you want to use a different row as the basis for the % of Income calculation, you need to set the **Marker** field to **Income** for that row. This marker can only be set for one row at a time. If you want to include a total of multiple rows in the % of Income calculation, you can add a formula row to compute this total, and set its **Marker** field to **Income**.

![Screenshot of the Edit Columns page of the Financial Report Builder with the Marker field outlined and set to Income](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBIncomeMarker.png)

#### To add a Percent of Income column to your Income Statement: {#procedure_N2109275}

1.  Display the income statement in the Financial Report Builder.
    
2.  Determine the row that should have a marker for use as the Total Income value.
    
    -   If you want to base the Total Income value on the default Income section, skip to step 5.
        
    -   If you want to base the Total Income value on another Income Statement row, skip to step 4.
        
    -   If you want to base the Total Income value on a computation of multiple row values, you need to add a formula row before you can set the marker. Go to step 3.
        
3.  To add a formula row computing Total Income based on multiple row values:
    
    1.  Select the row below the place where you want to add a new formula row, and from the **Add Row/Section...** list select **Add Formula Row**.
        
    2.  Enter a name for the new row in the **Formula Label** field.
        
    3.  To exclude this row's values from report results, clear the **Display Row** box.
        
    4.  Use the formula builder to enter an expression that computes a total for all of the sections and rows to be included in the Total Income value. Add each section or row value on a separate line. For each line:
        
        -   Select an operator. In most cases it will be addition (+) or possibly subtraction (-).
            
        -   Select opening parentheses if needed.
            
        -   In the **Type** field, indicate whether the value is a constant number (**Constant**) or a value from another section or row (**Row**). You'll most likely select **Row** here.
            
        -   In the **Value** field, select a section or row, or enter a constant value.
            
        -   Select closing parentheses if needed, and click **OK**.
            
    5.  Review the expression displayed at the top of the formula builder for correctness, and make adjustments as necessary.
        
    
    Following is an example layout of a formula row used for Total Income in the % of Income calculation:
    
    ![Screenshot of the Edit Columns page of the Financial Report Builder showing a formula row for calculated income displayed as a percentage](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBIncomeFormulaRow.png)
4.  On the Financial Report Builder Edit Layout page, set the **Income** marker on the row to be used as the Total Income value for the % of Income calculation.
    
    1.  In the outline, select the row.
        
    2.  Ensure the **Marker** field is set to **Income**.
        
    3.  Click **OK** in the warning dialog.
        
5.  After you've set the marker for the Total Income value, you can add the % of Income column on the Edit Columns page.
    
    1.  Click the **Edit Columns** link.
        
    2.  In the Report Preview pane, select an amount column.
        
    3.  When the amount column is highlighted, check the **Add % of Income Column** box.
        
6.  Click **Save**.
    

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2093552.html)
-   [Financial Report Builder Edit Layout Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106362.html)
-   [Financial Report Builder Edit Columns Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106822.html)
-   [Editing a Financial Statement Formula Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2117576.html)
-   [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
