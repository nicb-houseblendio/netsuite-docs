---
id: "section_N2495338"
type: "section"
title: "Bundle an SSP Application"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Bundle an SSP Application"
parent: "preface_1521816133"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495338.html"
anchors: []
sha256: "bb7ebcfeeb54247aa78840c291560bf1baba10e463616154a93bdb621397ea03"
---

After you've created an SSP Application record and uploaded its assets to the file cabinet, you can use the Bundle Builder in NetSuite to package the SSP application into a SuiteApp for distribution to other NetSuite accounts. For more information about creating a bundle, see [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html). If you don't want users in target accounts to edit SSP application files, you can lock the SSP application when you create the bundle.

Additional notes on bundling SSP applications:

-   SSP applications are listed in Step 3 of the Bundle Builder, where you select objects to include in the bundle.
    
-   When you select an SSP application here, the SSP Application record and all files in its file cabinet are included in the bundle.
    
-   When the bundle is installed in a target account, the full SSP Application record is copied there. All files are also copied to an application folder in the target account's file cabinet:
    
    **<Default Target HTML Hosting Root>: /SSP Applications/<Application Publisher>/<Application Name>**
    
-   As of 2019.1, when you update a bundle with an SSP application, script deployments aren't updated in the target account. That means, existing touch points aren't overwritten and the Log Level and Status fields are also not updated. You can see the Log Level and Status fields on the Script Deployment page.
    

### Related Topics

-   [SSP Application Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2490486.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)
-   [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1521816133.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
