---
id: "section_N3382176"
type: "section"
title: "Bundling NetSuite Financial Statements"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Bundling NetSuite Financial Statements"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html"
anchors: []
sha256: "bf1295ebda7dfc94f9229a713a6f660685d9491c48fdf754dea117daac300359"
---

Financial statements, which include income statements, balance sheets, and cash flow statements, are specialized reports that use layouts to determine their look and feel. A financial statement layout is a set of definitions for report rows, including the rows and financial sections to be displayed, row order and hierarchy, section filter criteria, methods for calculating summary amounts, row labels, and text, line, and background formatting options.

When you include a custom financial statement in a bundle, the custom layout assigned to the report is automatically bundled as well. Both the layout and report are added to target accounts during bundle installation.

You can assign layouts to financial statements, and view layout assignments, at _Reports > Financial > Row Layout Assignment_. Be sure to review these before bundling financial statements. Whenever possible, the assignment of a layout to a bundled financial statement from the source account is preserved in target accounts. If there is ambiguity about this assignment, it is not preserved in target accounts, and users in these accounts can set up the assignments themselves.

For example, in OneWorld accounts, NetSuite provides specialized country-specific layouts for each subsidiary's financial statements, so that each custom layout is associated with a subsidiary as well as with a financial statement. If the source account for a bundled financial statement uses OneWorld, the layout assignment in the source may not be preserved in the target, because the associated subsidiary in the source may not exist in the target.

In cases where the assignment is not preserved, the layout is still added to the target account. After bundle installation, a target account user should review the layout assigned to the bundled financial statement and change this assignment as necessary, at _Reports > Financial > Row Layout Assignment_. For details, see [Financial Reports: Row Layout Assignment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112344.html).

Important:

An update to a bundle that includes a custom financial statement updates the report and the layout objects, but does not update the layout assignment in target accounts. If the assignment has been changed in a target account since the bundle was originally installed, the update does not revert the change.

Note:

SuiteBundler cannot properly match up data for financial statements installed from two different bundles sourced from a sandbox account. To avoid duplicate sections and rows in financial statements, use only one bundle to install them from a sandbox account to a production account.

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [Financial Statements Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html)
-   [Assigning a Layout to a Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112565.html)
-   [Financial Reports: Row Layout Assignment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112344.html)
-   [Subsidiary-Specific Financial Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123802.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
