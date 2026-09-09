---
id: "section_N2112804"
type: "section"
title: "Financial Statement Sections"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Sections"
parent: "chapter_N2105415"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html"
anchors: []
sha256: "719c36e1568a895151dbf76c38b280cb1dfee04b9f7f3a87b246fcf19ad7d7db"
---

A financial section is a subset of financial data in a financial statement. Each financial section has a header row with its description, account rows showing data amounts, and a total row showing the section's total amount.

The following screenshot shows rows in the Bank section of a standard Balance Sheet:

![Screenshot showing a standard Balance Sheet with the rows expanded](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionOverview.png)

| 1 | Header Row |
| --- | --- |
| 2 | Account Rows |
| 3 | Total Row |

Note that if you collapse a section, only its header row displays with header text and the amount from the total row. Bank, Other Current Asset, and Fixed Assets are collapsed in the following example:

![Screenshot showing the Assets section of a standard Balance Sheet with the rows collapsed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionCollapsed.png)

If a section isn't preceded by the plus sign or minus sign, it can't be collapsed or expanded.

The following screenshot illustrates the editing of the Bank section in the Financial Report Builder:

![Screenshot showing the Bank section in edit mode on the Edit Layout page of the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionMedium.png)

For standard financial statements, each financial section corresponds to an account type, and section data rows are grouped and sorted by account number. The criteria used for section data are dynamic so that when a financial statement is run, each section includes data for all accounts of the selected type. This method of defining section criteria is preferable to using static lists of accounts. Dynamic criteria ensure that all necessary accounts are included in a financial section and are particularly useful for including newly created accounts.

When you create custom financial statements, you can define custom sections that are based on criteria other than account type. These criteria may include account name, account number, class, department, location, and subsidiary. See [Creating a Custom Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html).

You can make many other changes to sections in custom financial statements including changing their grouping, sorting, hierarchy, expansion, labels, and format options. See [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html).

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have the necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

The Financial Report Builder also enables you to add new sections to a custom financial statement. See [Adding a Section to a Custom Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2114746.html).

If you use NetSuite OneWorld, you can filter and group section data by subsidiary. See [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html).

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Statement Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2110511.html)
-   [Financial Statement Rows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115374.html)
-   [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html)
-   [Available Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092953.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
