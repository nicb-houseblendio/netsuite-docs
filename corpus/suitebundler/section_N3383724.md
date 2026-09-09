---
id: "section_N3383724"
type: "section"
title: "Upgrading Your Managed Bundle Install Base"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Managed Bundles Overview > Upgrading Your Managed Bundle Install Base"
parent: "section_N3382953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383724.html"
anchors: ["bridgehead_4779578669", "bridgehead_4779577970", "bridgehead_4779622008", "bridgehead_4779581148", "procedure_N3383766"]
sha256: "c4c822a90d98900599bc97c186fd4ddae60b2480b1921b7910e38c82278b2c02"
---

One of the issues that solution providers face is ensuring that users of their bundles apply updates as they become available. Managed bundles allow you to upgrade bundles in the accounts where they are installed whenever a new version is available.

Users who have installed a managed bundle do not have responsibility for updating it; the bundle author completes this task at their discretion. For managed bundles, only an administrator or a user with the SuiteBundler Upgrade Install Base permission can apply updates to the install base.

For information about managed bundle upgrades, see:

-   [Timing Managed Bundle Upgrades](#bridgehead_4779578669)
    
-   [Canceling Pending Managed Bundle Upgrades](#bridgehead_4779577970)
    
-   [Notifications for Managed Bundle Upgrades](#bridgehead_4779622008)
    
-   [Steps for Managed Bundle Upgrades](#bridgehead_4779581148)
    

Note:

Support for managed bundle upgrades varies across the different types of NetSuite accounts. See [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).

## Timing Managed Bundle Upgrades {#bridgehead_4779578669}

With managed bundles, you can more carefully manage updates during the phased NetSuite release cycle when some of the accounts in your install base might be running a different version of NetSuite than your account. Managed bundles support a phased upgrade process that supports maintenance of multiple versions of a managed bundle. With phased upgrades, you can continue to push maintenance updates to accounts still using the older version of the bundle, during the time that other accounts are being upgraded to the new version. See [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html).

You can use the Release Preview account to test updates to a managed bundle before you push updates to the production accounts for your install base. For more information about the Release Preview account, see [Overview of Release Preview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471776042.html) and [Test Your Installed SuiteApps (Bundles)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471785065.html).

Note:

You should not attempt to maintain more than two released versions of a managed bundle at any one time.

## Canceling Pending Managed Bundle Upgrades {#bridgehead_4779577970}

Managed bundle upgrades are typically pushed to multiple target accounts at one time. If you discover an error before the upgrade is completed in all target accounts, you can stop the upgrade immediately. You do not have to wait for the upgrades to complete in all accounts and then start over. The **Cancel Pending Upgrades** button is available on the Initiate Upgrade page for managed bundles. You can click this button to cancel the upgrades in any target accounts that have a status of **Pending**.

## Notifications for Managed Bundle Upgrades {#bridgehead_4779622008}

SuiteBundler sends email notifications of successful managed bundle upgrades to target account users. For details, see [Managed Bundle Upgrade Notifications to Target Account Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html#bridgehead_4779618604).

SuiteBundler also sends email notifications of managed bundle upgrades to bundle owners. After a managed bundle upgrade has ended, a summary email message containing details about the upgrade is sent to the user who initiated the upgrade. This message can also be sent to other users in the managed bundle's source account. These additional recipients can be set in a new **Email Recipients** field that is available on the Bundle Details page in the source account.

This summary email has a subject of **Summary of Managed Upgrade for Bundle <BundleID>**. It includes the following details:

-   bundle ID
    
-   bundle name
    
-   bundle version
    
-   source account ID
    
-   overall upgrade start date and time
    
-   overall upgrade end date and time
    
-   overall status
    
    -   Completed - Upgrade was initiated on all target accounts.
        
    -   Failed - Process failed unexpectedly before upgrade was initiated on all accounts.
        
    -   Canceled - Upgrade initiator clicked Cancel before upgrade was initiated on all accounts.
        
-   details for each target account
    
    -   account ID
        
    -   company name
        
    -   status
        
    -   upgrade start date and time
        
    -   upgrade end date and time
        

## Steps for Managed Bundle Upgrades {#bridgehead_4779581148}

Complete the following procedure to upgrade a managed bundle.

#### To upgrade a managed bundle: {#procedure_N3383766}

1.  Go to _Customization > SuiteBundler > Managed Bundles_.
    
2.  Click **Upgrade** next to the bundle you want to install in other accounts.
    
3.  The Initiate Upgrade page shows the following:
    
    -   the account number and name of each company that has installed your managed bundle
        
    -   the version of NetSuite they are running
        
    -   the version of the bundle installed in the account
        
    -   the date of the installation
        
        Note:
        
        The date value is hardcoded to Pacific Time Zone and does not reflect the time zone setting on _Home > Set Preferences_.
        
    -   the date of the last upgrade
        
        Note:
        
        The date value is hardcoded to Pacific Time Zone and does not reflect the time zone setting on _Home > Set Preferences_.
        
    
    You can filter the target accounts displayed on this page by region, bundle version, and NetSuite version. See [Filtering on Bundle Install Base Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_96103016312.html) and [Filtering Managed Bundle Install Base by NetSuite Version](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4846913876.html).
    
4.  If you have deprecated the managed bundle to be upgraded, be aware of the following:
    
    -   The Initiate Upgrade page for the deprecated version of a managed bundle lists only the accounts that have not yet been upgraded to the replacement version. This page can be used to push maintenance fixes to accounts with the lagging bundle version.
        
    -   The Initiate Upgrade page for the replacement version of the bundle lists accounts with the deprecated version as well as accounts with the replacement version installed. This page can be used to upgrade accounts with the lagging bundle version to the newer version as well as push maintenance fixes to accounts that already have the newer version installed.
        
5.  Check the box in the **Include** column next to each account where you want to install the new version, or use **Mark All** and **Unmark All** to select accounts to upgrade.
    
6.  Click Upgrade.
    
    -   After you have initiated the upgrade, the Bundle Install Base shows the status of the upgrade in each account in the **Install Status** column
        
    -   At any time, you can click the **Cancel Pending Upgrades** button to prevent the upgrade of accounts with a status of **Pending**. When you click this button, a popup asks whether you are sure. When you confirm, a banner appears on the Initiate Upgrade page stating that cancellation of pending upgrades is in progress, until the cancellation is complete.
        

Important:

During an upgrade to a managed bundle, handling of data updates for custom lists, and for custom records that include data, depends on the option set for each of these objects on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the Bundle Builder. The default is to preserve target account object data, but the bundle author can also choose an option to replace target account object data with bundled object data. See [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).

Note:

You can update a managed bundle in accounts that have installed it, but you cannot install a bundle in other accounts unless you have administrator access. For more information, see [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html).

The user shown in the bundle audit trail as executing a managed bundle update in a target account is an arbitrary designation. The managed bundle update process selects a user in the target account employee list to be the entry in the **Installed By** column of the audit trail. This selection is the administrator that has the lowest internal ID.

After an upgrade of a managed bundle, the owner of the bundle is set to a random account administrator. This setting may not correspond to the administrator who originally installed the bundle. This behavior is intentional and should not cause issues.

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [Managed Bundles - Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3383397.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
-   [Phased Upgrade of Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384115.html)
-   [Filtering Managed Bundle Install Base by NetSuite Version](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4846913876.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
