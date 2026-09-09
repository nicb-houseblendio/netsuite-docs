---
id: "section_N2496052"
type: "section"
title: "Change SSP Application Precedence"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Change SSP Application Precedence"
parent: "section_1529595280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html"
anchors: ["procedure_N2491576", "procedure_N2496083"]
sha256: "ff8a418fa73452eb61d40a5f57125bd7f887364ef8d7d281ce9d463778b86cfd"
---

SSP applications allow you to store multiple website customizations in one account, including customizations for the same web store touch point. When a URL refers to an asset in multiple SSP applications, a system of precedence determines which SSP application handles a particular request.

## Precedence for SSP Application Assets {#procedure_N2491576}

Each SSP application has a precedence sequence number, such as 1, 2, 3, 4, and so on. The lower the precedence number, the higher the application precedence. Files within an SSP application of higher precedence are used first.

Be default, newer SSP applications take precedence over existing SSP applications when added to an account. However, you can change the precedence of any SSP application in NetSuite.

For example, you install an SSP application. Because this is the latest addition, it bears a precedence of 1 by default. Any files within this application take a higher precedence over files within SSP application folders with a precedence of 2, 3, 4, and so on. You can configure NetSuite to change this precedence at any time.

#### To change SSP Application precedence: {#procedure_N2496083}

1.  Go to Customization > Scripting > SSP Applications.
    
2.  Click the **Change Precedence** button.
    
    ![Shows how you can change SSP application precedence in the NetSuite interface.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/SystemManagement/SSPs/WebAppChangePrecedence.png)
3.  Change numbers in the **Precedence** column as desired and click **Submit**.
    

### Related Topics

-   [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html)
-   [Create a SuiteScript 1.0 SSP Application Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html)
-   [Upload SSP Application Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494548.html)
-   [Set Execute as Role Permissions for .ss and .ssp Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4589350481.html)
-   [Select Supported Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html)
-   [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html)
-   [Remove Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753064405.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
