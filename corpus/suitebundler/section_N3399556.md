---
id: "section_N3399556"
type: "section"
title: "Reviewing the Preview Bundle Update Page"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Installed Bundle Updates > Reviewing the Preview Bundle Update Page"
parent: "section_N3397927"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html"
anchors: ["bridgehead_N3399684", "bridgehead_N3399815", "bridgehead_3705113180"]
sha256: "74dd21621ff5ea8ba04aabc2dc4f31c3800161d09fe1aae43bd33a708832cb76"
---

After you click Update for a bundle on the Installed Bundles page, the Preview Bundle Update page opens and lists the objects that'll be added or updated.

Important:

The process for updating bundles installed into production from sandbox is different from the update process for other bundles, to meet the specialized requirements of bundles developed in sandbox accounts. See [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html).

Note:

The process for updating bundles installed into a sandbox account from a development account is the same as the update process for other bundles. The normal bundle update process updates all bundle objects in the target account, overwriting target account objects with source bundle objects. For bundle updates from a development account to a sandbox account, the Preview Bundle Update page always shows the Update action for all objects, even for objects that have not changed in the source account since the last bundle update.

![Preview Bundle Update page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/PrevBundUpdtPrefs.png)

-   For some objects, a lock icon may display in the Lock on Install column, indicating that target account users cannot modify the object.
    
-   For objects that are included in the currently installed version of the bundle, the Action column displays **Update**.
    
-   For objects that are not included in the currently installed version of the bundle, and do not conflict with existing target account objects, the Action column displays **Add**.
    
-   For objects that are not included in the currently installed version and conflict with existing target account objects, the Action column includes a dropdown menu. See [Choose Actions for Conflicting Objects](#bridgehead_N3399684).
    
-   For some objects, you can choose setup preferences in the Preference column. See [Set Bundle Update Preferences](#bridgehead_N3399815).
    

When you're done reviewing the page, click Update Bundle to start the update.

Note:

If you are required to accept new terms of service for the bundle, a dialog displays these terms. Click I Agree to proceed with the update.

You can continue working in NetSuite as the bundle updates. To check on the progress of the update, go to the list of installed bundles at _Customization > SuiteBundler > Search & Install Bundles > List_. See [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html).

## Choose Actions for Conflicting Objects {#bridgehead_N3399684}

On the Preview Bundle Update page, conflicting objects show up in red in the Existing Object in Conflict and Script ID columns. For each conflict, pick one of these options from the Action dropdown:

-   **Add and Rename** - NetSuite appends a number to the bundle object's name or script ID, to differentiate it from the preexisting custom object. The bundle object is added to account, and the preexisting object remains intact.
    
-   **Replace Existing Object** - The bundle object keeps the same name or script ID. The bundle object is added to the account and the preexisting custom object no longer exists in the account.
    
    If you choose this option for a conflicting object during bundle installation, the preexisting custom object is PERMANENTLY replaced by the bundle's object. Even if you choose to uninstall the bundle later, changes to the replaced object remain and the original object is not restored.
    
    For each custom record that includes data and each custom list where this option is chosen, a preference dropdown list is displayed so you can choose whether to replace, preserve, or merge data in the target account object to be replaced.
    

For more information, see [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html).

## Set Bundle Update Preferences {#bridgehead_N3399815}

On the Preview Bundle Update page, review the bundle object preferences set by the author and change them if you want. The following preferences may be available:

-   Do Not Update Users or Update Users of Published Dashboards
    
    For each dashboard being updated as part of this update, you can set a preference to indicate whether these updates should be applied to the dashboards of users to whom the dashboard has been published. (Updates are always applied to the dashboard definition.)
    
    The default option is not to apply updates to users, allowing an administrator to publish updates to users' dashboards as desired after the bundle update. See [Applying Changes to Published Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N634404.html).
    
-   Show or Hide Custom Fields
    
    For each custom field being installed for the first time, you can choose whether it shows or hides on existing custom forms in your account. The setting you chose during the most recent installation or update of this bundle is displayed by default.
    
    Note that this setting does not affect bundled forms, because all custom fields in a bundle are always shown on all custom forms included in that bundle.
    
-   Update or Do Not Update Script Deployments
    
    For each SuiteScript to be updated, you can choose whether to update script deployments in the target account. The setting you chose during the most recent installation or update of this bundle is displayed by default.
    
    If the update deployments option is applied, bundled script deployments completely overwrite target account script deployments, **except for script deployment audience definitions**. Bundle updates do not impact script deployment audience definitions in target accounts. These audiences are not changed, even if the Update Deployments option is applied.
    
    Note that changes to an icon associated with a dashboard SuiteApp portlet are always copied during a bundle update. This overwrite of the icon in the target account occurs even if the bundle preference is set to prevent the update of script deployments. See [Giving Users Dashboard Access to a SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html#bridgehead_4852122809).
    
-   Replace Data, Preserve Data, or Merge Data for Custom Records and Custom Lists
    
    This preference is available for each custom record with data and each custom list that conflict with existing target account objects and have Replace Existing Object chosen, as well as for each custom record with data and each custom list that need to be updated as part of the bundle update.
    
    You can choose one of the following: Replace Data, Preserve Data, or Merge Data. (The setting you chose during the most recent update of this bundle is displayed by default.)
    
    -   The Replace Data option overwrites existing target account object data with bundle object data. This process compares script IDs for records in the bundle and those in the account, to do the following:
        
        -   Delete records from the target account that no longer exist in the bundle's source account.
            
        -   Update records in the target account that also exist in the source account so that values match.
            
        -   Add records to the target account that are new to the source account since the bundle was previously updated in the target account.
            
    -   The Preserve Data option preserves existing data in the target account object.
        
    -   The Merge Data combines bundled object data with target account object data. As part of this merge:
        
        -   Any records that were added to the object in the target account after bundle installation are preserved.
            
        -   Any records that were added to the object in the bundle source account, after installation in the target account, are added to the target account object.
            
        -   Any records in the target account object that were added as part of the bundle installation and remain in the bundled account object are handled as follows:
            
            -   If the values are the same in both objects, target account object values are preserved as is.
                
            -   If the values are different, target account object values are updated to match bundled account object values.
                
        
        NetSuite uses internal IDs to compare and update these values.
        

## Merge Data Example {#bridgehead_3705113180}

For example, consider a custom list called Colors that has been installed as part of a bundle in a target account. At the point in the time when a bundle update is to occur, this list has different data in the target account and the bundle:

-   The values in the existing target account Colors list are: red, orange, yellow, green, blue, and purple (installed by the bundle), and white (added in the target account after bundle installation).
    
-   The values in the bundled Colors list are: red, orange, yellow, green, blue, indigo, violet (changed from previous value of purple), black, and gray.
    

Results of updating the bundle would vary according to the option chosen for the custom list data preference, as shown in the following table:

| Option Chosen | Target Account Colors List Data After Bundle Update |
| --- | --- |
| 
Preserve Data

(Do not change target account object data.)



 | red, orange, yellow, green, blue, purple white |
| 

Replace Data

(Overwrite target account object data with bundled object data.)



 | red, orange, yellow, green, blue, indigo, violet, black, gray |
| 

Merge Data

(Add bundled object data to target account object data, eliminating any duplicates.)



 | red, orange, yellow, green, blue, indigo, violet, white, black, gray Note merge handling of data values:

-   red, orange, yellow, green, blue remain as is
-   purple is updated to violet
-   white is preserved
-   indigo, black, and gray are added

 |

Note:

Bundle updates do not change the values of script deployment parameters that have a user or company preference set, even if the bundle preference for the script is set to Update Deployments. For more information, see [Script Parameter Preference Updates in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000106.html).

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Bundle Update Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400349.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Choosing a Bundle to Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399359.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
