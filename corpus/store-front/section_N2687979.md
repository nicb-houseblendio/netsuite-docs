---
id: "section_N2687979"
type: "section"
title: "Prepare Pages for Product Merchandising Zones"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Marketing > Storefront Merchandising Tools > Product Merchandising > Prepare Pages for Product Merchandising Zones"
parent: "section_N2687121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687979.html"
anchors: ["section_N2688418", "procedure_N2688430"]
sha256: "c439bd48a7e8842da19943b76a7ed152aabbdd73706673a71d1e75982ce9cc6e"
---

Preparing pages for Product Merchandising zones should be done by your web application developers since it involves editing code on the related page.

## Configure the Reference Implementation {#section_N2688418}

To call Merchandising Rules from your site pages, you must first configure the SuiteCommerce Advanced SSP to include the merchandising script.

#### To include the Product Merchandising script: {#procedure_N2688430}

1.  Go to _Commerce > Hosting > SSP Applications_.
    
2.  Click **Edit** next to the SuiteCommerce Advanced SSP application used for the web site where product merchandising is used. For example, SuiteCommerce Advanced - Dev \[version\].
    
3.  In the **Libraries** subtab under **Scripts**, click **Add**.
    
4.  Go to the path of the dynamic\_merchandising\_library\_v2.js file in the Product Merchandising reference installation.
    
    ![Library script files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/Marketing/refPM_library.PNG)
    
    Important:
    
    If you're using a custom ssp application, you will need to define this library for your custom ssp application.
    
5.  Click **Save**.
    

### Related Topics

-   [Product Merchandising Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687230.html)
-   [Create a Product Merchandising Rule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687488.html)
-   [Storefront Merchandising Tools](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1531814631.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
