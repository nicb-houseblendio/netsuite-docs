---
id: "section_N3391248"
type: "section"
title: "Copying a Bundle to Other Accounts"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Copying a Bundle to Other Accounts"
parent: "section_N3384420"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html"
anchors: ["bridgehead_N3391452", "bridgehead_N3391534", "procedure_N3391543", "bridgehead_N3391649", "bridgehead_N3391699"]
sha256: "78ff96f94eac187de0d985babc5f6859c11bd8584b8c282eab0b30a49c00efd5"
---

You can use the Copy option available in the Action list on the Saved Bundles page to copy a customization bundle from one account into another. You can copy one bundle to multiple other accounts. If you make changes to the original bundle, you can repeat the copy action to update copied bundles in other accounts.

-   Copied bundles expand the options for bundle deployment. For example, you can copy a bundle to a deployment account to support your release process.
    
-   Copied bundles can help you to implement a bundle versioning strategy. You can copy a bundle to a development account, allowing the separation of changes to the released bundle version from the development of a new version.
    
-   The ability to copy bundles is linked to the ability to deprecate bundles, meaning replacing a bundle with an updated version. For details about deprecation, see [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html).
    

For details about copying bundles to other accounts, see the following:

-   [Limitations for Copying Bundles](#bridgehead_N3391452)
    
-   [Steps to Copy a Bundle](#bridgehead_N3391534)
    
-   [Reviewing Copy Bundle Status](#bridgehead_N3391649)
    
-   [Notes about Copied Bundles](#bridgehead_N3391699)
    

## Limitations for Copying Bundles {#bridgehead_N3391452}

Note the following limitations on copying bundles:

-   Only customization bundles can be copied. Configuration bundles cannot be copied or deprecated.
    
-   You cannot create a copy of the bundle in the same account where it is currently located (the source account). Each copy must be made to a different account.
    
-   You cannot create more than one copy in any account. When you copy a bundle to an account where it has been previously copied, the existing copy is updated.
    
-   Bundle copy is only supported for production accounts and development accounts. You cannot copy a bundle from or to any type of account other than production or development.
    
-   You cannot copy a bundle to an account where it has been previously installed, and you cannot install a bundle in an account where it has been previously copied. For bundles that are copies of copies, this limitation extends to any bundles that have a common ancestor, based on tracking of the full ancestral path of each bundle.
    
-   You cannot copy a bundle created from an SDF SuiteApp to an account where the same SDF SuiteApp has been previously installed.
    

## Steps to Copy a Bundle {#bridgehead_N3391534}

Complete the following procedure to copy a bundle.

#### To copy a bundle: {#procedure_N3391543}

1.  Go to _Customization > SuiteBundler > Create Bundle > List_.
    
2.  In the **Action** list for the bundle you want to deprecate, click **Copy**.
    
    The Copy Bundle to Accounts page displays, with a list of the accounts to which you have administrator access. (Account IDs and names in the following screenshot have been obfuscated for privacy reasons.)
    
    ![Copy Bundle To Accounts page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleCopy2.png)
3.  Check one or more boxes in the **Copy/Update** column, and click the **Copy** button.
    
    The **Status** column indicates whether the bundle has been previously copied in the account.
    
    -   If you check the box for an account where the bundle has not been copied, a new copy is created.
        
    -   If you check the box for an account where the bundle has been previously copied, this copy is updated with any changes.
        

Note:

During a bundle copy, if conflicts are detected between a copied bundle's objects and existing target account objects, copied bundle objects are added and renamed. For more information about how SuiteBundler resolves conflicts, see [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html).

## Reviewing Copy Bundle Status {#bridgehead_N3391649}

After you click the Copy button on the Copy Bundle to Accounts page, the Copy Bundle Status page appears. This page is also available from the Saved Bundles page, by clicking Show Copies in the Action list.

![Copy Bundle Status page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleCopyStatus.png)

-   The copied bundle's status displays as Pending, whereas previously copied bundle(s) display a green check mark to indicate that the copy action is complete.
    
-   Each copied bundle has a new bundle ID, different from the ID of the source bundle.
    

## Notes about Copied Bundles {#bridgehead_N3391699}

-   A copied bundle is available from the Saved Bundles list in the new account and has the same actions available as bundles created in that account. It includes a Copied From column with the bundle ID and account ID of the bundle from which it was copied, in the format **<Bundle ID> Account:<Account ID>**.
    
-   When you copy a bundle that includes locked objects, the objects are not locked in the account where the bundle is copied. However, their locked settings are maintained on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the copied bundle, and are enforced in target accounts where the copied bundle is installed, unless the settings are changed in the copied bundle. See [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html).
    
-   When you copy a bundle that includes hidden scripts, the scripts are not hidden in the account where the bundle is copied. However, their hidden property is enforced in target accounts where the copied bundle is installed. See [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html).
    
-   Bundle object preferences set in the source account are not applied to the account where the bundle is copied. Note that data is always replaced and script deployments are always updated during an update of a bundle copy. However, source account preferences are maintained on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the copied bundle, and are applied in target accounts where the copied bundle is installed, unless preferences are edited in the copied bundle. See [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).
    
-   The initial availability of a copied bundle is always set to Private, no matter what the availability of the source bundle was, and any shared account IDs listed for the source bundle are cleared from the copied bundle. Copied bundle availability can be reset to Shared or Public as needed, and the account ID list can be cut and pasted from the source bundle, if desired.
    
    -   To change the availability level and add account IDs for a copied bundle, click Set Availability in the Action list. See [Sharing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385867.html).
        
    -   To make other changes to a copied bundle, click Edit in the Action list. See [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html).
        
-   You can differentiate objects added to your account through bundle copy from other account objects, because they have a bundle ID listed in the From Bundle column of list pages. See [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html).
    
-   When you remove any object from a bundle and then copy the bundle to the target account, the object is not removed from the target account if the object is also included in any other bundle copied to the account.
    

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Reviewing the Saved Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385293.html)
-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
-   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)
-   [Deleting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4465929869.html)
-   [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html)
-   [Sending Bundle Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html)
-   [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
