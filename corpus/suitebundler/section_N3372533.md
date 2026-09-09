---
id: "section_N3372533"
type: "section"
title: "Step 1 Bundle Basics"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Creating a Bundle with the Bundle Builder > Step 1 Bundle Basics"
parent: "section_N3374254"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html"
anchors: []
sha256: "b563a0407c65612704dbc5df1b5137f1418d11e13a53e0993604ab9dfe04cd78"
---

On the **Bundle Basics** page of the Bundle Builder, enter basic definitions for a bundle .

The following screenshot shows the **Bundle Basics** page:

![Bundle Builder Bundle Basics page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleBasics1.png)

#### To complete Step 1 Bundle Basics in the Bundle Builder:

1.  Log in to the account where you want to create a bundle.
    
    You should consider the bundle deployment strategy before you begin creating a bundle, so that you create the bundle in the appropriate account. For information about bundle deployment, see For explanations of deployment-related terms and preferred deployment methods, see [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html).
    
2.  Go to _Customization > SuiteBundler > Create Bundle_.
    
3.  Enter the following properties:
    
    | Property | Description |
    | --- | --- |
    | Name | Name of the bundle. This is the only required field. |
    | Version | Bundle version used to track future updates. You can use any numbering scheme in this field. This is an optional field, but you should give each bundle a version number to be displayed on bundle list pages. This number is vital to help you manage updates. SuiteBundler alerts your install base to version updates with an icon on bundle list pages and a **SuiteBundles to Update** reminder in the Reminders portlet; these alerts do not occur if you do not use version numbers. |
    | Abstract | Brief description of the bundle. This description is displayed in the **Abstract** column of the **Installed Bundles** page and **Saved Bundles** pages, and on the **Bundle Details** page. This is an optional field. You can enter a longer description on the next page in the Bundle Builder, **Bundle Properties**. For more information, see [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html). |
    | Installation Script | Specialized SuiteScript to be associated with the bundle. A bundle installation script fires triggers that execute as part of bundle installation, update, or uninstall. These triggers automatically complete required setup, configuration, or data management tasks, depending on the bundle. Use this option if you require additional operations in addition to installing the bundle. This script is optional and is not required to install the bundle. See [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html). |
    
4.  If necessary, check the following boxes:
    
    | Box | Description |
    | --- | --- |
    | Configuration Bundle | Indicates the bundle is a configuration bundle that contains setup and configuration objects. When you install a configuration bundle in a target account, it sets configuration parameters, enables or disables features, and sets company preferences. If you check this box, the **Select Objects** page displays only setup and configuration object types. See [Configuration Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html). When this box is checked, the **Managed Bundle** box is disabled because configuration bundles cannot be managed. Note: You cannot create a bundle that contains both customization and configuration objects. If your solution requires both types of objects, you must create and distribute two distinct bundles. |
    | Managed Bundle | Indicates that the upgrade process for the bundle should be controlled by you. When this option is enabled, you can choose when to push updates to accounts that have previously installed the bundle. This control over bundle updates enhances your ability to manage your install base. You must have the Managed Bundles feature is enabled in your account to use this option. See [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html). |
    | Bundle All | Auto-selects all available objects for the bundle. All objects are listed under **Bundle Contents** on the **Select Objects** page, and you can remove objects from the bundle as necessary, rather than adding them. This option may save time, if it is quicker to de-select the objects that you do not want to include in the bundle rather than select the objects that you want to include. |
    | Hide Components | Indicates that the bundle objects do not display in target account lists. By default, bundled objects installed in target accounts display in object list pages. See [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html). |
    
5.  If you are creating a bundle for an SDF SuiteApp project, select the correct value for the **SuiteApp ID** property.
    
    | **Property** | **Description** |
    | --- | --- |
    | SuiteApp ID | Lists SDF SuiteApp projects in your account. You can select a SuiteApp project to be bundled. The objects included in the SuiteApp project are added to the bundle and are shown on the Select Objects page of the Bundle Builder. The selected SuiteApp ID associates a specific publisher, or owner, with the bundle. To obtain a unique publisher ID, you must register with SDN. For information about SDN, go to [http://www.netsuite.com/portal/developers/sdn.shtml](http://www.netsuite.com/portal/developers/sdn.shtml). For information about using SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). |
    
6.  Click **Next**.
    
    To continue creating a bundle in the Bundle Builder, go to [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html).
    

### Related Topics

-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html)
-   [Step 3 Select Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373513.html)
-   [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html)
-   [Finish the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422697218.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
