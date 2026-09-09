---
id: "section_N2113041"
type: "section"
title: "Creating a Custom Financial Statement Section"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Sections > Creating a Custom Financial Statement Section"
parent: "section_N2112804"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html"
anchors: ["bridgehead_N2113099", "procedure_N2113107", "bridgehead_N2113321", "procedure_N2113330"]
sha256: "132e0ffb8206f9ebc02c774c2a94a42c77d04cdd44f43b23f5c8af7a5389ca2a"
---

On the Financial Report Builder's Edit Layout page, you can create a custom section by adding a new section with new selection criteria. You can also edit selection criteria for an existing section, which causes a duplicate section to be created. Selection criteria define the accounts to be included in a financial statement section.

Be aware of the following limitations for custom sections:

-   To avoid unexpected results, don't define overlapping criteria for two or more custom sections in a financial statement. If an account fits the criteria for more than one section, the system determines the account's section, which may not be the one you expect.
    
-   If you create a custom Cash Flow Statement that includes custom sections, its Cash at Beginning of Period row value is likely to be incorrect. To ensure accuracy, create a custom Cash Statement that shares these custom sections and make it the referenced report for that row. See [Customizing Cash Flow Statement Account Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103948.html).
    
-   Section filtering doesn't result in a duplicate combination of account, department, location, class, or subsidiary filtered values on multiple lines. This is because a financial statement can't display values for an identical account multiple times. To avoid incorrect totals, the statement displays correct values the first time the account is listed and displays zeroes for later listings of the same account. For example, this issue may occur when accounts are filtered by a department that is a parent of one or more other departments.
    

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

## Editing Selection Criteria for an Existing Section {#bridgehead_N2113099}

#### To edit selection criteria for an existing section: {#procedure_N2113107}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  Select a financial section in the Layout outline.
    
    ![Screenshot of the Layout Add Row/Section list of the Edit Layout page in the Financial Report Builder with the Bank section selected](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionSelect.png)
3.  In the right pane of the Financial Report Builder on the Section subtab, click **Edit Criteria**.
    
    ![Screenshot of the right pane of the Edit Layout page in the Financial Report Builder with the Edit Criteria button outlined in red](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionEditCriteria.png)
4.  In the Edit Section Criteria popup, click **OK** to indicate that you're creating a new custom section.
    
5.  You can insert and remove filters.
    
    -   To add a filter, select a field from the list in the **Filter** column.
        
    -   In the Filter popup that opens immediately after you select a filter, select one or more values to indicate the criteria to be applied to this section. You also can click **Set Options** to open this popup.
        
    -   If you want to use parenthetical expressions to define section data filters, check the **Use Expressions** box. This option functions here in the same manner as it does for search criteria. For more information, see [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html).
        
6.  If you want this custom section to be available for use in other custom financial layouts, click **Share Section**.
    
    -   In the Share Section popup, click **OK**.
        
    -   Change the section name/ID as desired.
        
7.  Make other changes to the section as desired. See [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html).
    

## Adding a New Custom Section {#bridgehead_N2113321}

#### To add a new custom section to a custom financial statement: {#procedure_N2113330}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, select the row where you want to insert the new section. The section is added above the selected row. (Note that you also can use the up arrow and down arrow buttons or drag and drop the section to move it after it's added.)
    
3.  From the **Add Row/Section...** list, select **Add Financial Section**.
    
4.  In the New Section Row popup, choose the **Create New Section** option, and click **OK**.
    
5.  You can insert and remove filters.
    
    -   To add a filter, select a field from the list in the **Filter** column.
        
    -   In the Filter popup that opens immediately after you select a filter, select one or more values to indicate the data that will be included in this section. You can also click **Set Options** to open this popup.
        
    -   If you want to use parenthetical expressions to define section data filters, check the **Use Expressions** box. This option functions here in the same manner as it does for search criteria. For more information, see [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html).
        
6.  If you want this custom section to be available for use in other custom financial statements, click **Share Section**.
    
    -   In the Share Section popup, click **OK**.
        
    -   Change the section name/ID as desired.
        
7.  Make other changes to the section as desired. See [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html).
    

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Statement Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Adding a Section to a Custom Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2114746.html)
-   [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
