---
id: "chapter_N2490486"
type: "chapter"
title: "SSP Application Overview"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > SSP Application Overview"
parent: "preface_1521816133"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2490486.html"
anchors: ["bridgehead_N2491060", "bridgehead_N2490559"]
sha256: "0101832d4b2119247dc70e657817955894b37bf81be0f580c191a1f7702f9965"
---

SuiteScript Server Pages (SSP) is the custom web application platform you use to build applications for Commerce web stores. SSP applications are an iteration on the Suitelet, letting you build frontend pages that run server-side SuiteScript to generate dynamic content. The technology emulates JSP, but uses SuiteScript as the underlying mechanism. You can also bundle and distribute SSP applications as SuiteApps, making it easier to share or sell custom applications.

SSP applications include .ssp files and a library of JavaScript files. The .ssp files make AJAX calls to backend services and keep frontend (website display) and backend (business) logic separate.

Every SSP application has entry points you can connect to different parts of your web store. The entry points for an SSP application depend on the SuiteScript version it uses. For SSP applications written in:

-   **SuiteScript 1.0**: Entry points (or touch points) are set as Supported Touch Points on the SSP application record. Each touch point matches a part of the web store, such as View Homepage, Log In, and Log Out. When a user goes to a certain part of the store, the connected SSP application runs and generates dynamic content for that area.
    
-   **SuiteScript 2.0**: The default SSP file selected on the SSP application record is the single entry point.
    

All files in an SSP application are grouped by author (application publisher) and stored together in Web Site Hosting files folder in the files cabinet.

The SuiteScript Server Pages feature works for both Site Builder and Commerce websites. This feature lets you package Commerce website assets as SSP applications. You can create SSP applications and link them to your website to customize it.

For more information, see [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html).

## SSP Application Structure {#bridgehead_N2491060}

SSP files (.ssp) are user interface elements on a website. They can generate anything from a banner to a whole web page. A .ssp file has the presentation logic for the web page it replaces. These .ssp files let you to add HTML and generate dynamic content to show in the browser.

An important job of .ssp files is to generate dynamic content for supported web store touch points. SSP applications written in SuiteScript 1.0 support several touch points and you can select a different .ssp file for each one. In SuiteScript 2.0 SSP applications, the default .ssp file decides which .ssp file to use for each purpose.

Backend services go in .ss files, usually one .ss file per service. Ajax calls from an .ssp file let you access .ss file services. Note that besides the SuiteScript API, both .ssp and .ss files can use the Commerce API. For more information, see [File Types for SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491273.html#bridgehead_N2491667).

## SSP Applications and Commerce web stores {#bridgehead_N2490559}

Commerce web store is a website and checkout solution delivered as a set of SSP applications, available as a SuiteApp you can install in your account. You can modify, test, and debug files for SSP applications in your NetSuite account. This setup lets you to manage multiple SSP applications to customize a single web store. SSP applications ensure that all assets are linked together. This setup also supports access with named URLs.

### Related Topics

-   [Components of SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491273.html)
-   [SSP Applications Compared to Customization with SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4390440744.html)
-   [SSP Applications (SuiteScript 1.0 Compared with SuiteScript 2.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1529593660.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)
-   [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [Bundle an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495338.html)
-   [SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1521816133.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
