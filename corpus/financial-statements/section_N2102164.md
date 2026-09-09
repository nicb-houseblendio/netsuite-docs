---
id: "section_N2102164"
type: "section"
title: "Multi-Column Balance Sheets"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Balance Sheets > Multi-Column Balance Sheets"
parent: "section_N2098170"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2102164.html"
anchors: []
sha256: "95224388b110886e7554066f919afdcdd8384c41d23989ec88157f774c3c7eaf"
---

A multi-column balance sheet lets you compare account balances for the selected reporting period with account balances for previous reporting periods. It also lets you include columns for the sum of all debits and credits posted to each account within a selected reporting period. NetSuite lets you customize the standard balance sheet report to produce a multi-column balance sheet.

Customization options for the Balance Sheet Report enable you to comply with different international legal requirements by adding columns to the report using the Financial Report Builder. For example, in addition to the account balances for the selected reporting period shown in the standard report, you can display columns for the previous period balance. You can also display columns for the total debits and the total credits. The same options are available for the Trial Balance Report using the Report Builder.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

#### To create a multi-column balance sheet report:

1.  Go to _Reports > Financial > Balance Sheet_, and wait for the standard report to load.
    
2.  Click **Customize** to open the Financial Report Builder.
    
3.  In the **Name** field, enter a new name for the report, such as **Multi-Column Balance Sheet**.
    
4.  Click **Edit Columns**. For more information, see [Financial Report Builder Edit Columns Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106822.html).
    
    The Report Preview displays the single **Amount** column from the standard report. This column is automatically selected.
    
5.  Change the **Column Label** from **Amount** to **Closing Balance**.
    
    Don't remove the original Amount column.
    
6.  Add a column for the opening balance as follows:
    
    1.  In the Add Fields area, open the **Financial** folder and select **Amount**.
        
    2.  Move the new column to the left of the Closing Balance column, and change the **Column Label** from **Amount** to **Opening Balance**.
        
    3.  In the **Alternate Period Range Type** list, select **Relative to report date**. Additional options appear below the list.
        
    4.  Check the **Cumulative Value** box.
        
    5.  In the **Alternate Period Range** list, select **Last Period**.
        
7.  Add a column for the total debits as follows:
    
    1.  In the Add Fields area, open the **Financial** folder and select **Amount (Debit)**.
        
    2.  Move the new column to the left of the Closing Balance column, and change the **Column Label** if desired.
        
    3.  In the **Alternate Period Range Type** list, select **Relative to report date**. Additional options appear below the list.
        
    4.  Clear the **Cumulative Value** box.
        
    5.  In the **Alternate Period Range** list, select **This Period**.
        
8.  Add a column for the total credits as follows:
    
    1.  In the Add Fields area, open the **Financial** folder and select **Amount (Credit)**. This adds a new column to the right of the Closing Balance column.
        
    2.  Move the new column to the left of the Closing Balance column, and change the **Column Label** if desired.
        
    3.  In the **Alternate Period Range Type** list, select **Relative to report date**. Additional options appear below the list.
        
    4.  Clear the **Cumulative Value** box.
        
    5.  In the **Alternate Period Range** list, select **This Period**.
        
9.  Click **Save**.
    

### Related Reports

-   [Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2098310.html)
-   [Balance Sheet Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2100658.html)
-   [Comparative Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2101379.html)
-   [Multi-Book Balance Sheet Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495037141.html)
-   [Multi-Book Balance Sheet Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495119693.html)

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Available Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092953.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
