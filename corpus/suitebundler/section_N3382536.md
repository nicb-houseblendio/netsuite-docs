---
id: "section_N3382536"
type: "section"
title: "Bundle Support during NetSuite Release Phasing"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Bundle Support during NetSuite Release Phasing"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html"
anchors: []
sha256: "e4420d8b0732ff3c0bddc7c8a76b9229df88809c7ce62d0121f494dad316be6b"
---

Upgrades of NetSuite accounts to each new release occur as a phased process. During phasing of a new release, some accounts are still using the lagging version of NetSuite during the time that other accounts have been upgraded to the leading version. During this time period, you are likely to be using a different NetSuite version than some of the accounts where your bundles are installed, so you need to be aware of the following:

-   Bundles developed with the lagging version can be installed into accounts that are already using the leading version.
    
-   Bundles developed with the leading version can be installed into accounts that are still using the lagging version, but note the following limitations:
    
    -   When a user in a lagging version account installs a bundle from a leading version account, any object types in the bundle that are not supported in the lagging version are not installed, resulting in potentially serious impact to bundle function.
        
    -   A bundle with a SuiteScript that uses a new API available only in the leading version can be installed into a lagging version account, but the script may not function correctly because the lagging version does not support the API.
        

You should avoid distributing bundles containing any new leading version API to accounts still using the lagging version. To accomplish this purpose, you can create a bundle installation script that uses the **getVersion()** method to check the target account version, and prevents installation of the associated bundle if the lagging version is in use. See [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html) and the SuiteScript help topic [Setting Up a Bundle Installation Script](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158134526570.html).

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
