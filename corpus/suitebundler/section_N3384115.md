---
id: "section_N3384115"
type: "section"
title: "Phased Upgrade of Managed Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Managed Bundles Overview > Upgrading Your Managed Bundle Install Base > Phased Upgrade of Managed Bundles"
parent: "section_N3383724"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html"
anchors: []
sha256: "535325f4fda92d1a0d47da64fe646870fa907bad21e46ddf056cf8af936265aa"
---

SuiteBundler supports a phased release process for managed bundle upgrades, similar to the release process for NetSuite upgrades. You can release a new managed bundle version to subsets of the install base, in phases, instead of having to upgrade the entire install base at the same time. You can maintain multiple versions of a managed bundle, because you can continue to push maintenance updates to accounts still using the older version of the bundle, during the time that other accounts are being upgraded to the new version.

Note:

You should not attempt to maintain more than two released versions of a managed bundle at any one time.

You can copy both a managed or a non-managed bundle to begin work on a new version, then deprecate the original bundle. However, the consequences of deprecating a managed bundle are different from deprecating a non-managed bundle.

-   Deprecating a non-managed bundle prevents editing and installation in target accounts. Also, any accounts that upgrade a non-managed deprecated bundle automatically received the new version.
    
-   When you deprecate a managed bundle, you can continue to edit it to fix issues, and you can continue to install it and push upgrades to it in target accounts.
    

Warning:

You should not remove a bundle from the copy chain while the older version of the bundle is installed by some users and that version is deprecated by a newer version of the bundle. Removing a bundle from the copy chain prevents users from installing the latest version. To understand the chaining of bundle copies, see [Ancestry of Copied Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html#bridgehead_N3386926).

The following screenshots of the Bundle Availability page illustrate the differences in deprecation behavior for managed and non-managed bundles.

-   For a non-managed bundle:
    
    ![Deprecate bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleDeprecateNonManaged.png)
-   For a managed bundle:
    
    ![Deprecate bundle for managed bundle.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleDeprecateManaged.png)

Deprecated managed bundles have the Edit, Push, and Upgrade Install Base options available in the Action menu on the Saved Bundles page and Managed Bundles page. Non-managed bundles don't have these options on the Saved Bundles page.

![Managed Bundles page with available actions highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleDeprecateActionOptions.png)

Be aware of the following for upgrades to a managed bundle that has been deprecated:

-   The Initiate Upgrade page for the deprecated version of a managed bundle lists only the accounts that have not yet been upgraded to the replacement bundle. This page can be used to push maintenance fixes to accounts with the lagging bundle version.
    
-   The Initiate Upgrade page for the replacement version of the bundle lists accounts with the deprecated version as well as accounts with the replacement version installed. This page can be used to upgrade accounts with the lagging bundle version to the newer version as well as push maintenance fixes to accounts that already have the newer version installed.
    

For steps for upgrading a managed bundle, see [Upgrading Your Managed Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html).

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [Managed Bundles - Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383397.html)
-   [Filtering Managed Bundle Install Base by NetSuite Version](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4846913876.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
-   [Upgrading Your Managed Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
