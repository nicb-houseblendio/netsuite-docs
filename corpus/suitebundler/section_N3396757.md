---
id: "section_N3396757"
type: "section"
title: "Bundle Installation Notes"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Installing a Bundle > Bundle Installation Notes"
parent: "section_N3395142"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396757.html"
anchors: ["bridgehead_N3396769", "bridgehead_N3396848", "bridgehead_N3396860", "bridgehead_N3396880", "bridgehead_1557476077", "bridgehead_4619493064", "bridgehead_1537206984", "bridgehead_1540479278"]
sha256: "45df4e584a580aa141b9f8513552eb7eeb565bf3534c1cefd4277dc6806b8a28"
---

You should know the following before you install a bundle in your account.

## Difference in NetSuite Versions for Source and Production Accounts {#bridgehead_N3396769}

During phasing of a new NetSuite release, bundles developed with the lagging version of NetSuite can be installed into accounts that are already using the leading version. Also, bundles developed with the leading version can be installed into accounts that are still using the lagging version, but be aware of the following limitations:

-   When a user in a lagging version account installs a bundle from a leading version account, any object types in the bundle that are not supported in the lagging version are not installed, resulting in potentially serious impact to bundle function.
    
-   A bundle with a SuiteScript that uses a new API available only in the leading version can be installed into a lagging version account, but the script may not function correctly because the lagging version does not support the API.
    

## Restrictions for Release Preview Account Bundles {#bridgehead_N3396848}

Be aware that there are limitations on the types of accounts from which you can install bundles into Release Preview accounts. For more details, see [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).

## Pushed Installations {#bridgehead_N3396860}

Bundle authors with administrator access to your account may install bundles directly without any actions required by you. See [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html).

Important:

The **Push** action isn't available in sandbox accounts. If a bundle author wants to install a bundle from a sandbox account to your account where they have admin access, they'll need to log in to your account to search for and install the bundle, or you can do it yourself.

## Bundled Server SuiteScripts {#bridgehead_N3396880}

If an installed bundle includes server SuiteScripts, you might not be able to view the script files, depending on whether the bundle's creator enabled an option in the script file's File Cabinet record to hide it in bundle installations. You can see the file records for hidden scripts, but you cannot open their .js files to view their contents.

If an installed bundle contains SuiteScripts and there are object conflicts, choosing to add and rename bundle objects requires that the script id references are encapsulated in quotes (" or ') so that the references are correctly renamed in the scripts. For information about the impact of the operation, see [Choose Actions for Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html#bridgehead_N3399684) and [Impact of Choosing Add and Rename](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html#bridgehead_N3394469).

## Bundle with SSP Applications {#bridgehead_1557476077}

As of 2019.1, when you update an installed bundle that includes an SSP application, the script deployments are not updated in the target account. Because script deployments are not updated, the existing touch points are not overwritten and both the Log Level and Status fields are also not updated in the target account. You can view the Log Level and Status fields on the Script Deployment page.

## Impact of Language Preferences on Bundled Custom Forms {#bridgehead_4619493064}

When a bundle that includes a custom form with sublists showing data from custom child records is installed in a target account with a different language preference than used in the source account for the bundle, the labels for the sublists may not be translated correctly. The system attempts to obtain the translations of labels in the language of the target account, but if these translations don't exist, the translated name of the child record type is used instead. A workaround is to manually rename sublists on the custom form in the target account, but when the bundle is updated, these manual changes will be overwritten. Another workaround is to change the language preference of the target account to be the same as the source account.

## Updates Required for Some Bundle Objects that Reference Custom Segments {#bridgehead_1537206984}

The unified ID has an impact on bundled objects. When the Use as Field ID setting is enabled for custom segments, existing customizations that include these segments may not work as expected. Objects that may be impacted include scripts, workflows, custom Advanced PDF/HTML templates, and saved searches. As of 2019.1, creating a new custom segment automatically uses the unified ID, and the **Use as Field ID** box is not visible. For more information, see [Creating a Custom Segment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4313465979.html).

To make sure bundled objects that reference custom segments install successfully, follow these guidelines:

| Source Account | Target Account | Installation Notes |
| --- | --- | --- |
| Custom segment objects created in a NetSuite version prior to 2019.1 | Custom segment objects created in a NetSuite version prior to 2019.1 | If the Use as Field ID setting is enabled on the segment in the source account, ensure that the objects in the bundle's target account are updated to reference the unified ID for the segment. |
| Custom segment objects created in NetSuite version 2019.1 or later | Custom segment objects created in a NetSuite version prior to 2019.1 | The Use as Field ID setting is enabled on the segment in the source account. Ensure that the objects in the bundle's target account are updated to reference the unified ID for the segment. |
| Custom segment objects created in a NetSuite version prior to 2019.1 | Custom segment objects created in NetSuite version 2019.1 or later | The Use as Field ID setting is enabled on the segment in the target account and cannot be changed. If the Use as Field ID setting was not enabled on the source account and **Replace Existing Object** selected to resolve the conflict, existing customizations that include those segments may stop working or may not work as expected. Objects that may be impacted include scripts, workflows, printing templates, and saved searches. |
| Custom segment objects created in NetSuite version 2019.1 or later | Custom segment objects created in NetSuite version 2019.1 or later | The Use as Field ID setting is enabled on the segment in both the source account and the target account. No change is needed. |

## Default Values for CSV Files {#bridgehead_1540479278}

When a bundle includes CSV files, you might need to manually map default values using the Import Assistant after installing the bundle. For more information, see [Including Import Maps and CSV Files in SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html).

### Related Topics

-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)
-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Choosing a Bundle to Install](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395426.html)
-   [Reviewing the Preview Bundle Install Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html)
-   [Starting the Bundle Installation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396567.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
