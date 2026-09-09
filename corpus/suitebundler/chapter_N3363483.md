---
id: "chapter_N3363483"
type: "chapter"
title: "SuiteBundler Overview"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteBundler Overview"
parent: "book_N3363377"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3363483.html"
anchors: []
sha256: "472bdafab45be74e5bb7808c484fbfd587a0d49d197096b2d92a97bb2da50158"
---

Note:

SuiteBundler is still supported, but it will not be updated with any new features.

To take advantage of new features for packaging and distributing customizations, you can use the Copy to Account and SuiteCloud Development (SDF) features instead of SuiteBundler.

Copy to Account is an administrator tool that you can use to copy custom objects between your accounts. The tool can copy one custom object at a time, including dependencies and data. For more information, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

SuiteCloud Development Framework is a development framework that you can use to create SuiteApps from an integrated development environment (IDE) on your local computer. For more information, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).

SuiteBundler allows NetSuite users to package together groups of objects for distribution to other accounts. These packages are called bundles, or SuiteApps. Bundle authors may be internal developers creating customizations for their companies, independent software vendors (ISVs) distributing solutions to their customers, or administrators making their bundles publicly available through a deployment account.

Two types of bundles can be created and made available for installation:

-   A **customization bundle** is a group of custom objects that implement customized behavior in the NetSuite application.
    
-   A **configuration bundle** is a group of NetSuite setup entries and preference settings.
    

NetSuite offers a Bundle Builder that guides you through creating bundles. NetSuite account administrators and users with the SuiteApp Marketplace permission can use the Bundle Builder when the SuiteBundler feature is enabled. In the Bundle Builder, users define bundle properties and select objects to be included.

After you've created a bundle, you're setting its availability - it can be private, shared with specific accounts, or public.

NetSuite administrators and users with SuiteApp Marketplace permission can install bundles that have been shared with their accounts or made public. You can install a bundle from another NetSuite account if you have the account ID.

Users can search for a bundle across all locations, including production accounts and sandbox accounts. They also have options to narrow a bundle search to a specific location or filter it by keywords or by bundle characteristics such as Availability, Product, Vertical, and Language.

Important:

Bundles are also known as SuiteApps.

SuiteBundler help topics are aimed primarily at users who want to create and distribute bundles. There are also help topics targeted at users who want to install bundles.

For information about how bundle support varies in different NetSuite account types, including sandbox, Release Preview, and development accounts, see [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).

For information about creating bundles, see:

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
    
    -   [Types of Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364548.html)
        
    -   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
        
    -   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
        
    -   [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html)
        
    -   [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html)
        
    -   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
        
    -   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
        
    -   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)
        
    -   [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html)
        
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
    
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
    

For information about installing bundles, see:

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
    
    -   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
        
    -   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
        
    -   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
        
    -   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
        
    -   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
        
    -   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
        
    -   [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html)
        
    -   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)
        
    -   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
        
    -   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)
        
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
    
-   [SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_3134602194.html)
    

For information about creating bundles that include custom transaction types, see [Custom Transaction Types in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4177814825.html).

For information about adding a custom segment to a bundle, see [Adding a Custom Segment to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4520725557.html).

You can also use SuiteScript to get information about installed bundles and SuiteApps. For more information, see [N/suiteAppInfo Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160236086332.html).

### Related Topics

-   [SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N3363377.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
-   [SuiteBundler Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3783020489.html)
-   [Custom Transaction Types in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4177814825.html)
-   [Adding a Custom Segment to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4520725557.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
