---
id: "section_N3383397"
type: "section"
title: "Managed Bundles - Best Practices"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Managed Bundles Overview > Managed Bundles - Best Practices"
parent: "section_N3382953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383397.html"
anchors: []
sha256: "594e96acbe22ea6fd218c05faec4eb6482672df1cc488f2e44aa61c01bf9dba1"
---

Follow these practices when you use the Managed Bundles feature:

-   Develop a communication plan for your updates. You can push bundle updates that are bug fixes quickly and seamlessly without disturbing your install base. For bundle updates that are new releases, be sure to communicate with your install base ahead of time.
    
-   You can communicate with your bundle install base by sending bundle messages, for example, to welcome new users or to provide upgrade notifications. These messages appear on the Bundle Details page and can also be sent as email to bundle administrators in target accounts. See [Sending Bundle Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html).
    
-   Avoid doing updates during install base peak hours. You can review the regions in which your install base are located on the Bundle Install Base page to determine the time zones that you need to take into account.
    
-   Be sure that bundle updates do not overlap with the NetSuite phased release cycle if the upgrades rely on new features that are only available in the leading version. You can review the current NetSuite versions of your install base on the Bundle Install Base page. See [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html).
    
-   Managed bundles support a phased upgrade process similar to the release process for NetSuite upgrades. You can release a new managed bundle version to subsets of the install base, in phases. See [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html).
    
-   Be aware that the order in which bundled scripts run in the source account is maintained when the bundle is installed in target accounts. You can set up script execution order for client and user event scripts on the Scripted Records page, at _Customization> Scripting > Scripted Records_. See [The Scripted Records Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2936246.html).
    
-   Lock objects in managed bundles to avoid clobbering customizations in target accounts. You can mark bundle objects as locked on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the Bundle Builder. See [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html).
    
-   Set bundle object preferences on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the Bundle Builder, to ensure that objects are set up properly in target accounts. For information about available preferences, see [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).
    
-   You can write SuiteScripts to accomplish required setup tasks that are not covered by bundle preferences, and run these scripts as part of bundle updates in target accounts. You can associate a SuiteScript with a bundle on the [Step 1 Bundle Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html) page of the Bundle Builder. See [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html).
    
-   If you would prefer that bundle objects not be displayed in target account list pages, you can enable the Hide Components option. See [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html).
    

For steps for using the Managed Bundles feature, see [Upgrading Your Managed Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html).

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [Upgrading Your Managed Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html)
-   [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
