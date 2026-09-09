---
id: "section_N668091"
type: "section"
title: "Entering Formulas for a Mass Update"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Mass Updates > Entering Formulas for a Mass Update"
parent: "article_1103335211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668091.html"
anchors: []
sha256: "09e381d5bd3f5bdae16428f00f00b7d84b561161b5dc2418af4447c2f7ee551e"
---

For mass updates that are General updates, you can update multiple fields per record. You select the fields to be updated on the Mass Update Fields subtab of the mass update page, by checking the Apply box. For each selected field, you can enter a static value to use for updating the field in all records, in the Value field. Or, if you want to update a field based on dynamic values, you can enter a SQL expression in the Formula field. You can enter SQL directly in the Formula field, or click the Set Formula button to display a popup formula builder.

Formula values are dynamically calculated at the time a mass update is performed. Formulas can include NetSuite field IDs for which field values are substituted, SQL functions, and mathematical operators. NetSuite field IDs should be formatted as follows: {field\_name}. Most common SQL functions and operators are available.

The following are example mass update formulas:

-   To increase customer credit limits by 25%, do a Customer general update, check the Apply box for Credit Limit, and enter this formula: {creditlimit} \* 1.25.
    
    ![Credit Limit box selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/creditlimit1.png)
-   To set inventory items' preferred stock level to twice the reorder point, do an Inventory Item general update, check the Apply box for Preferred Stock Level, and enter this formula: {reorderpoint} \* 2.
    
    ![Preferred Stock Level box selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/MassUpdateForm2.png)

Note:

Knowledge of SQL will help you to fully leverage the flexibility and power of SQL functions to define complex formulas. For more details, refer to [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html) . Also, you can refer to [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html) for tables of NetSuite field IDs.

### Related Topics

-   [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html)
-   [Defining a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N667342.html)
-   [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html)
-   [Translations for Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668849.html)
-   [Example Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N669099.html)
-   [Available Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N669340.html)
-   [Mass Updates of Global Subscription Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N672926.html)
-   [Performing Mass Deletes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4098351672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
