---
id: "section_N3373513"
type: "section"
title: "Step 3 Select Objects"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Creating a Bundle with the Bundle Builder > Step 3 Select Objects"
parent: "section_N3374254"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373513.html"
anchors: ["bridgehead_4422693502"]
sha256: "6b76a00f27371f1ca1886d02b80a98cac8bea1c35826937aec19f529dce805a3"
---

On the **Select Objects** page of the Bundle Builder, select the objects to be included in the bundle. The available objects vary, depending on whether you are creating a customization bundle or a configuration bundle. See [Objects Available in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364871.html#bridgehead_N3364890) and [Objects Available in Configuration Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html#bridgehead_N3366368).

![Bundle Builder Select Objects page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleSelectObjects.png)

#### To complete Step 3 Select Objects in the Bundle Builder:

1.  If you have not already done so, complete [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html).
    
2.  In the **Object Types** list, expand the folder for the type of object that you want to include in the bundle.
    
    The **Choose Objects** list displays available objects of the selected type, if any.
    
3.  In the **Choose Objects** list, check the box next to each object you want in the bundle, or check the **Select All** box to check all of the objects listed for the object type.
    
    Each time you check a box, NetSuite updates the **Bundle Contents** list.
    
    Warning:
    
    Enabling the **Include Data** option for a bundled custom record object with an extremely large number of custom records may result in bundle installation failure due to network connection problems. To ensure installation success, do not enable the **Include Data** option for the custom record object. Then run a bundle installation script that executes after installation to import custom record object data into the target account through CSV import. For information, see [SuiteScript 2.1 Bundle Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460460309.html) and [task.CsvImportTask](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345798668.html).
    
    Note:
    
    If there are existing custom records for a bundled custom record object, check the **Include Data** box under the object to include this data in the bundle. Even if you do not check the **Include Data** box, NetSuite may still pull data for a custom record, if another object in the bundle depends on the data in the custom record.
    
4.  To de-select an object, select its object type in the **Bundle Contents** list and clear its box in the **Choose Objects** list.
    
5.  Click **Next.**
    
    To continue creating a bundle in the Bundle Builder, go to [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html).
    

## General Guidelines for Selecting Objects {#bridgehead_4422693502}

-   When you add most types of custom objects to a bundle, all of the necessary elements referenced by that object are also automatically added to the bundle, so you do not need to explicitly add them. However, some referenced objects are not added automatically, and you'll need to add them manually. For more information, see [Referenced Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3920794409.html).
    
-   For customization bundles, use unique script IDs for each object to prevent installation conflicts. If a bundle object's ID matches one in the target account, the bundle object's ID will be appended with a number. For more information, see [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html).
    
-   If your bundle includes server SuiteScripts, you can check the Hide in SuiteBundle box on their File Cabinet file records to prevent users who install the bundle from viewing the script files. See [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html). Client SuiteScript files or files referenced in client SuiteScript files cannot be hidden.
    
-   If you see configuration objects (Company Preferences, Features, Other Lists, and Renaming) on the Select Objects page, you have set the bundle to be a configuration bundle. To define the bundle as a customization bundle, go back to the Bundle Basics page and clear the **Configuration Bundle** box.
    
-   Including a configuration object in a configuration bundle does not create a new instance of that object in the target account when the bundle is installed. Configuration bundle installation simply copies the settings for included configuration objects from the source account to the target account.
    

### Related Topics

-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 1 Bundle Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html)
-   [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html)
-   [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html)
-   [Finish the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422697218.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
