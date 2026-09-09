---
id: "section_N3382953"
type: "section"
title: "Managed Bundles Overview"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Managed Bundles Overview"
parent: "chapter_N3364150"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html"
anchors: ["bridgehead_N3383151", "bridgehead_N3383221", "procedure_N3383234"]
sha256: "77bf73fc049790b82468e5dc7aac136320daf6820c14c1a653f3d5577599e070"
---

Important:

This topic is aimed at solution providers who create managed bundles. For information about installing and using managed bundles, see [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html).

If the Managed Bundles feature is enabled in your account, you can create managed bundles to give you control over when bundles are updated in target accounts. When installing a managed bundle, the installer agrees to receive future updates at the author's discretion. As updates are developed, they can be installed by the bundle author into the target accounts without any action required by the target account administrator. Only customization bundles can be managed bundles.

Note:

If you are a Premier or Select member of the SuiteCloud Developer Network, you can request access to the Managed Bundles feature by filing a support case through the NetSuite Partner Center. Be sure to include your deployment account ID.

**The Managed Bundles feature is only enabled on SDN trailing accounts.** An SDN trailing account is one that is upgraded in the last phase of a phased release. The Managed Bundles feature is not available for SDN leading accounts.

To indicate that a bundle is a managed bundle, check the Managed Bundle box on the [Step 1 Bundle Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html) page of the Bundle Builder. The box is only visible if the Managed Bundles feature is enabled. The option is disabled if Configuration Bundle is enabled, as only customization bundles can be managed.

Unlike pushing bundles, updating a managed bundle from the source account does not require administrator access to the target account. If, however, a bundle author has administrator access to another NetSuite account, they can install a managed bundle in that account. Managed bundles can be saved and upgraded through a deployment account.

Warning:

You should not remove a bundle from the copy chain while the older version of the bundle is installed by some users and that version is deprecated by a newer version of the bundle. Removing a bundle from the copy chain prevents users from installing the latest version. To understand the chaining of bundle copies, see [Ancestry of Copied Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html#bridgehead_N3386926).

For more information about managed bundles, see:

-   [Managed Bundles in Target Accounts](#bridgehead_N3383151)
    
-   [SuiteBundler Upgrade Install Base Permission](#bridgehead_N3383221)
    
-   [Managed Bundles - Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383397.html)
    
-   [Upgrading Your Managed Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html)
    
-   [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html)
    
-   [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html)
    
-   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
    
-   [SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_3134602194.html)
    
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
    
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
    
-   [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html)
    

## Managed Bundles in Target Accounts {#bridgehead_N3383151}

When users install a managed bundle in their account, they are presented with a popup message informing them that by installing the bundle, they are giving the bundle author permission to install future updates at any time.

![Confirmation message to proceed with bundle installation.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/Bundler_managedBundle_agreementDialog.png)

If a bundle is installed and later changed to a managed bundle, the next time the installer clicks **Update**, they are informed of the change and must agree to have the bundle managed by the developer before it can be updated. If the installer no longer wants the managed bundle, they can uninstall it and receive no further upgrades.

In addition, for managed bundles, target account users cannot override bundle object preferences set by bundle authors. If a user-installed bundle later becomes managed, all preferences previously selected in target accounts are ignored during bundle updates. See [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).

SuiteBundler sends email notifications of managed bundle upgrades to target account users. Email recipients can be designated on the Bundle Details page. When a managed bundle is successfully upgraded in a target account, an email message containing the bundle name, bundle ID, bundle version, and account ID is sent. No email is sent if the upgrade fails. Recipients are determined by the **Email Recipients** setting on the Bundle Details page. The default choice is **All Bundle Admins**, indicating that all administrators and users with the SuiteApp Marketplace permission in the account are recipients. Choosing **None** opts out of receiving the email. A choice of **Custom** allows the entry of specific users to receive the email.

The list of installed bundles, at _Customization > SuiteBundler > Install Bundle > List_, has a Managed column that indicates which bundles are currently managed, for reference purposes.

## SuiteBundler Upgrade Install Base Permission {#bridgehead_N3383221}

By default, only account administrators can upgrade bundles managed by your company, but you can assign the SuiteBundler Upgrade Install Base permission to custom roles to allow developers and release engineers to perform upgrades.

#### To grant the SuiteBundler Upgrade Install Base permission: {#procedure_N3383234}

1.  Edit or customize the role to which you want to give this permission.
    
2.  On the **Permissions** subtab, click the **Setup** subtab.
    
3.  In the **Permission** column, select **SuiteBundler Upgrade Install Base**.
    
    The access level is set to **Full**.
    
4.  Click **Add**.
    
5.  Click **Save**.
    

This permission grants access to the Managed Bundles page.

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Types of Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364548.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Managed Bundles - Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383397.html)
-   [Upgrading Your Managed Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html)
-   [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
