---
id: "section_N2117576"
type: "section"
title: "Editing a Financial Statement Formula Row"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Rows > Editing a Financial Statement Formula Row"
parent: "section_N2115374"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2117576.html"
anchors: ["procedure_N2117618", "bridgehead_N2117777", "bridgehead_N2117790", "bridgehead_N2117807", "bridgehead_N2117839", "procedure_N2117872"]
sha256: "98d0c740709960dba7d01d177ae34b7fc841c0ef95dbfb72ecb16aaa782d77fd"
---

A formula row can be used to display a value calculated from the values of other rows in a financial statement. The Financial Report Builder lets you define and edit the expression used to calculate a formula row value. It also lets you edit other formula row characteristics in custom financial statements.

The following screenshot illustrates the editing of a formula row in the Financial Report Builder:

![Screenshot showing where you edit formula rows on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBFormulaRowEdit.png)

#### To edit a formula row: {#procedure_N2117618}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, do one of the following:
    
    -   Select the row below the place where you want to add a new formula row, and select **Add Formula Row** from the **Add Row/Section** list.
        
    -   Select an existing formula row.
        
3.  Complete any of the following tasks:
    
    -   [Editing a Formula Row Header Label](#bridgehead_N2117777)
        
    -   [Modifying Formula Row Hierarchy](#bridgehead_N2117790)
        
    -   [Modifying Formula Row Format Options](#bridgehead_N2117807)
        
    -   [Defining a Formula Row Expression](#bridgehead_N2117839)
        

Note:

If you want to use a formula row to calculate % of Expense or % of Income column values for a custom income statement, set its **Marker** field to **Expense** or **Income**. See [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html) or [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html).

## Editing a Formula Row Header Label {#bridgehead_N2117777}

You can edit the Formula Label for a formula row. This is the row's text. To hide this row, clear the **Display Row** box.

## Modifying Formula Row Hierarchy {#bridgehead_N2117790}

You can change a formula row's placement in the report hierarchy by selecting a different row in the Child Of dropdown. The formula row is moved under the row you select here. This move is reflected in the Layout outline.

Alternatively, you can drag and drop a formula row in the Layout outline to change its hierarchy.

## Modifying Formula Row Format Options {#bridgehead_N2117807}

You can modify the formatting of text, lines, and background color for a formula row. You can also indicate whether to show currency symbols, reverse signs, or include text before or after the formula row amount.

Note:

Checking the **Reverse Sign** box for a row affects all dynamic total calculations that include that row's value. Always run the report and review the accuracy of all total rows if you use this option.

For more information, see [Setting Financial Statement Formatting Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119303.html).

## Defining a Formula Row Expression {#bridgehead_N2117839}

You can define the expression used to calculate a value for a formula row, using constants and values from other rows in the financial statement.

![Screenshot showing the expression builder for a formula row on the Edity Layout page of the Financial Report Builder and an example to calculate gross profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBFormulaExpression.png)

## To define an expression to calculate a formula row value: {#procedure_N2117872}

With the formula row selected in the Layout outline, use the formula builder available in the Summary box to enter an expression. Add each value on a separate line.

1.  Select an operator if needed. Addition (+), subtraction (-), multiplication (\*), division (/), and percentage (%) operators are available.
    
2.  Select opening parentheses if needed.
    
3.  Indicate whether the value is a constant number (**Constant**) or a value from another row in the report (**Row**).
    
4.  Enter the value.
    
    If the **Type** is **Constant**, enter a number in the field.
    
    If the **Type** is **Row**, select a value from the dropdown list.
    
5.  Select closing parentheses if needed.
    
6.  Repeat until the formula expression is complete.
    
7.  Review the expression displayed at the top of the formula builder for correctness, then make adjustments as necessary.
    

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Statement Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115374.html)
-   [Editing Financial Statement Header and Summary Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115720.html)
-   [Editing a Financial Statement Reference Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2118055.html)
-   [Editing a Financial Statement Text Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119004.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
