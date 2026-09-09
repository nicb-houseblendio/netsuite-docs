---
id: "section_N3387345"
type: "section"
title: "Implementing Phased Updates by Setting Bundle Availability"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Bundle Availability > Implementing Phased Updates by Setting Bundle Availability"
parent: "section_N3385668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3387345.html"
anchors: ["procedure_N3390941"]
sha256: "ffcb7426c4855203a2220e6fc277651e431c4b894f104b809103460356c4f1d5"
---

For managed bundles, NetSuite supports phased release of upgrades to subsets of the install base. For details, see [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html).

NetSuite does not support this same process for bundles that are not managed. However, you can complete the following steps to release an upgrade for a non-managed bundle to subsets of your install base.

#### To release a bundle update to subsets of customers in phases: {#procedure_N3390941}

1.  Create a new bundle. (See [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html).)
    
    1.  Set the bundle version number and include it in the bundle name for maximum clarity, for example, My SuiteApp v1.0.
        
    2.  Set the bundle's availability to **Public** or **Shared**, so that it is available for installation by customers. If you set it to **Shared**, enter account IDs for all customers on the Bundle Availability page. (See [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html).)
        
2.  Copy the original bundle. (See [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html).)
    
    1.  Up the version number of this copy and include the version number in the bundle name, for example, My SuiteApp v2.0.
        
    2.  Set the bundle availability to **Private** during the time that it is in development.
        
    3.  Make the desired updates to the bundle.
        
3.  At this point, you can deprecate the original bundle with the copied bundle, to prevent new customers from installing the older bundle version. (See [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html).)
    
    Be aware that after the original bundle is deprecated, it can no longer be edited.
    
4.  Set the availability of the copied bundle to Shared, and enter account IDs on the Bundle Availability page for the subset of customers who should have access to the updated bundle in the first phase.
    
    -   All of the customers who have installed My SuiteApp v1.0 will see an 'Update Available' indicator.
        
    -   However, only the customers whose account IDs are listed on the Bundle Availability page for My SuiteApp v2.0 will be able to update the bundle.
        
    -   Other customers will see an error when they attempt to run the bundle update. To reduce confusion, you need to proactively communicate with customers about when they can expect the update to be available for their accounts.
        
5.  Repeat step 4 multiple times, as desired, to enter account IDs for additional customers on the Bundle Availability page, until you have made the updated bundle available to all of your customers.
    

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Sharing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385867.html)
-   [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html)
-   [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
