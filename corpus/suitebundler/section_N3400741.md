---
id: "section_N3400741"
type: "section"
title: "Using Managed Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Using Managed Bundles"
parent: "chapter_N3394134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html"
anchors: ["bridgehead_N3400819", "bridgehead_N3400850", "bridgehead_4798497171", "bridgehead_4779618604"]
sha256: "43b10688d2b62f2f968ad98c08fbcd43719092307e464acbfb95300457187bd3"
---

Managed bundles support automated updates by solution providers. Because the solution provider is responsible for the bundle update process, you do not have to take any action to ensure that a managed bundle installed in your production account is always the most up-to-date version.

The list of installed bundles, at Customization > SuiteBundler > Search & Install Bundles > List, has a Managed column that indicates which bundles are managed.

![Installed Bundles page with Managed column highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/ManBundleColumn.png)

You cannot manually update a managed bundle installed in a production account by selecting the Update option in this page's Action menu. Managed bundle updates are pushed into your account at the discretion of the solution provider.

In addition, you cannot override the managed bundle object preferences set by the solution provider. If a non-managed bundle installed in your account later becomes managed, all preferences previously selected in your account are ignored during bundle updates. See [Set Bundle Installation Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html#bridgehead_N3396336) and [Set Bundle Update Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html#bridgehead_N3399815).

## Installing a Managed Bundle {#bridgehead_N3400819}

You can install a managed bundle in the same way that you install any other bundle in your account, but before you proceed with installation, you are presented with a popup message. This message informs you that by installing the bundle, you are giving the solution provider permission to install future updates at any time.

![Confirmation message to install a SuiteBundle.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/Bundler_managedBundle_agreementDialog.png)

## Updating a Bundle that was Converted to Managed {#bridgehead_N3400850}

In some cases, a bundle may not be a managed bundle when you first install it, but later is converted to be a managed bundle. In this case, the next time you click **Update**, you are informed that the bundle is now a managed bundle, and you must agree to let the solution provider manage future bundle updates before you can update the bundle. If you don't want the managed bundle anymore, you can uninstall it and you won't get any more upgrades.

## User for Managed Bundle Update Audit Trail {#bridgehead_4798497171}

The user shown in the bundle audit trail as executing a managed bundle update in your account is an arbitrary designation. The managed bundle update process selects a user in the employee list to be the entry in the **Installed By** column of the audit trail. This selection is the administrator that has the lowest internal ID.

## Managed Bundle Upgrade Notifications to Target Account Users {#bridgehead_4779618604}

SuiteBundler sends email notifications of managed bundle upgrades to target account users. Email recipients can be designated on the Bundle Details page.

When a managed bundle is successfully upgraded in your account, an email message containing the bundle name, bundle ID, bundle version, and account ID is sent. No message is sent when an upgrade fails.

The recipients for this email message are based on the **Email Recipients** setting on the Messages subtab of the Bundle Details page in your account. The default choice is **All Bundle Admins**, indicating that all administrators and users with the SuiteApp Marketplace permission in the account are recipients. A choice of **None** opts out of receiving this email. A choice of **Custom** allows the entry of specific users to receive the email.

Note:

The **Email Recipients** setting applies to all bundle messages, not only managed bundle upgrade notifications. For more information, see [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html).

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html)
-   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
