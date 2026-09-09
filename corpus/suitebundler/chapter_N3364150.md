---
id: "chapter_N3364150"
type: "chapter"
title: "SuiteApp Creation and Distribution"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution"
parent: "book_N3363377"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html"
anchors: ["subsect_156839755912", "bridgehead_4852122809"]
sha256: "f0ec53a53bd3b0889d262ddaa258d1c3bb35bda7a0e056cc409b1368656d45c6"
---

Note:

SuiteBundler is still supported, but it will not be updated with any new features.

To take advantage of new features for packaging and distributing customizations, you can use the Copy to Account and SuiteCloud Development (SDF) features instead of SuiteBundler.

Copy to Account is an administrator tool that you can use to copy custom objects between your accounts. The tool can copy one custom object at a time, including dependencies and data. For more information, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

SuiteCloud Development Framework is a development framework that you can use to create SuiteApps from an integrated development environment (IDE) on your local computer. For more information, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).

The SuiteBundler feature enables packaging of customization objects or configuration settings into a bundle that can be installed in other NetSuite accounts. To create bundles, this feature must be enabled in your account, and you must have the SuiteApp Marketplace permission. For details about how bundles can be used and the objects they can include, see [Types of Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364548.html). Each bundle has a unique bundle ID that is used to identify it and differentiate it from other bundles.

Important:

Bundles are also known as SuiteApps.

The Bundle Builder walks you through the steps of creating bundles.

-   For details about this interface and the step-by-step instructions for creating a bundle, see [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html).
    
-   You can control the update process for your bundles by defining them as managed if the Managed Bundles feature is enabled in your account. See [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html).
    
-   SuiteCloud Development Framework (SDF) includes support for SuiteApp projects, self-contained, standalone projects that enable SuiteCloud Developer Network (SDN) members to develop and deploy SuiteApps to their NetSuite accounts. SuiteBundler is used to bundle and share SDF SuiteApps. You can create a bundle with all objects from an SDF SuiteApp project, without manually adding them in the Bundle Builder. For information about using SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).
    

After creating a bundle, you can set it up to be released to other accounts. See the following:

-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
    
-   [Sharing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385867.html)
    

You can publish user help content for the bundle in the NetSuite Help Center. See [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html).

You can use bundle copy and deprecate actions to implement a bundle versioning strategy. These actions provide increased flexibility and control of the development and release process. See [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html) and [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html).

Other NetSuite account users can install your bundle if you've shared it with them or made it public. You can also install the bundle in other accounts where you have administrator access. This type of installation is called a push. See [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html).

NetSuite tracks the details of accounts where each bundle is installed on the Bundle Install Base page. See [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html).

Note:

Before creating a bundle, consider your deployment strategy. For explanations of deployment-related terms and preferred deployment methods, see [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html).

## Distributing Bundles Through the SuiteApp Marketplace {#subsect_156839755912}

You can distribute your SuiteApp bundles through the SuiteApp Marketplace. The information for a SuiteApp listing on the SuiteApp Marketplace is synchronized from the Advanced Partner Center (APC) record, and includes graphics, overview, features, and publisher information. The First Released date is also listed. For more information about the SuiteApp Marketplace, see [SuiteApp Marketplace](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1540487155.html).

SuiteApp bundles are distributed through the SuiteApp Marketplace when they meet the following requirements:

-   The Advanced Partner Center (APC) record for the SuiteApp has completed the listing review and been approved.
    
    The APC record provides the information displayed to your users in the SuiteApp listing. Contact SDN to learn how to complete a listing review. For more information about the Advanced Partner Center role, see [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html).
    
-   The primary bundle ID in the APC record refers to an existing bundle.
    
    Note:
    
    Secondary and tertiary bundle IDs are not used for the SuiteApp Marketplace listing. If the primary bundle ID is not set in the APC record, the SuiteApp bundle is not listed in the SuiteApp Marketplace, even when the SuiteApp is listed on [SuiteApp.com](http://suiteapp.com/).
    
-   A Built for NetSuite (BFN) review has been completed.
    
    To find out how to complete a BFN review, see [Built for NetSuite Overview](http://www.netsuite.com/portal/developers/built-for-netsuite.shtml) and [BFN Verification Process](http://www.netsuite.com/portal/developers/built-for-netsuite/bfn-verification-process.shtml).
    

Important:

Although your users can view SuiteApp bundles on the SuiteApp Marketplace, they must install them from the Bundle Details page. When viewing the SuiteApp listing for your SuiteApp bundle, users can click **View SuiteApp** to view and install it from the Bundle Details page. For more information, see [Installing from the SuiteApp Marketplace](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539799323.html) and [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).

SuiteApp bundles that are distributed through the SuiteApp Marketplace also appear in bundle searches. For information about searching for bundles, see [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html) and [Choosing a Bundle to Install](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395426.html).

## Giving Users Dashboard Access to a SuiteApp {#bridgehead_4852122809}

You can give target account users access to your SuiteApps by including a Dashboard SuiteApp portlet script in your bundles. This type of script provides a dashboard component for your SuiteApp, a portlet that is available to users from the Personalize Dashboard menu when the bundle is installed in an account. This menu includes a SuiteApps option. Users can click this option for a quick view of installed SuiteApps with a dashboard component. These SuiteApps are represented by portlet icons in the Personalize Dashboard window. Each SuiteApp's icon is displayed with its branding graphics. A user can double-click or drag a SuiteApp portlet's icon to add a portlet to their dashboard that gives direct access to the SuiteApp.

To add this capability to a SuiteApp, you can create a SuiteScript 2.0 portlet script that provides custom content. You can upload a graphics file to be shown as the icon in the Personalize Dashboard window. On the script deployment record for the new portlet script, you should indicate that the script is designed for a dashboard SuiteApp portlet. And you can indicate the graphics file to be shown for the SuiteApp. For more information, see [SuiteScript 2.1 Portlet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799288.html) and [Guidelines for Creating a Dashboard SuiteApp Icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515621736.html).

After creating and editing the portlet script, include it in your SuiteApp. On the Select Objects page of the Bundle Builder, you can indicate the script should be included in the bundle. The graphics file selected for the icon is automatically included in the bundle with the script. In accounts where the bundle containing the new script is installed, users can add the SuiteApp portlet to their dashboards. For more information, see [SuiteApp Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4629724453.html).

Important:

Be aware that changes to an icon associated with a dashboard SuiteApp portlet are always copied during a bundle update. This overwrite of the icon in the target account occurs even if the bundle preference is set to prevent the update of script deployments.

### Related Topics

-   [SuiteBundler Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3363483.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Types of Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364548.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [SuiteCloud Plug-ins and Extensions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156026287422.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
-   [SuiteBundler Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3783020489.html)
-   [Custom Transaction Types in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4177814825.html)
-   [Adding a Custom Segment to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4520725557.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
