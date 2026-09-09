---
id: "section_N1508163"
type: "section"
title: "CSV Import for Subsidiary Budgets"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Subsidiary Budgets in OneWorld > CSV Import for Subsidiary Budgets"
parent: "section_N1506361"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508163.html"
anchors: []
sha256: "76c6156f938c99a59eea13a22b12001bef1187eedc4f943b074698ceff3cf7e8"
---

You can use a Comma Separated Values (CSV) file to import budget amounts for NetSuite OneWorld subsidiary budgets. For example, many companies develop budgets using a spreadsheet application, which can save budget data in a CSV file.

For the specific steps to import budget data in a CSV file, see [Importing a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505717.html).

Important:

When you use the NetSuite Budget template to create the CSV file, enter budget amounts consistent with the budget category type and Subsidiary values. The Category column determines whether NetSuite stores budget amounts using the global (root parent's base currency) or local (subsidiary's base currency) currency. The Subsidiary column determines the subsidiary's base currency.

![Screenshot of a portion of the NetSuite Budget CSV file with Category and Subsidiary columns outlined in red](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/ImportSubBudget.png)

For example, your root parent subsidiary uses British pounds and your company has a subsidiary in Canada. Your CSV file has **local** in the Category column and **Canada** in the subsidiary column. If you enter 10,000 in the Amount column, the amount is stored as 10,000 Canadian dollars. However, if the file had **global** in the Category column and **Canada** as the subsidiary, the 10,000 would be stored as British pounds.

### Related Topics

-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Subsidiary Budgeting Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506662.html)
-   [Creating Budget Categories for Local Subsidiary Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html)
-   [Setting Up a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507295.html)
-   [Guidelines for Copying a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507638.html)
-   [Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
