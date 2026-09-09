---
id: "section_N2115720"
type: "section"
title: "Editing Financial Statement Header and Summary Rows"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Rows > Editing Financial Statement Header and Summary Rows"
parent: "section_N2115374"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115720.html"
anchors: ["procedure_N2115762", "bridgehead_N2115900", "bridgehead_N2115946", "bridgehead_N2115962", "bridgehead_N2116058", "procedure_N2116098", "bridgehead_N2116175"]
sha256: "9c968930d348c91c3d628517e2b3acfa2e774efa7bfdd3f1ccf0259ca4ced788"
---

In NetSuite financial statements, header rows and their linked summary rows are used to aggregate related rows of data. The header row appears above its set of child rows and usually contains descriptive text. The summary row appears below the set of rows and summarizes the row amounts. This summary can be a dynamic total that adds all row amounts or a calculation based on a more complex formula.

The following screenshot points out header rows and their linked summary rows. These header rows differ from section header rows in that they don't include their own account rows, but instead group data from other rows.

![Screenshot of a Balance Sheet with numbered callouts indicating header and summary rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBHeaderRowOverview.png)

| 1 | Header row: Assets |
| --- | --- |
| 2 | Summary row: Assets |
| 3 | Header row: Current Assets |
| 4 | Summary row: Current Assets |
| 5 | Header row: Liabilities & Equity |
| 6 | Summary row: Liabilities & Equity |

#### To edit header and summary rows: {#procedure_N2115762}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, do one of the following:
    
    -   Select the row below the place where you want to add a new header row, and from the **Add Row/Section** list, select **Add Header and Summary Rows**.
        
    -   Select an existing header row or linked summary row that you want to edit. (Notice that whenever you select a header or summary row, its linked row is also selected, and you can edit properties for both rows.)
        
3.  Complete any of the following tasks:
    
    -   [Editing Header and Summary Labels](#bridgehead_N2115900)
        
    -   [Modifying Header Row Hierarchy](#bridgehead_N2115946)
        
    -   [Modifying Header Row Expansion](#bridgehead_N2115962)
        
    -   [Setting Summary Calculation Method](#bridgehead_N2116058)
        
    -   [Modifying Header and Summary Row Format Options](#bridgehead_N2116175)
        

## Editing Header and Summary Labels {#bridgehead_N2115900}

You can:

-   Edit the **Header Label**. This is the header row's text.
    
-   Choose whether to display the header row. To hide this row, clear the **Display Row** box.
    
-   Edit the **Summary Label**. This is the summary row's text. If this field is left blank, the default label **Summary - <Header Label>** is displayed.
    
-   Choose whether to display the Summary row. To hide this row, clear the **Display Row** box.
    

## Modifying Header Row Hierarchy {#bridgehead_N2115946}

You can change a header row's placement in the report hierarchy by selecting a different row in the Child Of dropdown. The header row is moved under the row you select here. This move is reflected in the Layout outline.

Alternatively, you can drag and drop a header row in the Layout outline to change its hierarchy.

## Modifying Header Row Expansion {#bridgehead_N2115962}

You can indicate the expansion of data rows under a header row by selecting from the Display dropdown:

-   **Expanded** - data rows are displayed in expanded format. Viewers can collapse the header row to hide other rows. This is the default.
    
    ![Screenshot showing that a minus sign before a section in a financial statement indicates that the section is expanded](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBHeaderRowExpand.png)
-   **Collapsed** - the header row is displayed in collapsed format. Viewers can expand it.
    
    ![Screenshot showing that a plus sign indicates a collapsed section in a financial statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBHeaderRowCollapse.png)
-   **Cannot Expand** - the header row is displayed in collapsed format. Viewers can't expand it. In this case, the summary amount is displayed and the details that make up the summary can't be seen.
    
    ![Screenshot showing that a section in a financial statement cannot be expanded or collapsed unless it has a plus or minus sign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionCannotExpand.png)

## Setting Summary Calculation Method {#bridgehead_N2116058}

By default, a summary row displays a sum of amounts for the group of rows under its linked header. This sum is dynamic. This means it changes when any of the row amounts change. The Financial Report Builder also enables you to define a formula to calculate the summary.

![Screenshot showing the formula builder row for summary rows on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBHeaderDynamicTotal.png)

Note:

Enabling the **Reverse Sign** option for a row affects all dynamic total calculations that include that row's value.

#### To define a formula to calculate a summary row: {#procedure_N2116098}

1.  When a header and summary rows combination is selected in the Layout outline, choose the **Apply a Formula** option.
    
2.  Use the formula builder to enter an expression. Add each value on a separate line.
    
    1.  Select an operator if needed. Addition (+), subtraction (-), multiplication (\*), division (/), and percentage (%) operators are available.
        
    2.  Select opening parentheses if needed.
        
    3.  Indicate whether the type of value is a constant number (**Constant**) or a value from another row in the report (**Row**).
        
    4.  Enter the value, which is a field or a dropdown depending on the value type you select.
        
    5.  Select closing parentheses if needed.
        
    6.  Repeat until the formula expression is complete.
        
    7.  Review the expression displayed at the top of the formula builder for correctness, then make adjustments as necessary.
        

## Modifying Header and Summary Row Format Options {#bridgehead_N2116175}

You can modify the formatting of text, lines, and background color for header and summary rows. You can also indicate whether to show currency symbols, reverse signs, or include text, such as USD, before or after the summary row amount.

![Screenshot showing format options for header and summary rows on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBHeaderRowFormat.png)

Note:

Enabling the **Reverse Sign** option for a row affects all dynamic total calculations that include that row's value.

For more information, see [Setting Financial Statement Formatting Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119303.html).

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Statement Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115374.html)
-   [Editing a Financial Statement Formula Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2117576.html)
-   [Editing a Financial Statement Reference Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2118055.html)
-   [Editing a Financial Statement Text Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119004.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
