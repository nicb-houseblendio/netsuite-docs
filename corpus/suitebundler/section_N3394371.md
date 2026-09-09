---
id: "section_N3394371"
type: "section"
title: "Resolving Conflicting Objects"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Resolving Conflicting Objects"
parent: "chapter_N3394134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html"
anchors: ["bridgehead_N3394388", "bridgehead_N3394425", "bridgehead_N3394469", "bridgehead_N3394491"]
sha256: "7f53c8d39d8e5c748a555d5e4345232f819dbe830a18204813c49d536b1544ea"
---

When you install a customization bundle, the objects in the bundle are checked against preexisting custom objects in your account to identify possible conflicts. In the same manner, when you update a previously installed customization bundle, any newly added bundle objects are checked against preexisting custom objects in your account. The results of this check are displayed on the Preview Bundle Install page or Preview Bundle Update page. When you review these pages, you'll see options for resolving these conflicts.

For managed bundles, you cannot override bundle installation preferences during bundle installation. For more information, see [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).

Important:

Updating bundles from sandbox to production works differently to meet the special needs of sandbox-developed bundles. See [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html).

Note:

Updating bundles from a development account to a sandbox account works the same as updating other bundles. The usual update process overwrites all target account objects with those from the source bundle. For updates from a development account to sandbox, the Preview Bundle Update page always shows the Update action for all objects, even if they haven't changed since the last update.

## How Conflicts Are Identified {#bridgehead_N3394388}

Conflicts happen when bundle objects have the same script IDs or names as existing objects in your account. Generally, a conflict exists for one of the following reasons:

-   The same object already exists in your account, usually because it was installed with another bundle.
    
-   A different, unrelated object coincidentally has the same ID or name.
    

NetSuite checks for conflicts first by script ID, or by name and type if there's no script ID. For example, custom fields, which have script IDs, are identified by their script IDs, whereas custom forms, which do not have script IDs, are identified by their form name and type.

Bundle authors can avoid conflicts by giving each custom object a name that's unique to its function in the bundle.

## Options for Resolving Conflicting Objects {#bridgehead_N3394425}

For each bundle object that is identified as conflicting, you can choose one of the following actions on the Preview Bundle Install page and Preview Bundle Update page:

-   **Add and Rename** the bundle object, leaving the preexisting custom object intact, or
    
-   **Replace Existing Object** with the bundle object.
    

Typically, you would choose Add and Rename if the conflicting ID or name is a coincidence, and you would choose Replace Existing Object if you are sure the bundle object and the preexisting object in the account are the same object. You can still choose Add and Rename even if the objects are the same, but this will create a duplicate object.

Installation of a bundle from a sandbox account to a production account almost always involves conflicting objects. In this case, you'd usually pick Replace Existing Object.

Warning:

For any bundle object conflict where the Preview Bundle Update page displays both a Delete action, and a dropdown to select either Add and Rename, or Replace Existing Object, a bundle update causes deletion of the object and removal of its data from the target account.

## Impact of Choosing Add and Rename {#bridgehead_N3394469}

If you choose to add and rename a bundle object, a number is appended to the bundle object's name or script ID, to differentiate it from the preexisting custom object. Additionally, all references to the custom object in SuiteScript change to reflect this renaming. For example, if the bundle includes a custom field with the ID **custentity\_deptaddr** and the target account has a custom field with the same ID, then the field in the bundle is given the ID **custentity\_deptaddr2**, and any of the SuiteScript code in your bundle that referenced custentity\_deptaddr2 is updated automatically to reference custentity\_deptaddr2 instead.

## Impact of Choosing Replace Existing Object {#bridgehead_N3394491}

For a custom field, choosing Replace Existing Object generally does not have any impact on data that has been entered to the existing field, if the bundle field has the same data type as the existing field. This option causes the field definition to be updated to match the definition for the bundled field. If the bundled field has a different data type, data may have to be deleted from the existing field because the bundled field type, for example, INTEGER, cannot store the existing type of data, for example, TEXT. In this case, you'd probably want to pick Add and Rename to create a new field and give it a unique script ID.

For custom records with data or custom lists, when you pick Replace Existing Object, you can set the bundle preference to Replace Data, Preserve Data, or Merge Data. The Replace Data option overwrites existing target account object data with bundle object data. The Preserve Data option, which is the default, preserves existing data in target account objects. The Merge Data option retains any data added to target account objects after bundle installation and at the same time updating data that was previously installed with the bundle. See [Set Bundle Installation Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html#bridgehead_N3396336) and [Set Bundle Update Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html#bridgehead_N3399815).

If you choose to replace a preexisting custom object with a bundle object, the bundle object keeps the same name or script ID, and the preexisting custom object no longer exists in the account. For example, if the bundle includes a custom field with the ID **custentity\_deptaddr** and the target account has a custom field with the same ID, then the field in the bundle keeps the ID **custentity\_deptaddr** and the preexisting custom field no longer exists in the account.

Warning:

If you choose the Replace Existing Object option for a conflicting object during bundle installation, the preexisting custom object is PERMANENTLY replaced by the bundle's object. Even if you choose to uninstall the bundle later, changes to the replaced object remain and the original object is not restored.

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html)
-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Reviewing the Preview Bundle Install Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html)
-   [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html)
-   [Uninstalling a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400972.html)
-   [Viewing the Bundle Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401188.html)
-   [Identifying Bundle Objects in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3401780.html)
-   [Filtering Bundle Objects on List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3402016.html)
-   [Reviewing the Preview Bundle Update Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html)
-   [Set Bundle Installation Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html#bridgehead_N3396336)
-   [Set Bundle Update Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html#bridgehead_N3399815)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
