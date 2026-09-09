---
id: "section_N2495714"
type: "section"
title: "Link a Website or Domain to an SSP Application"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Link a Website or Domain to an SSP Application"
parent: "section_1529595280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html"
anchors: ["procedure_N2495730", "bridgehead_3909504552"]
sha256: "a5fed1d19b265a593af28f2580ea82effe4da4ea027a94feca15c96c75c2a197"
---

Your website is linked to an SSP application when touch points are defined on the Web Site Setup page. After linking the website to an SSP application a URL is generated that points to assets in the SSP application for each supported touch point. You can use all the touch points supported by an SSP application, or only some of them.

You can also link a domain to an SSP application. In this way, your website customization is associated with a specific domain. For more information, see [Link a Domain to an SSP Application](#bridgehead_3909504552).

Note:

Touch points configured for a domain override the touch points configured for the related web site. However, if you are linking a domain to an SSP application, you must also define touch points on the web site record; domain-only touch point configuration is not supported.

#### To link your site to an SSP application: {#procedure_N2495730}

1.  Do one of the following:
    
    -   Go to Customization > Scripting > SSP Applications > New.
        
    -   Go to _Commerce > Hosting > SSP Applications > New_.
        
2.  On the list page, click **Edit** next to the SSP application you want to use on your website.
    
3.  Verify that some **Supported Touch Points** are selected. For more information, see [Select Supported Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html).
    
4.  Click the arrow in the **Save** button. Choose **Save & Link to Site**.
    
5.  Select a site on the **Link Site To SSP Application** page.
    
    Note:
    
    You can only link an SSP application to a website that has the same hosting root as the SSP application. For example, if you created an SSP application in the Staging Hosting Files folder, then you cannot link that SSP application to a website in the Live hosting root.
    
6.  Click **Save**.
    

The touch points selected on the SSP Application record are listed on the Touch Points subtab of the Web Site Setup page, indicating the SSP application is live on the website. Note that you must complete additional setup tasks when installing a reference implementation. For more information, see [Set Up SCA Developer Tools](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2673589.html).

Important:

You should first try linking your website to an SSP application in a sandbox account or another test site.

## Link a Domain to an SSP Application {#bridgehead_3909504552}

You can link a domain to supported touch points to create a unique web store experience for that domain. For example, you may want a certain look and feel for an entry point to your site using a certain domain.

#### To link a domain to an SSP application:

1.  Follow Steps 1 - 4 in [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html).
    
2.  Click **Save and Link to Domain**.
    
3.  Select a domain on the **Link Domain To SSP Application** page.
    
    Note:
    
    You can only select a domain that is pointing to the same hosting root as the SSP application. For example, you cannot deploy an SSP application created in the Staging Hosting files folder to a domain pointing to the Live Hosting Files folder.
    
4.  Click **Save**.
    

Alternatively, you can click the Link to Domain button when the SSP application record is in view mode. To verify the domain is linked to the SSP application, visit the Domains subtab on the Web Site Setup page to confirm that you see the same supported touch points that exist on the SSP application.

See also, [Select Supported Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html), and [Remove Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753064405.html).

### Related Topics

-   [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html)
-   [Create a SuiteScript 1.0 SSP Application Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html)
-   [Upload SSP Application Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494548.html)
-   [Set Execute as Role Permissions for .ss and .ssp Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4589350481.html)
-   [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
