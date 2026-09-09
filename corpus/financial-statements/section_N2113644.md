---
id: "section_N2113644"
type: "section"
title: "Editing a Financial Statement Section"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Sections > Editing a Financial Statement Section"
parent: "section_N2112804"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html"
anchors: ["procedure_N2113683", "bridgehead_N2114140", "bridgehead_N2114220", "bridgehead_N2114256", "bridgehead_N2114352", "bridgehead_N2114437", "bridgehead_N2114597"]
sha256: "c297f777d8d5af90cab18f0190b2d44ee9cf261b191bcc7511b960a479f0e4ae"
---

On the [Financial Report Builder Edit Layout Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106362.html) you can perform other edits to financial sections, in addition to defining selection criteria that determine the accounts to be included.

When you edit selection criteria for a section, you're creating a new section. See [Creating a Custom Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html).

#### To edit a section: {#procedure_N2113683}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, select the section that you want to edit.
    
3.  Complete any of the following tasks:
    
    -   [Editing Financial Section Labels](#bridgehead_N2114140)
        
    -   [Modifying Financial Section Hierarchy](#bridgehead_N2114220)
        
    -   [Modifying Financial Section Row Expansion](#bridgehead_N2114256)
        
    -   [Modifying Financial Section Grouping](#bridgehead_N2114352)
        
    -   [Modifying Financial Section Sort Order](#bridgehead_N2114437)
        
    -   [Modifying Financial Section Format Options](#bridgehead_N2114597)
        

Note:

If you want to use a section to calculate % of Expense or % of Income column values for a custom income statement, set its **Marker** field to **Expense** or **Income**. See [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html) or [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html).

## Editing Financial Section Labels {#bridgehead_N2114140}

You can:

-   Edit the section's Header Label. This is the text in the section's header row.
    
-   Choose whether to display the Header row. To hide this row, clear the **Display Row** box.
    
-   Edit the section's Total Label. This is the text in the section's total row that lists the total amount for the section. If this field is left blank, the default label
    
    Total - <Header Label> is displayed.
    
-   Choose whether to display the total row. To hide this row, clear the **Display Row** box.
    
    ![Screenshot of the Header Label and Total Label fields for the Income account section on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionEditGenLabels.png)

## Modifying Financial Section Hierarchy {#bridgehead_N2114220}

You can change a financial section's placement in the report hierarchy by selecting a different row in the Child Of list. The section is moved under the row you select here, as reflected in the Layout outline.

![Screenshot of the field that controls section hierarchy, the Child Of list, for the Income account section on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionEditChild.png)

Alternatively, you can drag and drop a financial section in the Layout outline to change its hierarchy.

## Modifying Financial Section Row Expansion {#bridgehead_N2114256}

You can indicate the expansion of financial section data, by selecting from the Display list:

-   **Expanded** - the section is displayed in expanded format, showing all rows. Viewers can collapse it. This is the default.
    
    ![Screenshot showing that a minus sign before a section in a financial statement indicates that the section is expanded](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionExpanded.png)
-   **Collapsed** - the section is displayed in collapsed format, showing a header row with a summary amount. Viewers can expand it.
    
    ![Screenshot showing that a plus sign indicates a collapsed section in a financial statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionCollapsed.png)
-   **Cannot Expand** - the section is displayed in collapsed format. Viewers can't expand it.
    
    ![Screenshot showing that a section in a financial statement cannot be expanded or collapsed unless it has a plus or minus sign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionCannotExpand.png)

## Modifying Financial Section Grouping {#bridgehead_N2114352}

By default, financial section data are grouped by accounts.

-   You can select from the Group By dropdown list to change this primary grouping to be by class, department, location, customer/project, item, or if you're using NetSuite OneWorld, subsidiary.
    
-   You also can set an optional, secondary grouping in the Then By dropdown list to be by accounts, class, department, location, customer/project, item, or subsidiary.
    

The Show Hierarchy check boxes next to the Group By and Then By dropdown lists indicate whether full hierarchical names are used for group labels and sort order. Full hierarchical names are in the format of grandparent : parent : child. Non-hierarchical, or flat, names include only the child. By default, these boxes are checked and full hierarchical names are used.

Be aware of how grouping interacts with filtering to select accounts for a section. Your custom financial statement doesn't include multiple lines with a duplicate combination of account, department, location, class, customer/project, item, or subsidiary filtered values. This is because a financial statement can't display values for an identical account multiple times. To avoid incorrect totals, the statement displays correct values the first time the account is listed and displays zeroes for later listings of the same account.

## Modifying Financial Section Sort Order {#bridgehead_N2114437}

Within each grouping of financial section data, you can define the sort order of account rows on the Order subtab. Note that if you've defined a secondary grouping, two Order subtabs are provided.

![Screenshot showing Group By field and Account Order subtab on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionOrder.png)

For grouping by accounts, available sort orders include:

-   Account Name Ascending
    
-   Account Name Descending
    
-   Account Number Ascending
    
-   Account Number Descending
    
-   Custom
    

For grouping by class, department, location, item, or subsidiary, available sort orders include:

-   Ascending
    
-   Descending
    
-   Custom
    

For grouping by customer/project, available sort orders include:

-   Customer/Project Name Ascending
    
-   Customer/Project Name Descending
    
-   Customer/Project Number Ascending
    
-   Customer/Project Number Descending
    
-   Custom
    

The Custom sort order enables you to manually set the order of data rows. For example, you could set the order so that all new accounts display at the end of the section.

Note:

If a list used for grouping includes more than 200 records, the list is truncated and custom sort order isn't supported. This scenario is most likely to occur when grouping by item or customer/project.

## Modifying Financial Section Format Options {#bridgehead_N2114597}

You can modify the formatting of text, lines, and background color for section rows, including the header row that displays a description of the section, account rows that display data amounts, and the total row that displays the total amount for the section. Note that the same format options are applied to all account rows in a section. You also can indicate whether to show currency symbols, reverse signs, or include text, such as USD, before or after amounts for the account rows and total row.

You can't change whether account numbers are displayed. Account names include account numbers when the accounting preference Use Account Numbers is checked.

You can make these edits on the Format subtab.

![Screenshot showing the Format subtab of the Edit Layout page, and its fields, for the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionFormat.png)

Note:

Checking the **Reverse Sign** box for a row affects all dynamic total calculations that include that row's value. Always run the report and review the accuracy of all total rows if you use this option.

For more information, see [Setting Financial Statement Formatting Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119303.html).

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Statement Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html)
-   [Creating a Custom Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html)
-   [Adding a Section to a Custom Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2114746.html)
-   [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
