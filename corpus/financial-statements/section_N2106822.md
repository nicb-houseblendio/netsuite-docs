---
id: "section_N2106822"
type: "section"
title: "Financial Report Builder Edit Columns Page"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Report Builder Interface > Financial Report Builder Edit Columns Page"
parent: "section_N2106055"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106822.html"
anchors: []
sha256: "b758112ebb47d84d4f7227f99e49d4036c5d290a7c20b3ff8e541dfd21008d0e"
---

On the Edit Columns page of the Financial Report Builder, you can make changes to the columns for a custom financial statement.

![Screenshot of the Edit Columns page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBColumnBig.png)

The functions available on this page are similar to those available on the Report Builder Edit Columns page, as described in [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html). Additional capabilities include:

-   [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html)
    
-   [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html)
    
-   [Adding Budget Columns to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109623.html)
    
-   [Adding Persistent Matrix Columns to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109761.html)
    

Avoid selecting values related to time from the View Columns By dropdown list for reports that use the Subsidiary Context of Subsidiary (Consolidated).

Note:

If you remove the original Amount column, you can't drill down on the data in the Amount column that you add later.

Most of your financial statement customizations are likely to be made to rows, and so are done on the [Financial Report Builder Edit Layout Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106362.html).

Column values in financial statement results are rounded to the currency precision. The precision is determined by the format of the company currency, or in NetSuite OneWorld, by the format of the subsidiary base currency. This rounding applies to currency values and non-currency values, including formula column values.

Warning:

For performance reasons, a report can't include more than 30 data columns. If you try to add a 31st column on the Edit Columns page, you'll receive an error. Report results may include more than 30 columns because of persistent matrix columns defined in the View Columns By list. See [Adding Persistent Matrix Columns to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109761.html).

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Report Builder Edit Layout Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2106362.html)
-   [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
