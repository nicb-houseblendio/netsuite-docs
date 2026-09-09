---
id: "section_N2494795"
type: "section"
title: "Select Supported Touch Points"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Select Supported Touch Points"
parent: "section_1529595280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html"
anchors: ["procedure_N2494815"]
sha256: "5dafc97e82ce2c1e18efe091bc118a79926f8b7c3a2ba299989d04f83019b68d"
---

An SSP application can contain customizations for one or more web store touch points. After you have uploaded SSP application files to the file cabinet, you can select the supported touch points on the SSP Application record and link them with the URL of the .ssp files that contain the customizations for each touch point. You can define parameters for each URL.

After selecting supported touch points on the SSP application record, you link your site or domain to one or more of the supported touch points by defining them on site and domain records.

Supported touch points include the following:

-   Log In
    
-   Log Out
    
-   Proceed to Checkout
    
-   Register
    
-   View Cart
    
-   View Customer Center
    
-   View Homepage
    

If you need to remove touch points from an SSP application or from a website, see [Remove Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753064405.html).

#### To select supported touch points on an SSP application: {#procedure_N2494815}

1.  Go to _Commerce > Hosting > SSP Applications_.
    
2.  Click **Edit** next to an SSP application.
    
3.  Click the **Supported Touch Points** subtab.
    
4.  Select each touch point in the **Name** column. The **Entry Page** column shows the URL that points to assets in the SSP application.
    
    ![Shows how to select supported touch points when editing an SSP application in the NetSuite interface.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/SystemManagement/SSPs/SSPAppTouchPoints_2015.2.png)
    
    Note the following:
    
    -   When installing a reference implementation, supported touch points are displayed by default.
        
    -   If you use the website preference, Password Protect Entire Site, then the Log In touch point must be associated with an .ssp file. Other file types, such as HTML will not display in the website when used in this context.
        
5.  In the **Entry Page** field, enter or select the page to be inserted at the selected entry point.
    
6.  Enter any URL parameters to be used.
    

All available touch points are displayed in the list. Note that some SSP applications are not compatible with every touch point. For more information about touch points available for specific reference implementations, see [Set Up SCA Developer Tools](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2673589.html).

After you have selected touch points for the SSP application, you can link the SSP application to your website. For more information, see [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html).

### Related Topics

-   [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html)
-   [Create a SuiteScript 1.0 SSP Application Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html)
-   [Upload SSP Application Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494548.html)
-   [Set Execute as Role Permissions for .ss and .ssp Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4589350481.html)
-   [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
