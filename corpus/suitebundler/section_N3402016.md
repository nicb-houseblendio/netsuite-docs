---
id: "section_N3402016"
type: "section"
title: "Filtering Bundle Objects on List Pages"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Filtering Bundle Objects on List Pages"
parent: "chapter_N3394134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html"
anchors: []
sha256: "138638b87744a1ddddf5c088340ae9286a90c3e51b9d2638ba41ab20615028f0"
---

Any NetSuite list page for a bundleable object type may display objects that have been installed by a bundle. You can use the **From Bundle** dropdown list in the **Filter** area to filter the objects from bundles that are displayed on the page. This filtering capability can make object lists more manageable, allowing you to shorten lists and find specific objects.

Whether a bundle's objects are displayed in list pages depends on the hide or show setting for bundle components. This setting is defaulted according to the option chosen by the bundle author. In your account, this setting can be changed on the Bundle Details page. See [Choosing to Hide or Show Bundle Components](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397428.html).

![From Bundle options on the Custom Entry Forms page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleFromBundleFilter.png)

The **From Bundle** filter includes the following options:

-   **Any** - Select this option to display any objects that have been installed by bundles. Objects created within the account are not displayed.
    
-   **None** - Select this option to display only objects created within the account. Objects installed by bundles are not displayed.
    
-   **<Bundle ID>** - ID for each bundle that has been installed in the account - Select a bundle ID to display only objects that have been installed by that specific bundle.
    

The **From Bundle** filter is available on list pages for all object types that have at least one object installed by a bundle, where that bundle is not marked to hide components. For example, if an account contains custom lists, custom records, and saved searches installed by bundles, and none of these bundles are marked to hide components, the **From Bundle** filter is available on Custom List, Custom Record, and Saved Search list pages. However, if an account contains custom roles installed by a bundle, but that bundle is marked to hide components, these roles are not displayed in the roles list page and the **From Bundle** filter is not available on this page.

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Choosing to Hide or Show Bundle Components](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397428.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
-   [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html)
-   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
