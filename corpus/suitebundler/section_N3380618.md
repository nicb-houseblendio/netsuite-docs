---
id: "section_N3380618"
type: "section"
title: "Hiding Bundle Components in Target Accounts"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Hiding Bundle Components in Target Accounts"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html"
anchors: []
sha256: "89a3b752bc3618dd2cacd335bad63327143e000d91881f9f2e58a4334c43b1b0"
---

By default, list pages for bundleable objects include objects that have been installed by bundles. You can identify bundle objects by the bundle ID in the From Bundle column on list pages. See [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html).

In some cases, you may prefer that objects installed by your bundle are not visible in target account list pages.

To enable an option not to display bundle objects in target account list pages, check the Hide Components box on the Bundle Basics page of the Bundle Builder:

![Bundle Builder page with Hide Components box highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleHideComponents.png)

Checking this box hides the bundle's components from target account list pages by default. Also, the bundle is not listed in the From Bundle filter on list pages. See [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html). Note that this option cannot be enabled for a configuration bundle.

After bundle installation in a target account, an administrator can change this hide or show setting. This change can be made by selecting the Hide Components or Show Components option button on the Components subtab of the Bundle Details page.

![Components subtab with Display Options highlighted and Show Components option selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundDetailsHideShow.png)

Important:

The target account selection of the Hide Components or Show Components display option for a bundle is not overwritten by the Bundle Builder setting during bundle updates. The Bundle Builder Hide Components option is applied only during bundle installation.

Warning:

If Hide Components is enabled for a bundle created in a production account, refreshes to Release Preview and sandbox accounts cause that bundle's components to be hidden in the Release Preview and sandbox accounts.

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 1 Bundle Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
