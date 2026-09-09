---
id: "bridgehead_N2842249"
type: "bridgehead"
title: "Bundling Fields with Access Restrictions"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Restricting Access to Custom Fields > Bundling Fields with Access Restrictions"
parent: "section_N2841053"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2842249.html"
anchors: []
sha256: "7ffb40134585f143333133fbec97f7002e2af222474b518525cd40d2cd2991d3"
---

Note:

SuiteBundler is still supported, but it won't be updated with any new features.

To take advantage of new features for packaging and distributing customizations, you can use the Copy to Account and SuiteCloud Development (SDF) features instead of SuiteBundler.

Copy to Account is an administrator tool that lets you copy custom objects between your accounts. The tool can copy one custom object at a time, including dependencies and data. For more information, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

SuiteCloud Development Framework is a development framework that lets you create SuiteApps from an integrated development environment (IDE) on your local computer. For more information, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).

If you include a custom field in a bundle that has access restrictions, custom roles that have access aren't automatically included in the bundle. If, however, you include those custom roles in the same bundle, the access restrictions are preserved.

The access level assigned to standard roles is preserved when you bundle a custom field that has access restrictions.

Custom field restrictions based on subsidiary or departments aren't carried over into the target account because departments and subsidiaries can't be included in a bundle.

### Related Topics

-   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
-   [Setting Role, Department, or Subsidiary Access Restrictions for a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1106091633.html)
-   [Access Level History for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2842230.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
