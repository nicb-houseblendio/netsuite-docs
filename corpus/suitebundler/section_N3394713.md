---
id: "section_N3394713"
type: "section"
title: "Bundle Searches Overview"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Bundle Searches Overview"
parent: "chapter_N3394134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html"
anchors: ["bridgehead_3874318550", "bridgehead_3874342671"]
sha256: "17a50244a1c18b1404ad6db3a990324132d978002be42f83169ecd15c7b7fdbb"
---

The Search & Install Bundles page, available at _Customization > SuiteBundler > Search & Install Bundles_, includes the following two search modes:

-   Basic mode. Simple bundle searches across all production locations.
    
-   Advanced mode. Bundle searches that support additional search filters.
    

Tip:

To search for the most popular bundles by the number of installations, leave the Keywords box blank and click Search.

**Notes:**

-   Both basic and advanced searches show bundles you can install-either public bundles or ones shared with your account. You'll also see bundles that aren't shared with your account but are marked "Visible by All."
    
-   Search results are sorted by the number of installs in target accounts, from highest to lowest.
    
-   If you use advanced search and get multiple pages of results, you should narrow your search criteria to limit the number of bundles returned.
    
-   Basic search doesn't look in Sandbox accounts; to search there, you need to use advanced search.
    
-   A basic search may return multiple instances of a single bundle, if that bundle is available in multiple NetSuite accounts.
    
-   Support for bundle searches varies across the different types of NetSuite accounts. See [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).
    

## Basic Mode {#bridgehead_3874318550}

**Basic** search mode (the default) lets you search for bundles across all production locations. Use basic search when you're not sure where a bundle is or don't have much info about it.

![Search & Install Bundles page Basic items.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleSearchBasicNew.png)

## Advanced Mode {#bridgehead_3874342671}

**Advanced** search mode lets you use extra filters. Use an advanced search when you know the Account ID where a bundle is located or you want to narrow the search based on other bundle characteristics. By default, this search covers all production locations.

![Search & Install Bundles page Advanced items.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/PublisherIDSearch.png)

The following table describes the filters for an advanced search:

| Filter | Description |
| --- | --- |
| Location | Where the source bundle is located -- choose from the following options:
-   **All Production: (the Default)** Lists all bundles to which you have access across all production accounts.
-   **Production Account:** Lists bundles to which you have access in a selected NetSuite production account. You need to provide an account ID when you choose this filter.
-   **Sandbox Account:** Lists bundles to which you have access in a selected sandbox account. You need to provide an account ID when you choose this filter.

 |
| Availability | The options are All, Public, Shared, or Private. |
| Keywords | You can search for bundles by keywords included in the bundle's Name, Bundle ID, Company Name, or Description |
| Product | The NetSuite product for which the bundle is intended, for example, NetSuite OneWorld. |
| Vertical | The vertical market for which the bundle is intended, for example, IT Services. |
| Language | The language translations included in the bundle. For example, a bundle may include translations in French and English of custom records, custom forms, or other elements in the bundle. |
| Publisher ID | Applicable to bundles created from SDF SuiteApp projects. The publisher ID associated with the SuiteCloud Developer Network (SDN) member who created the SDF SuiteApp project on which the bundle is based. |

Note:

If you leave the Keywords box blank for an advanced search, NetSuite returns the most popular bundles that meet the filter criteria.

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Choosing a Bundle to Install](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395426.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
-   [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html)
-   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
