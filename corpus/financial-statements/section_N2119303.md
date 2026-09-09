---
id: "section_N2119303"
type: "section"
title: "Setting Financial Statement Formatting Options"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Setting Financial Statement Formatting Options"
parent: "chapter_N2105415"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119303.html"
anchors: ["procedure_N2119508", "bridgehead_4362642447"]
sha256: "d8c37fb744f01950276f5a058e7696995f3abebc43b0ccd132aa8c6d7c1685df"
---

The Financial Report Builder enables you to set row-level formatting options to give you fine-tuned control over the look of your custom financial statements.

Note:

Other formatting options are available in the [Financial Report Builder More Options Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2110228.html). These are report-level, not row-level.

You can set the following format options for all types of rows:

-   Font options, for row text and numerics
    
    -   Font size
        
    -   Bold
        
    -   Italic
        
    -   Color
        
    
    Note:
    
    To change the font for a row, you must enable the option in your personal preferences. For details, see [Changing the Font for a Report Row](#bridgehead_4362642447).
    
-   Line options, for row borders
    
    -   Line placement (above row, below row, above & below row)
        
    -   Line type (solid, dashed, dotted, double)
        
    -   Line size
        
    -   Line color
        
-   Row color options, for row backgrounds
    

You can set the following additional format options for rows that display amounts, including section account rows, summary rows, and reference rows:

-   **Show Currency** - Check to display a currency symbol with row amounts. This preference is also available at the report-level on the More Options page. The row-level preference overrides the report-level preference.
    
-   **Reverse Sign** - Check to change positive row amounts to negative, and negative row amounts to positive. Use this option when the database positive or negative value differs from what is expected for financial reports. When you select this option for a row, it affects all dynamic total calculations that include that row's value. After you select this option, be sure to run the report and review the accuracy of all total rows.
    
-   **Prefix** - Enter text to display immediately before each row amount.
    
-   **Suffix** - Enter text to display immediately after each row amount, such as USD.
    

You can't change whether account numbers are displayed. Account names include account numbers when the accounting preference Use Account Numbers is checked.

#### To set row-level format options: {#procedure_N2119508}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, select the row for which you want to set format options.
    
3.  Make changes in the Format box in the right pane.
    
    ![Screenshot showing format options for summary rows on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBFormatOptions.png)

## Changing the Font for a Report Row {#bridgehead_4362642447}

By default, all reports are displayed using the Open Sans font. To change the font for a report row, you must enable the related personal preference.

1.  Go to _Home > Set Preferences_.
    
2.  On the **Analytics** subtab, select **Customize Font on Financial Reports**, and click **Save**.
    

This setting changes the default font on your financial reports to Arial and enables you to change to a different font in the Financial Report Builder.

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Statement Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115374.html)
-   [Editing Financial Statement Header and Summary Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115720.html)
-   [Editing a Financial Statement Formula Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2117576.html)
-   [Editing a Financial Statement Reference Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2118055.html)
-   [Editing a Financial Statement Text Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119004.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
