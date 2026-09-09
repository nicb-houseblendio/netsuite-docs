---
id: "section_N2493657"
type: "section"
title: "Create a SuiteScript 1.0 SSP Application Record"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Create a SuiteScript 1.0 SSP Application Record"
parent: "section_1529595280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html"
anchors: []
sha256: "8f5c47d4e77da7beded8b09d3163627d6bbaa9640d8b2a2fa783f28d709ac4e1"
---

The SSP Application record stores details about your website customization. This record enables you to group website assets, debug script files, and package your customization for use in other NetSuite accounts. You can define the following properties on the SSP application record:

-   The folder in the NetSuite file cabinet where your website customization assets are stored.
    
-   Supported touch points.
    
-   URL root used in website links to website assets.
    

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

#### To create an SSP application record:

1.  Do one of the following:
    
    -   Go to Customization > Scripting > SSP Applications > New.
        
    -   Go to _Commerce > Hosting > SSP Applications > New_.
        
    -   If at least one SSP Application folder already exists in your file cabinet, go to _Commerce > Hosting > Website Hosting Files_, select a website hosting folder, click New SSP Application, select an application publisher, and then continue on to create a new SSP Application record.
        
2.  Enter a **Name** for the SSP application.
    
    This name is like a project name, and is used in NetSuite lists, for example, on the SSP Applications list page, and in the Bundle Builder. This name is not directly visible to web store users.
    
3.  (Optional) Enter an **ID**.
    
    This identifier is used for scripting purposes, for the SSP Application record to be called by a SuiteScript. If you do not enter a value, a default is provided, webapp###. This value cannot be edited after the SSP Application record is saved.
    
4.  Select the SuiteScript **Version** that has been used in the SSP application. This field is available only if you have enabled the ability to create SSP applications in SuiteScript 2.0.
    
    Warning:
    
    You cannot change the version after you have saved the SSP application record.
    
5.  Select an **Application Folder**. The list contains all SSP Application folders in the WebSite Hosting Files Folder. If you have enabled the ability to create SSP applications in SuiteScript 2.0, any application folders already assigned to SuiteScript 2 SSP applications are not displayed. Application folders that contain SuiteScript 2.0 scripts are also not displayed.
    
    You can also create a new application folder. For more information, see [Create an SSP Application Folder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4343918704.html).
    
6.  Review the **URL Root** and edit as desired.
    
    This is the base URL that is used to link to the SSP application from the web store and may be visible to web store users. See [The URL Root and its Components](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2491541.html) for more information.
    
7.  (Optional) Enter a **Description**.
    
    This is a description of the SSP application. The description is only displayed internally in NetSuite.
    
8.  Select a **Status**.
    
    Leave as the default of Testing while you are creating and debugging your SSP application. Set to Released after you have completed the SSP application and linked it to your website.
    
9.  (Optional) Select a **Log Level**.
    
    The value in this field determines the type of messages written to the script execution log for the SSP application. See [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html).
    
10.  (Optional) Select an **Owner**.
     
     Sets the owner of the SSP application. Default is the currently logged in user. After an SSP application is created, only the owner of the SSP application can modify it. The owner is different from the application publisher, as the owner refers to the individual user who is allowed to modify the SSP application record.
     
11.  Add library script files on the **Scripts** subtab.
     
     These are external files that are called from the SSP application's script files.
     
     -   Files in the SuiteBundles, SuiteScripts, and Web Site Hosting Files folders of your file cabinet can be selected as library files.
         
     -   After you add a library file to an SSP application, it can be referenced by any of the .ss or .ssp files in the SSP application.
         
     
     For more information, see [Upload SSP Application Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494548.html).
     
12.  Select **Supported Touch Points**.
     
     These are the pages where website visitors can interact with the SSP application. For more information, see [Select Supported Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html).
     

### Related Topics

-   [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html)
-   [Set Execute as Role Permissions for .ss and .ssp Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4589350481.html)
-   [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html)
-   [Remove Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753064405.html)
-   [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
