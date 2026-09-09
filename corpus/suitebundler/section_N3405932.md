---
id: "section_N3405932"
type: "section"
title: "Sandbox Refresh Impact on Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApps and Sandbox Accounts > Sandbox Refresh Impact on Bundles"
parent: "chapter_N3405306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405932.html"
anchors: ["subsect_1517244125", "subsect_1517244495", "subsect_1517244524"]
sha256: "61683627f4eb69841e3875659374b0de9baf5835c49bd6636593d26818e037c7"
---

A refresh of a sandbox account overwrites the sandbox account contents with the related production account contents. The intent is that, after the refresh is complete, the sandbox account mirrors the related production account. However, the handling of bundles during refreshes may result in some differences between bundles in the sandbox account and bundles in the production account.

A sandbox refresh has the following impacts on bundles:

-   A bundle definition for a bundle created in a sandbox account may not be preserved in the sandbox account after a refresh.
    
    -   If the bundle was installed in the related production account before a refresh, NetSuite maintains the bundle definition in the sandbox account after the refresh. NetSuite also maintains the link between the bundle's source and target accounts.
        
    -   If the bundle was not installed in the related production account before a refresh, the bundle definition is not maintained in the sandbox account after the refresh.
        
    -   You also must take steps to preserve any changes made to a sandbox account between the latest production snapshot at the time of the refresh request and the time the refresh is activated. See [Preserving Changes Made to Sandbox Accounts During the Refresh Process](#subsect_1517244125).
        
        Warning:
        
        Bundles developed in sandbox accounts should be used only for account customizations in linked production accounts. A refresh of a sandbox account used as a source for bundle installation may result in broken bundle operation in target accounts other than the linked production account. To avoid this issue, do not install bundles in your production account from sandbox accounts other than your own. And do not allow installation of bundles developed in your sandbox account to others' production accounts.
        
-   A bundle definition created in production before a refresh isn't transferred to the related sandbox during a refresh.
    
    -   The bundle definition is NEVER transferred from production to sandbox because a bundle can have only one source account. If the bundle definition were transferred from production to sandbox during a refresh, both production and sandbox accounts would be a source account of this bundle. You can't have more than one source account for a single bundle.
        
    -   This type of bundle will not be listed on the Saved Bundles page in the sandbox account after a refresh. The Saved Bundles page in a sandbox account only lists bundles that were recreated, that have a bundle definition in the sandbox account. The Installed Bundles page lists all bundles installed from other accounts into the sandbox account, including bundles copied to the sandbox account as part of a refresh.
        
-   If any objects from a bundle created in a sandbox are deleted from the corresponding bundle in the production account, when the sandbox account is later refreshed, these deletions have an impact on the bundle in the sandbox account. As part of the refresh, the objects that were deleted in production are deleted from the sandbox account, and are removed from the sandbox bundle definition
    

Warning:

After a sandbox account has been refreshed from production, it cannot be restored to its prior state. For more information about sandbox accounts, see [NetSuite Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N333400.html). For more information about sandbox refreshes, see [Using the Sandbox Accounts Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N333997.html).

Support for bundle operations varies across the different types of NetSuite accounts, including sandbox accounts. See [Bundle Support Across Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4853873261.html).

## Preserving Changes Made to Sandbox Accounts During the Refresh Process {#subsect_1517244125}

Before you activate a sandbox refresh, make sure you save any changes made to the sandbox during the refresh process. These updates will not be included in the newly activated sandbox. The contents of a refreshed sandbox are based on the latest snapshot of production account contents captured prior to the refresh request. For more information about sandbox refresh processing, see [Requesting a Refresh](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4177890138.html).

Warning:

As the bundle author, make sure your users don't install any bundles from sandbox during the refresh process. This applies to your customers or users at your company. Users installing bundles from the sandbox can later result in incorrect merging of different objects. To change bundle availability for your users, see [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html).

There are two options available to preserve sandbox account changes:

-   You can import updated sandbox account objects to a SuiteCloud project before activating the new sandbox. After activation, you can use SDF to deploy the updated objects to the new sandbox. This action is the preferred preservation method. For details, see [Using SDF to Preserve Sandbox Account Changes](#subsect_1517244495).
    
-   You can bundle updated sandbox account objects and install them in the related production account before activating the new sandbox. After activation, you can use SuiteBundler to install the updated objects to the newly activated sandbox account. For details, see [Using SuiteBundler to Preserve Sandbox Account Changes](#subsect_1517244524).
    

Warning:

Do not click the **Activate** button for the sandbox refresh until you have taken action to preserve all of the objects that have been updated during the refresh process. Otherwise the updates to these objects will be lost after the new sandbox is activated. You can preserve changes through import to a SuiteCloud project, or through bundling and installation in the related production account. If there have not been any updates since the refresh request was initiated, no preservation action is needed.

### Using SDF to Preserve Sandbox Account Changes {#subsect_1517244495}

SDF users can import updated sandbox account objects into a SuiteCloud project before the activation of a sandbox refresh, and then deploy those objects to the sandbox account after the refresh has been activated.

Follow these steps to use SDF to preserve sandbox account changes:

1.  When you receive the email notification that the sandbox refresh is ready to be activated, identify the changes that were made since the initiation of the refresh request.
    
    The changes are those you have made since the snapshot timestamp. To view the snapshot timestamp, go to _Setup > Company > Sandbox Accounts_. The snapshot timestamp is located in the **Snapshot Date** field.
    
2.  Preserve the changes by importing the desired custom objects into a SuiteCloud project. See [Account Component Imports to SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4702656511.html).
    
3.  Activate the sandbox refresh. See [Requesting a Refresh](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4177890138.html).
    
4.  After the sandbox refresh has completed, deploy the custom objects from the SuiteCloud project to the refreshed sandbox account. See [Deployment Logs for SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4715369474.html).
    

### Using SuiteBundler to Preserve Sandbox Account Changes {#subsect_1517244524}

You can preserve updated sandbox account objects by packaging them in a bundle and installing the bundle to a related production account before activating the refresh. Later you can install the objects into the sandbox account after the refresh has been activated.

Follow these steps to use SuiteBundler to preserve sandbox account changes:

1.  When you receive the email notification that the sandbox refresh is ready to be activated, identify the changes that were made since the initiation of the refresh request.
    
    The changes are those you have made since the snapshot timestamp. The snapshot timestamp is included in the email notification.
    
2.  Bundle the updated sandbox objects that you have identified and install the bundle into a related production account. See [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html), [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html), and [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).
    
3.  Activate the sandbox refresh (see [Requesting a Refresh](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4177890138.html)).
    
4.  After the sandbox refresh has completed, bundle the updated objects from production and install the bundle into the refreshed sandbox account.
    

### Related Topics

-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
-   [Single Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405732.html)
-   [Two Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405828.html)
-   [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html)
-   [Dissolving Bundles Created in Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770244609.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
