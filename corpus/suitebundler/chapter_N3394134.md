---
id: "chapter_N3394134"
type: "chapter"
title: "SuiteApp Installation and Update"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update"
parent: "book_N3363377"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html"
anchors: []
sha256: "df8b5cb8c825b8dcb2967ce29db0ae7044e996307d30b17ae03d2bd94cfbe807"
---

If you're the administrator of a NetSuite account or have the SuiteApp Marketplace permission, you can install any public bundle or any bundle that's been shared with your account.

-   When you install a customization bundle, objects included in that bundle are created in the target account.
    
-   When you install a configuration bundle, configuration settings included in the bundle are copied from the source account to the target account, overwriting existing configuration settings. Because the installation of a configuration bundle changes the setup of your account, make sure that you understand the changes that result from installation.
    

Before you can install a bundle, you need to find it in a NetSuite source account. See [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html) for a description of bundle search capabilities. See [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html) for an overview of the installation process. See [Choosing a Bundle to Install](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395426.html) for instructions for finding and installing a bundle in your account.

Tip:

Some SuiteApp bundles are available on the SuiteApp Marketplace. For more information, see [Installing from the SuiteApp Marketplace](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539799323.html) and [SuiteApp Marketplace](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1540487155.html).

The Installed Bundles page shows details about all bundles currently installed in your account, plus an action menu. See [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html).

When a new version is available for a bundle you've installed, you can update it from a link on the Installed Bundles page. When you update a customization bundle, new bundled objects are added to your account, and updates to bundled objects are copied to your account. When you update a configuration bundle, changes to bundled configuration settings are copied to your account. See [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html) for instructions for updating an installed bundle.

When you install a managed bundle, you consent to automatic updates from the solution provider. See [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html).

If you decide you don't want a customization bundle after installing it, you can uninstall it from the Installed Bundles page. You cannot uninstall a configuration bundle. For more information, see [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html).

SuiteBundler provides options during bundle installations and updates for handling any customization bundle objects that conflict with existing target account objects, meaning they have the same names or script IDs. See [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html).

The Bundle Audit Trail page tracks bundle installations, updates, and uninstalls for your account. The Audit Trail subtab on the Bundle Details page tracks these changes for each bundle. See [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html).

Important:

Bundles are also called SuiteApps.

Note:

You can use SuiteScript to get information about installed bundles and SuiteApps. For more information, see [N/suiteAppInfo Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160236086332.html).

### Related Topics

-   [SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N3363377.html)
-   [SuiteBundler Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3363483.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
-   [SuiteBundler Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3783020489.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Custom Transaction Types in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4177814825.html)
-   [Adding a Custom Segment to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4520725557.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
