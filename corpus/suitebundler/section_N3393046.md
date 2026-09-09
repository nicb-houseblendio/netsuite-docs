---
id: "section_N3393046"
type: "section"
title: "Bundle Details"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Bundle Details"
parent: "section_N3384420"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html"
anchors: []
sha256: "d4dbdeb6c79ffc2037cc104877e4daf76d97bf2c61526a9d08ddb2ec694dcab7"
---

You can view details about a bundle you have created or installed on the Bundle Details page, which is available from the Saved Bundles page and the Installed Bundles page. To view the Bundle Details page from one of these pages, click the bundle name link. To view the Installed Bundles page, go to Customization > SuiteBundler > Search & Install Bundles > List.

![Bundle Details page for custom fields.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleDetails2.png)

-   The **Overview** subtab shows the bundle abstract and description. It also includes a link to any bundle-specific terms of service. See [Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393542.html).
    
-   The **Components** subtab lists bundle objects, including their custom script IDs, referencing objects, and lock status.
    
    -   A bundle may include objects that were not explicitly added by the bundle author, because the Bundle Builder automatically pulls into the bundle any objects on which selected objects depend. These referenced objects display a chain icon. In contrast, objects that have been selected in the Bundle Builder have a check mark icon.
        
    -   In target accounts, the **Components** subtab includes an option to change the setting for whether to hide or show bundle components in lists.
        
        ![Bundle details show components option.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleTargetHideShow.png)
        
        See [Choosing to Hide or Show Bundle Components](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397428.html).
        
-   The **SuiteApp Info** subtab displays details about the bundle from SuiteApp.com, if the bundle is linked to that site.
    
-   The **Messages** subtab displays messages sent to the bundle's install base.
    
    -   If this is a bundle you have created, on this subtab you can create and send new messages. See [Sending Bundle Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html).
        
    -   If this is a bundle you have installed, on this subtab you can select the users in your account who should receive this bundle's messages as email. See [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html).
        

Note:

The Bundle Details page also displays when you select a bundle to install, for your review before the installation. In this case, this page does not include the Messages subtab.

-   If this is a bundle you have installed, the Bundle Details page includes an **Audit Trail** subtab that tracks installations, updates, and uninstalls of this bundle in your account. For details, see [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html).
    
-   If this is a managed bundle you have created, the **Email Recipients** field indicates users who should receive upgrade status notifications. By default the user who initiated the upgrade always receives the notifications. For more details, see [Notifications for Managed Bundle Upgrades](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html#bridgehead_4779622008).
    

Note:

When you try to view details about a bundle whose bundle source account is currently inactive, you will receive the following error message:

`The details about bundle <bundle_ID> cannot be displayed because the bundle source account <bundle_source_account_ID> has been inactivated. Please contact the bundle owner.`

To find out the bundle owner, go to Customization > SuiteBundler > Search & Install Bundles. Then, fill in the bundle ID to the KEYWORDS field and click Search. To identify the bundle owner, see COMPANY NAME in the results table.

### Related Topics

-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Reviewing the Saved Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385293.html)
-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html)
-   [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
-   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)
-   [Deleting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4465929869.html)
-   [Sending Bundle Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393542.html)
-   [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html)
-   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
