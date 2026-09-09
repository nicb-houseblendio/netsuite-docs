---
id: "section_N3400972"
type: "section"
title: "Uninstalling a Bundle"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Uninstalling a Bundle"
parent: "chapter_N3394134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html"
anchors: ["procedure_N3400999"]
sha256: "d6cee292ccca0e7355e7d494b8136250993e7f38adecb5f8190ae8a80c05819c"
---

You can uninstall a customization bundle at any time after installing it.

You cannot uninstall a configuration bundle. For more information, see [Configuration Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html).

Uninstalling a managed bundle stops all upgrades to that bundle in your account.

Warning:

Uninstalling a bundle may result in data loss. When you uninstall a customization bundle, all objects included in that bundle, including any data in these objects, are deleted. Additionally, any custom records you created from the custom record types in the bundle are deleted. To avoid potential data loss, do not uninstall the bundle.

#### To uninstall a bundle: {#procedure_N3400999}

1.  Log in to the account in which you installed the bundle.
    
2.  Go to _Customization > SuiteBundler > Search & Install Bundles > List_.
    
3.  Choose **Uninstall** from the **Action** dropdown list for the bundle you want to uninstall.
    
4.  In the confirmation popup, click **OK**.
    

NetSuite deletes the bundle, and the bundle's customization objects, from your account. Be aware of the following objects that are exceptions: objects referenced by other bundles installed in the account, and objects that were set to replace an existing object during bundle installation are not deleted.

Warning:

If when you installed this bundle, you set objects in the bundle to **Replace Existing Object**, then these objects cannot be uninstalled with this procedure. After uninstalling the bundle, the objects that you replaced remain in your account in the same configuration as they were in after installation.

**Note about Uninstalling Bundled Custom Records Used for Workflows**

The following changes are made to workflows related to a custom record type installed as part of a bundle when that bundle is uninstalled:

-   The bundle uninstall deletes any workflows that have been deployed to that record type.
    
-   The bundle uninstall deletes any actions that point to that record type but are deployed to different record type. (Note that in these cases, the actions are deleted, but not the workflows.)
    

After a bundle uninstall, you should review your workflows for possible changes.

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
-   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
