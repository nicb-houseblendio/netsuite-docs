---
id: "section_N3373802"
type: "section"
title: "Step 4 Set Preferences"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Creating a Bundle with the Bundle Builder > Step 4 Set Preferences"
parent: "section_N3374254"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html"
anchors: []
sha256: "b74a3ce28b4dbb7e4d7b49ea5415b2750ffd1ce39b265463b46a00e020bbde4f"
---

On the **Set Preferences** page of the Bundle Builder, you can review the bundle objects, including objects you select and any objects they reference, and save the bundle. For customization bundles, set preferences for objects to be applied during bundle installation and update. You can also lock certain objects to prevent target account users from making changes.

The following screenshot shows the **Set Preferences** page:

![Bundle Builder Set Preferences page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleBuilderPrefs.png)

#### To complete Step 4 Set Preferences in the Bundle Builder:

1.  If you have not already done so, complete [Step 3 Select Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373513.html).
    
2.  Review your bundle's contents. You can take the following actions for the objects included in the bundle:
    
3.  To add or remove objects, click **Back** to return to the **Select Objects** page and make changes.
    
4.  For dashboards, custom fields, custom lists, custom records that include data, custom forms, and SuiteScript files, review the settings in the **Preference** column, and change as desired. These settings are applied for managed bundles and other push installations and updates, and are defaults for other bundle installations and updates. See [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).
    
5.  If you are creating a customization bundle, check boxes in the **Lock on Install** column to lock selected bundle objects, or click **Lock All** to lock all lockable objects in the bundle. See [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html).
    
    For example, an independent software vendor (ISV) may distribute a customization bundle to its customers. To minimize the potential for support and upgrade issues, the ISV may choose to lock objects in the bundle. Locking also protects the ISV's customers from changing objects in a bundle and then discovering they cannot upgrade the bundle without breaking the changed objects.
    
    You cannot lock some objects in customization bundles. Non-lockable objects don't have a box in the **Lock on Install** column.
    
    Locking an object only prevents editing, not viewing. To hide bundle objects in target accounts, see [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html). To prevent target account users from seeing code in bundled server SuiteScripts, see [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html).
    
6.  After you are done making changes, click **Save**.
    
    To continue creating a bundle in the Bundle Builder, go to [Finish the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422697218.html).
    

### Related Topics

-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 1 Bundle Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html)
-   [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html)
-   [Step 3 Select Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373513.html)
-   [Finish the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422697218.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
