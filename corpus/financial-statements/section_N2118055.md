---
id: "section_N2118055"
type: "section"
title: "Editing a Financial Statement Reference Row"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Rows > Editing a Financial Statement Reference Row"
parent: "section_N2115374"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2118055.html"
anchors: ["procedure_N2118106", "bridgehead_N2118228", "bridgehead_N2118241", "bridgehead_N2118258", "bridgehead_N2118844"]
sha256: "fe4dbcd7da13bb189f745fc2325278b89c5a4254cbbec3e744897fdeeda1ba72"
---

A reference row can be used in a financial statement to display a value referenced from a section or row in another financial statement. Reference rows are available for Balance Sheet and Cash Flow Statement reports.

For example, the standard Cash Flow Statement uses the following reference rows: Net Income from the Income section of the standard Income Statement, and Cash at Beginning of Period from the Bank Accounts section of the standard Cash Statement.

The following screenshot illustrates the editing of a reference row in the Financial Report Builder:

![Screenshot showing the Reference Row fields on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBReferenceEdit.png)

#### To edit a reference row: {#procedure_N2118106}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, do one of the following:
    
    -   Select the row below the place where you want to add a new reference row, and from the **Add Row/Section** list, select **Add Reference Row**.
        
    -   Select an existing reference row.
        
3.  Complete any of the following tasks:
    
    -   [Editing a Reference Row Header Label](#bridgehead_N2118228)
        
    -   [Modifying Reference Row Hierarchy](#bridgehead_N2118241)
        
    -   [Defining the Financial Statement Row to be Referenced](#bridgehead_N2118258)
        
    -   [Modifying Reference Row Format Options](#bridgehead_N2118844)
        

## Editing a Reference Row Header Label {#bridgehead_N2118228}

You can edit the Header Label for a reference row (the row's text) and choose whether to display the row. To hide this row, clear the **Display Row** box.

## Modifying Reference Row Hierarchy {#bridgehead_N2118241}

You can change a reference row's placement in the report hierarchy by selecting a different row in the Child Of dropdown. The reference row is moved under the row you select here and is reflected in the Layout outline at left.

Alternatively, you can drag and drop a reference row in the Layout outline to change its hierarchy.

## Defining the Financial Statement Row to be Referenced {#bridgehead_N2118258}

You can select the financial statement (Report), the financial section or row (Row), and the date range (Relative Range) to be referenced for a reference row value.

![Screenshot of Reference Row fields on the Edit Layout page of the Financial Report Builder with the Report, Row, and Relative Range date fields outlined in red](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBReferenceRelRange.png)

The referenced date range is defined relative to the date range for the current financial statement. When the current financial statement's date range is changed, the date range for the referenced value is adjusted accordingly.

The referenced date range is set by selections from two dropdown lists for the start and end of the range. Be aware of how the values in these two dropdown lists can be used as shown in the following table.

| Relative Date Ranges for Financial Statement Reference Rows |
| --- |
| Start | End | End of Range Definition | Example Usage |
| --- | --- | --- | --- |
| Balance Forward | Beginning of Year | 
(Exclusive)

Ends on day before Beginning of Year



 | Balance Sheet, Retained Earnings Net Income row; referencing Income Statement, Income section |
| Balance Forward | Start Date | 

(Exclusive)

Ends on day before Start Date



 | Cash Flow Statement, Cash at Beginning of Period row; referencing Cash Statement, Bank Accounts section |
| Balance Forward | End Date | 

(Inclusive)

Ends on End Date



 | Balance Sheet, Net Income row; referencing Income Statement, Income section |
| Beginning of Year | Start Date | \- | Note: This combination shouldn't be used. |
| Beginning of Year | End Date | 

(Inclusive)

Ends on End Date



 |
| Start Date | End Date | 

(Inclusive)

Ends on End Date



 | Cash Flow Statement, Net Income row; referencing Income Statement, Income section |

## Modifying Reference Row Format Options {#bridgehead_N2118844}

You can modify the formatting of text, lines, and background color for a reference row. You can also indicate whether to show currency symbols, reverse signs, or include text, such as USD, before or after the reference row amount.

![Screenshot showing format options for reference rows on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBReferenceFormat.png)

Note:

Checking the **Reverse Sign** box for a row affects all dynamic total calculations that include that row's value.

For more information, see [Setting Financial Statement Formatting Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119303.html).

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Statement Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115374.html)
-   [Editing Financial Statement Header and Summary Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115720.html)
-   [Editing a Financial Statement Formula Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2117576.html)
-   [Editing a Financial Statement Text Row](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2119004.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
