---
id: "section_N2675216"
type: "section"
title: "Install Your Commerce Website Applications"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Getting Started > Install Your Commerce Website Applications"
parent: "section_N2655840"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2675216.html"
anchors: []
sha256: "01cb576247b1264fd1c84c4714444e40e8796ca6e4a330b5bf71d900818744f5"
---

When you're installing Commerce website applications for the first time, you'll need to install the latest version of the appropriate SuiteApp (bundle) and any other related SuiteApps you need. This process creates or installs records and files into your NetSuite account that are necessary to host your website.

Note:

Before you get started, you'll need to set up one or more domains for your Commerce website, enable features, and set your site preferences. See [Getting Started](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2655840.html) for more information.

#### To install your SuiteCommerce application:

1.  Go to Customization > SuiteBundler > Search & Install Bundles.
    
2.  Install all SuiteApps (bundles) required for your implementation.
    
    In the **Keywords** field, enter the Bundle ID of the version of the SuiteApp you want to install and click **Search**. See the following table for a list of SuiteApps and their Bundle IDs. Contact your NetSuite representative if you don't have access to shared SuiteApps.
    
    Note:
    
    Most Commerce SuiteApps are managed, and you automatically receive updates for fixes and enhancements for that SuiteApp without any need to update manually or migrate for future releases. But some SuiteApps, like SuiteCommerce Advanced, aren't managed and need you to update them manually.
    
    | SuiteApp | Bundle ID | Application | Required/Optional | Managed? | Shared? |
    | --- | --- | --- | --- | --- | --- |
    | SuiteCommerce | 596070 | 
    -   SuiteCommerce
    -   SuiteCommerce MyAccount
    
     | Required | Yes | Yes |
    | SuiteCommerce Advanced 2026.1.20 | 596543 | SuiteCommerce Advanced | Required | No | Yes |
    | SuiteCommerce Configuration | 381166 | 
    
    -   SuiteCommerce
    -   SuiteCommerce MyAccount
    -   SuiteCommerce Advanced
    
     | Required | Yes | No |
    | SuiteCommerce Extension Management | 582380 | 
    
    -   SuiteCommerce
    -   SuiteCommerce MyAccount
    -   SuiteCommerce Advanced
    
     | Required Important: You must install this SuiteApp before installing any theme or extension bundles. | Yes | Yes |
    | SuiteCommerce Base Theme | 596199 | 
    
    -   SuiteCommerce
    -   SuiteCommerce MyAccount
    -   SuiteCommerce Advanced
    
     | Required Note: You must activate a theme for a domain. You can activate only one theme per activation/domain at a time, but you can activate the same theme across multiple domains. There are other themes available to you. For details, see [Available Commerce Themes and Supported Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158695491035.html). | Yes | Yes |
    | SMT Core Content Types | 190323 | 
    
    -   SuiteCommerce
    -   SuiteCommerce Advanced
    -   Site Management Tools
    
     | Required Note: The following caveats apply to this bundle:
    
    -   For SuiteCommerce and SuiteCommerce Advanced 19.1 or later, the SMT Core Content Types bundle is automatically updated. Automatic updates are not available for SuiteCommerce Advanced 18.2 or earlier. You must contact professional services to upgrade to a newer version of SuiteCommerce Advanced or to SuiteCommerce.
    -   You must have SuiteCommerce or SuiteCommerce Advanced 19.1 or later installed to have access to the Enhanced Merchandising Zone. See [Merchandising Zone Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159561426850.html).
    
     | Yes | Yes |
    | Product Merchandising | 48476 | 
    
    -   SuiteCommerce
    -   SuiteCommerce Advanced
    
     | Optional Install this SuiteApp if you want to use Merchandising Zones. | No | Yes |
    | Reference Product Lists Records | 53051 | 
    
    -   SuiteCommerce
    -   SuiteCommerce Advanced
    
     | Optional Install if implementing Product Lists or Save-for-Later lists. For details on using Product List Records, see [Product List Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3957635745.html). | Yes | No |
    | SC Google Tag Manager Editor | 250341 | 
    
    -   SuiteCommerce
    -   SuiteCommerce Advanced
    
     | Optional Install if implementing Google Tag Manager. For details on using SuiteCommerce Google Tag Manager Editor, see [Google Tag Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4546835898.html) | Yes | No |
    | Reference Product Review Records | 53053 | 
    
    -   SuiteCommerce
    -   SuiteCommerce Advanced
    
     | Optional Install if implementing Product Reviews. For details on using Product Review Records, see [SuiteCommerce Product Reviews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3844716106.html). | Yes | No |
    
3.  Verify that the correct SuiteApp is returned in the search and select it.
    
4.  Review the SuiteApp details and then click **Install**.
    
    Note:
    
    The **Installed Bundles** page displays a list of SuiteApps. Installation of a SuiteApp might take some time. The status column indicates the progress. Refresh the page to update the status.
    

When you've completed installing all SuiteApps required for your needs, it's time to point your website application to a domain. See [Link Your Commerce Applications to a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157970772311.html) for details.

### Related Topics

-   [Getting Started](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2655840.html)
-   [Enable Features and Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656144.html)
-   [SuiteCommerce Roles and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_8115751901.html)
-   [Link Your Commerce Applications to a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157970772311.html)
-   [Prepare the Web Site Setup Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2675493.html)
-   [Next Steps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1520191430.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
