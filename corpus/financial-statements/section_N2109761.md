---
id: "section_N2109761"
type: "section"
title: "Adding Persistent Matrix Columns to Financial Statements"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Report Builder Interface > Financial Report Builder Edit Columns Page > Adding Persistent Matrix Columns to Financial Statements"
parent: "section_N2106822"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109761.html"
anchors: []
sha256: "7f730adc9257f91b6b44eca5b3d9befbdccbf1ad65a0c63a6809354d48f6be9b"
---

For reports other than financial statements, the only method for adding matrix columns to reports is to select from the Column list in the report footer. For details, see [Adding Matrix Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N741181.html). Matrix columns added through this method apply only to the current report, so you need to repeat the selection each time you run the report.

On the Financial Report Builder Edit Columns page, the View Columns By list lets you select a dimension to use for matrix columns that persist whenever a custom financial statement is run. Total is the default dimension.

![Screenshot of the Edit Columns page of the Financial Report Builder showing the View Columns By list with the Location dimension selected](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBColumnMatrix.png)

The data for the selected dimension can be displayed in separate columns for each dimension value or in a hierarchically with child values grouped under parent values within the same columns. To display data hierarchically, select a (Hierarchy) option in the View Columns By list. In NetSuite OneWorld, avoid selecting values related to time from the View Columns By list for reports that use the Subsidiary Context of Subsidiary (Consolidated).

![Screenshot of the Edit Columns page of the Financial Report Builder showing the View Columns By list with the Total dimension selected and hierarchy options for other dimensions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBViewColumnsHierarchy.png)

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. For more information, see [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html).

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Report Builder Edit Columns Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106822.html)
-   [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
