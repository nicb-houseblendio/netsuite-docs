---
id: "section_N3391992"
type: "section"
title: "Pushing a Bundle to Other Accounts"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Pushing a Bundle to Other Accounts"
parent: "section_N3384420"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html"
anchors: ["procedure_N3392077"]
sha256: "96a58f1dbc44e5c5581a38e716927886d521631a65d920dec05e2422619b4e5f"
---

Bundle authors can push their bundles to any NetSuite account to which they have administrator access. This enables NetSuite resellers and independent software vendors to install bundles without having to log in to each of their customers' accounts.

Important:

The Push action is not available in sandbox accounts. If you want to install a bundle from a sandbox account to another account where you have administrator access, you will need to go to that target account to search for and install the bundle. The Push action is only available in production accounts and development accounts and bundles can only be pushed to production accounts and development accounts.

When you push a bundle installation or update, the preferences you set in the Bundle Builder for custom fields, custom lists, custom records that include data, and SuiteScript deployments are applied directly to target accounts. Users in these accounts cannot override your preferences. See [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).

#### To push a bundle to another account: {#procedure_N3392077}

1.  Go to _Customization > SuiteBundler > Create Bundle > List_.
    
2.  Select **Push** from the **Action** list for the bundle you want to push.
    
    On the Push Bundles to Accounts page, NetSuite displays all of the accounts to which you have administrator access, with details about each account, including the status of the selected bundle's installation.
    
    You can filter the target accounts displayed on this page by region and bundle version. See [Filtering on Bundle Install Base Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_96103016312.html).
    
    ![Push Bundle to Accounts page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/PushBundleNew.png)
3.  Check the **Include** box for each account where you want to install the bundle.
    
4.  Click the Push button.
    

After you have pushed the bundle, the Bundle Install Base page appears. This page includes the status of the bundle installation on each account. See [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html).

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Reviewing the Saved Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385293.html)
-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html)
-   [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html)
-   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
-   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)
-   [Deleting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4465929869.html)
-   [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html)
-   [Sending Bundle Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
