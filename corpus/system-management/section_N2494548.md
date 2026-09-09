---
id: "section_N2494548"
type: "section"
title: "Upload SSP Application Files"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Upload SSP Application Files"
parent: "section_1529595280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494548.html"
anchors: ["bridgehead_N2494042"]
sha256: "3e2bb5040e471f2a0ab23a21eb5f716bfd05e18f46220be95771d4bd727b8e0e"
---

After you have created an SSP application record, you can upload all of the scripts, images, and other assets for your web store customization to SSP application folder.

#### To upload assets to an SSP application folder:

1.  Go to _Commerce > Hosting > Website Hosting Files_.
    
2.  Select the Web Site Hosting Files folder you need, and then select the SSP Applications folder.
    
3.  Select the application publisher, and then the SSP application folder you want to work with.
    
    -   Create new folders as desired. For example, you might create subfolders in your SSP application folder for style sheets, images, javascript, and SuiteScript.
        
    -   Add files as desired.
        
    -   For more information about uploading files to the file cabinet, see [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html).
        

Note:

For SuiteScript developers, notice that you need to upload your .ssp and .ss files to your SSP Applications folder. You should not upload these files to the SuiteScript folder in the file cabinet.

## Using the include Tag instead of Library Files {#bridgehead_N2494042}

For .ssp files, NetSuite recommends that you use the **include** tag to reference scripts rather than listing them as library script files. Use one of the following formats:

          `<%@include file='file'%>, or <%@include file='/path'%>` 
        

When the path begins with /, it is always relative to the root folder of the SSP application; otherwise it refers to a file in the same folder as the referring asset. You cannot use the **include** tag to reference files outside of the SSP application.

### Related Topics

-   [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html)
-   [Create a SuiteScript 1.0 SSP Application Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html)
-   [Set Execute as Role Permissions for .ss and .ssp Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4589350481.html)
-   [Select Supported Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html)
-   [Remove Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753064405.html)
-   [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html)
-   [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
