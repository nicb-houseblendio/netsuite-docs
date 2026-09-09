---
id: "chapter_N3405306"
type: "chapter"
title: "SuiteApps and Sandbox Accounts"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApps and Sandbox Accounts"
parent: "book_N3363377"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html"
anchors: ["bridgehead_3770203406", "bridgehead_3770202010", "bridgehead_3770203715"]
sha256: "b69665ce3556144c8e2048a1bd7f25a62449e45939d1205c73f9fb4849710773"
---

NetSuite sandbox accounts let you develop and test bundles without disrupting your day-to-day business in your NetSuite production account. You can use one or more sandbox accounts for development and testing of your own bundles as well as for testing bundles from external sources such as independent software vendors (ISVs).

Sandbox accounts offer:

-   a safe place to test customizations to NetSuite, such as bundles
    
-   a realistic starting point for development, since they start out as a copy of your production account, including its setup, data, and customizations
    

For general information about using sandbox accounts, see [NetSuite Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N333400.html). The NetSuite Development account is another option besides Sandbox. For details, see [The Development Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1121105419.html), [NetSuite Development Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4422375565.html), and the [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html).

Note:

Support for bundle operations varies between different types of NetSuite accounts, including sandboxes. See [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).

## Sandbox Bundle Deployment Models {#bridgehead_3770203406}

Review the following for brief descriptions of sandbox bundle deployment models:

-   [Single Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405732.html)
    
-   [Two Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405828.html)
    

## Limitations for Bundles in Sandbox Accounts {#bridgehead_3770202010}

Some features are limited in their functionality in sandbox accounts, particularly features related to payroll and credit card processing. When you're developing or testing bundles, make sure you keep these sandbox limitations in mind. For a complete list of limitations, see [Features Available for Testing in a Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N335071.html).

Also, keep in mind:

-   You can't deprecate a bundle created in a sandbox account. But if a bundle installed in a sandbox is deprecated, you can update it with the replacement bundle.
    
-   The Copy action isn't supported in sandbox accounts.
    
-   Unlike managed bundles installed in production accounts, managed bundles installed in sandbox accounts must be updated manually. For more information about managed bundles, see [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html).
    
-   The Push action isn't available in sandbox accounts. If you want to install a bundle from a sandbox to another account where you're an administrator, you'll need to go to that target account to search for and install the bundle.
    
-   Don't check the Hide In SuiteBundle box for a script you want to include in a sandbox-developed bundle. Checking this box for a script in the source sandbox account for the bundle can eventually lead to the script being hidden in that account. After the bundle is installed in production and the sandbox account is later refreshed, the production account setting for this option is copied to the sandbox account. This copy causes the Hide in SuiteBundle box to be checked and disabled in the source sandbox account, preventing bundle developers from accessing the script. For information about this option, see [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html).
    
-   Don't lock bundle objects you want to include in a sandbox-developed bundle. Locking objects in the source sandbox account for the bundle can eventually lead to the objects being locked in that account. After you install the bundle in production and refresh the sandbox, the production settings for locked objects are copied to the sandbox. This copy causes the objects to be locked in the source sandbox account, with their lock options disabled, preventing bundle developers from editing these objects. For information about setting lock preferences, see [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html).
    
-   Support for bundle operations varies across the different types of NetSuite accounts, including sandbox accounts. See [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).
    

Warning:

Users are strongly cautioned NOT to rebundle objects that are installed in sandbox from other bundles. If such objects are rebundled, users are also cautioned not to install these bundles in production. Installing bundles with rebundled sandbox objects in a production account has a particularly detrimental impact on SuiteApps, including managed bundles from NetSuite or partner-bundled solutions. These production rebundles can result in an unexpected state of the bundle and account data, and actions to resolve such a state may result in data loss. Users can reduce the risk of such rebundling unintentionally occurring by avoiding the use of the Bundle All option. Manually selecting components ensures that all components are not added by default.

## Specialized Features for Sandbox Bundle Development {#bridgehead_3770203715}

Sandbox bundle development involves issues that you do not encounter for bundles installed from an external (ISV) account into your production account. Because your sandbox account is a copy of your production account, the objects included in a bundle created in sandbox are likely to also exist in production. Because of this copying, bundle updates from sandbox to production usually involve significantly more object conflicts than updates of ISV bundles. Refreshes of a sandbox account can result in overwriting of bundle objects and loss of data, due to changes made to bundle objects in production. See [Sandbox Refresh Impact on Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405932.html).

SuiteBundler includes the following features that address unique issues for bundles developed in sandbox accounts:

-   [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html)
    
-   [Dissolving Bundles Created in Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770244609.html)
    

### Related Topics

-   [SuiteBundler Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3363483.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [SuiteBundler Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3783020489.html)
-   [NetSuite Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N333400.html)
-   [Refreshing Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N334348.html)
-   [Single Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405732.html)
-   [Two Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405828.html)
-   [Sandbox Refresh Impact on Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405932.html)
-   [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html)
-   [Dissolving Bundles Created in Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770244609.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Custom Transaction Types in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4177814825.html)
-   [Adding a Custom Segment to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4520725557.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
