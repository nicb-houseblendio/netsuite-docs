---
id: "section_N3401188"
type: "section"
title: "Viewing the Bundle Audit Trail"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Viewing the Bundle Audit Trail"
parent: "chapter_N3394134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html"
anchors: ["bridgehead_N3401308"]
sha256: "7bda0e775a64dc4c4b416a4aa61208e86f09dd3e2e60e976bd68b4c80a3fed34"
---

NetSuite supports tracking of all bundle installations, updates, and bundle uninstallations in your account. These actions are recorded on the read-only Bundle Audit Trail page, available at _Customization > SuiteBundler > Bundle Audit Trail_.

Audit trail results are always sorted in reverse chronological order, starting with the most recent action. You can filter the results by Action, Bundle ID, User, and time interval and you can export these results to a CSV file.

As of 2017.1, the SuiteBundler Audit Trail permission provides access to the Bundle Audit Trail page, but not to other SuiteBundler tasks. Prior to this release, the SuiteApp Marketplace permission was required to see the Bundle Audit Trail page. The SuiteBundler Audit Trail permission is useful for auditors. This permission includes only one level, Full. This level is required to view the Bundle Audit Trail page. Users without this permission can't access the page. By default, all account administrators have this permission.

![Bundle Audit Trail page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleAuditTrail.png)

The following table describes the bundle audit trail columns:

| Column Name | Description |
| --- | --- |
| Bundle ID | Unique system-defined identifier for the bundle. |
| Name | Name for bundle. Defined by the bundle author. |
| Version | Version number for bundle. Defined by the bundle author. |
| Action | Action performed by the bundler. Includes the following actions: Install, Update, Uninstall, or Managed Upgrade for managed bundles. |
| Start Date | Date and time the bundle action began. Note: The date and time value is hardcoded to Pacific Time Zone and does not reflect the time zone setting on Home > Set Preferences. |
| End Date | Date and time the bundle action ended. Note: The date and time value is hardcoded to Pacific Time Zone and does not reflect the time zone setting on Home > Set Preferences. |
| Status | Success or failure of the bundle action. |
| User | Name of the user who performed the bundle action. |
| Source | Location from which bundle was installed or updated. |
| Notes | Additional bundle details. For example, a bundle that replaces a deprecated bundle displays 'Deprecated bundle <bundle\_ID>. |
| Error Reference | The internal error database number for any error that occurs during bundle installation, update, or uninstallation. You can provide this number to NetSuite Customer Support when troubleshooting a failed bundle installation, update, or uninstallation. |

## Bundle-Specific Audit Trail {#bridgehead_N3401308}

The **Audit Trail** subtab of each Bundle Details page tracks installations, updates, and uninstalls of that specific bundle. This information can be filtered by **Action**.

![Bundel Details page with Audit Trail subtab displayed.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleAuditTrailSubtabNew.png)

Note:

The Bundle Audit Trail is available to account administrators and to other users with the SuiteApp Marketplace permission.

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
-   [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
-   [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
