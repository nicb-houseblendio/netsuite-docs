---
id: "section_N3386679"
type: "section"
title: "Deprecating a Bundle"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Bundle Availability > Deprecating a Bundle"
parent: "section_N3385668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html"
anchors: ["bridgehead_N3386797", "procedure_N3386807", "bridgehead_N3386926", "svg_1", "svg_1background", "bridgehead_N3387005", "bridgehead_N3387072", "bridgehead_N3387155"]
sha256: "d24e1b4c38273b88b08aa0a0f5b6c844d0cba775663578476b0e7f95ff812690"
---

You can deprecate a bundle to indicate that it is no longer the most up to date version available. When you deprecate a bundle, you specify another bundle as a replacement, newer version. You specify this replacement bundle by its name and NetSuite account ID. For instructions, see [Steps to Deprecate a Bundle](#bridgehead_N3386797).

Warning:

All versions in a bundle deprecation chain should be shared or public at least after their deprecation to avoid errors during bundle upgrades related to the accessibility of deprecated versions.

You can deprecate a bundle only after you have copied this bundle from one account to another. The copy of the bundle serves as the basis for development of a new bundle version. For details, see [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html).

Bundles can have multiple copies, with each copy having its own copies. When you deprecate a bundle, the replacement bundle must be a direct descendant of the deprecated bundle. To understand the chaining of bundle copies, see [Ancestry of Copied Bundles](#bridgehead_N3386926).

Deprecation affects managed and non-managed bundles differently. For details, see [Results of Deprecating Non-Managed Bundles](#bridgehead_N3387005) and [Results of Deprecating Managed Bundles](#bridgehead_N3387072).

On the Saved Bundles page, a deprecated bundle includes a Deprecated By column with the bundle ID and account ID of the replacement bundle, in the format **<Bundle ID> Account:<Account ID>**. For other details about deprecated bundles, see [Notes about Deprecated Bundles](#bridgehead_N3387155).

Important:

Deprecation is available only for customization bundles. You cannot copy or deprecate configuration bundles. Also, you cannot deprecate a bundle that has been created in a sandbox account.

## Steps to Deprecate a Bundle {#bridgehead_N3386797}

Complete the following procedure to deprecate a bundle.

#### To deprecate a bundle: {#procedure_N3386807}

1.  Go to _Customization > SuiteBundler > Create Bundle > List_.
    
2.  In the **Action** list for the bundle you want to deprecate, click **Set Availability**.
    
3.  On the Bundle Availability page, in the Deprecate Bundle section, select a replacement bundle for the bundle to be deprecated.
    
    -   **Deprecate With Bundle** lists bundles that are descendants of the deprecated bundle, in accounts where you have a role with SuiteApp Marketplace permission.
        
    -   The format of list options is **<Bundle ID> Account:<Account ID>**.
        
4.  Review other settings on the page. You may want to change the level of availability for the deprecated bundle or **Visible By All** setting.
    
5.  Save the changes to the Bundle Availability page.
    

## Ancestry of Copied Bundles {#bridgehead_N3386926}

Each copied bundle can have multiple ancestors, depending on the versioning strategy used for the bundled solution. An ancestor can be the bundle from which a bundle was directly copied, or a bundle from which a chained set of copies was made. The following illustration shows a chained set of copies. In this illustration, Bundle A is the common ancestor of all of the other bundles.

Note that bundles must be deprecated by their descendants. For example, in the scenario illustrated here, you could deprecate Bundle B and replace it with Bundle D, but you could not replace it with Bundle C.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                     

-   The deprecation feature supports chained updates across multiple new bundle versions. For example, if you deprecate Bundle A with Bundle B, and later deprecate Bundle B with Bundle D, accounts that still have Bundle A installed will be upgraded to Bundle D when they choose to update.
    
-   A bundle must be deprecated by a direct descendant. For example, in the scenario where: A is copied to B, A is copied to C, and B is copied to D:
    
    -   A can be deprecated by B, C, or D.
        
    -   B can be deprecated by D.
        
    -   D cannot be deprecated because it does not have any descendants.
        

## Results of Deprecating Non-Managed Bundles {#bridgehead_N3387005}

-   Deprecated non-managed bundles cannot be edited in the Bundle Builder.
    
-   The following occurs when users attempt to update or install a non-managed bundle that has been deprecated:
    
    -   When users attempt to install a bundle that has been deprecated, they are notified that the bundle can no longer be installed, and directed to install the replacement bundle instead.
        
    -   When users attempt to update a bundle that has been deprecated, the update uses the replacement bundle. Because a replacement bundle may have different availability settings than its deprecated bundle, an access check for the replacement bundle is performed. If access has not been provided for the user's account, the following message is returned: 'You cannot update this bundle as it has been deprecated, and you have not been granted access to the replacement bundle. Please contact the solution provider.'
        
-   The Bundle Install Base page for a deprecated bundle lists accounts that haven't updated to the replacement bundle. The Bundle Install Base page for a replacement bundle lists accounts that have updated to the replacement bundle, AND accounts that still have the deprecated bundle installed.
    
-   Non-managed deprecated bundles do not have the Edit and Upgrade Install Base options available in the Action menu on the Saved Bundles page, because these actions are not supported.
    

## Results of Deprecating Managed Bundles {#bridgehead_N3387072}

Managed bundle deprecation is handled differently than non-managed bundle deprecation. Managed bundle deprecation allows continuing support of an existing bundle version that has been installed in target accounts, including the ability to release bug fixes and minor changes, at the same time that development of a new version is occurring. See [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html).

-   A deprecated version of a managed bundle can be edited in the Bundle Builder.
    
-   You can continue to push upgrades of the deprecated version of a managed bundle to target accounts that have not yet been upgraded to the replacement version. These actions can occur during the same time period that you are installing and upgrading the replacement version of the bundle in other accounts.
    
-   Deprecated managed bundles have the Edit, Push, and Upgrade Install Base options available in the Action menu on the Saved Bundles page and Managed Bundles page.
    
    Edits to deprecated managed bundles should only be for bug fixes. Edits for new functionality should be made to the replacement bundle.
    
-   The Initiate Upgrade page for deprecated managed bundle versions are organized as follows:
    
    -   The Initiate Upgrade page for the deprecated version of a managed bundle lists only the accounts that have not yet been upgraded to the replacement bundle. This page can be used to push maintenance fixes to accounts with the lagging bundle version.
        
    -   The Initiate Upgrade page for the replacement version of the bundle lists accounts with the deprecated version as well as accounts with the replacement version installed. This page can be used to upgrade accounts with the lagging bundle version to the newer version as well as push maintenance fixes to accounts that already have the newer version installed.
        

## Notes about Deprecated Bundles {#bridgehead_N3387155}

-   Deprecating a bundle affects the display of bundle messages on the Bundle Details page in install base accounts. After an account installs the replacement bundle, only messages sent for that replacement bundle are displayed. Any messages previously sent for the deprecated bundle are not available in these updated accounts. The bundle author can continue to send messages from a deprecated bundle, but these are only sent to accounts that have not yet updated to the replacement bundle. See [Sending Bundle Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html).
    
-   If a replacement bundle includes a bundle installation script, any later replacement bundle deprecating the same bundle must also include a bundle installation script with the same logic. For example, in the case above, if Bundle B's bundle installation script executes data changes before update, Bundle C's bundle installation script must include this same logic in its Before Update function.
    

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Sharing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385867.html)
-   [Implementing Phased Updates by Setting Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3387345.html)
-   [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
