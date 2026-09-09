---
id: "section_N2491273"
type: "section"
title: "Components of SSP Applications"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > SSP Application Overview > Components of SSP Applications"
parent: "chapter_N2490486"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491273.html"
anchors: ["bridgehead_N2491374", "bridgehead_N2491424", "bridgehead_4351830068", "bridgehead_N2491667", "bridgehead_N2491735"]
sha256: "b6cac0853b7458f2148931bf9474dc2adfc4616186dbb7330863a4456c87bff7"
---

To customize and create SSP applications successfully, it is important to understand the different components involved:

-   [SuiteScript Server Pages Feature](#bridgehead_N2491374)
    
-   [SSP Application Record](#bridgehead_N2491424)
    
-   [SSP Application Precedence](#bridgehead_4351830068)
    
-   [File Types for SSP Applications](#bridgehead_N2491667)
    
-   [Commerce API](#bridgehead_N2491735)
    

## SuiteScript Server Pages Feature {#bridgehead_N2491374}

To use SSP applications, enable the following features:

-   **SuiteScript Server Pages** - to create, view, or customize SSP applications.
    
-   **SuiteScript 2 Server Pages** - to use SuiteScript 2.0 in SSP applications. Note that SSP applications written in SuiteScript 1.0 will continue to work as normal when this feature is enabled.
    

For more information, see [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html) and [SuiteScript 2.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529598062.html).

Important:

You must have the SuiteScript permission to access SSP Application records. To set up permissions, go to _Setup > Users/Roles > Manage Roles_.

## SSP Application Record {#bridgehead_N2491424}

The SSP Application record is a single NetSuite object that stores details about a website customization. This record lets you group assets, debug script files, and package the customization for use in other NetSuite accounts. On this record, you can set and view these properties:

-   **Application Folder** - the file cabinet folder where your customization files are stored. For more information, see [Create an SSP Application Folder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4343918704.html).
    
-   **URL Root** - the root used in web store links to SSP application assets. For more information, see [Create a SuiteScript 1.0 SSP Application Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html).
    
-   **Supported Touch Points** - the web store entry points where the SSP application can generate dynamic content. For more information, see [Select Supported Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494795.html). Touch points are only defined on the application record only for SSP applications written in SuiteScript 1.0.
    
-   **Default SSP File** - the file that controls the dynamic content the SSP application generates on the website or domain. Only SSP applications written in SuiteScript 2.0 have default SSP files. For more information, see [Select Default SSP File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529598336.html).
    
-   **Sites and Domains where the SSP application is deployed** - the website or domain where the SSP application is deployed. This only applies to SSP applications written in SuiteScript 2.0. For more information, see [SSP Applications (SuiteScript 1.0 Compared with SuiteScript 2.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1529593660.html) and [Deploy and Undeploy SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529598384.html).
    

## SSP Application Precedence {#bridgehead_4351830068}

When SSP applications share a URL and hosting root, a system of precedence determines which SSP application handles a particular request. For more information, see [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html).

Note:

SSP application precedence does not apply to SSP applications written in SuiteScript 2.0 because such applications cannot share both a URL and a hosting root. If two SSP applications written in SuiteScript 2.0 have the same URL root, they cannot be deployed to the same domain or website.

## File Types for SSP Applications {#bridgehead_N2491667}

Web store customizations implemented through SSP applications support the following file types:

-   **.ssp files:** These are **SuiteScript Server Pages** frontend pages you can write in HTML and/or server-side SuiteScript. They're similar to .jsp files, use a similar tag style, and support Includes so you can be pull in code from libraries. You can also call suitelets and RESTlets from .ssp files, and use them to build pages with JQuery.
    
-   **.ss files:** These are request handlers written in SuiteScript, a special kind of suitelet. They can be frontend non-HTML pages, such as AJAX handlers, or backend pages that handle HTTP requests and do things like write HTML, XML, JSON, or JavaScript to the output or issue a redirect.
    

Both .ssp files and .ss files run on the server and support all the SuiteScript APIs that work server-side. SSP application files written in Suitescript 1.0 also support the Commerce API for web store customizations.

For basic examples of .ssp and .ss file content, see [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html) and [Sample SSP Application Code (SuiteScript 2.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529598972.html).

## Commerce API {#bridgehead_N2491735}

The API, supported by both Site Builder and Commerce web stores, includes all of the web store-specific objects and related methods that you need to fully customize your web store on the SuiteCloud platform.

For details about this API, see [Commerce API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496227.html).

Note:

The Commerce API is not available for use with SSP applications written in SuiteScript 2.0.

### Related Topics

-   [SSP Applications Compared to Customization with SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4390440744.html)
-   [SSP Applications (SuiteScript 1.0 Compared with SuiteScript 2.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1529593660.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)
-   [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [Bundle an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495338.html)
-   [SSP Application Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2490486.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
