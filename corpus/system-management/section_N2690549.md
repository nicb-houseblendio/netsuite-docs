---
id: "section_N2690549"
type: "section"
title: "Preparing Pages for Content Delivery"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SuiteCommerce Integrations > Content Delivery Integration > Preparing Pages for Content Delivery"
parent: "section_N2688958"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2690549.html"
anchors: ["bridgehead_N2691686", "procedure_N2691698"]
sha256: "ab272b5120a8b133db6599865e6c0a379423739645b957460af5f1c4567f7530"
---

Important:

The Content Delivery Service is only supported up to the Denali R2 (revision 2) release of SuiteCommerce Advanced only. After that, you should use Site Management Tools for SuiteCommerce and for the Mont Blanc release and later.

This section shows you how to get Reference Implementation pages ready for content delivery. Your web application developers should handle this since it means editing code in the page.

## Configuring the Reference Implementation {#bridgehead_N2691686}

To show Content Delivery pages on your site, you must first set up the SuiteCommerce Advanced SSP to include the content delivery scripts.

If you use more than one Reference Application for your web store, you can select which applications use a Content Delivery record by adding the 'app' tag with the application name, like Checkout, MyAccount, or Shopping. For example, app:Shopping means the content only shows in the Shopping application. If you don't use an app tag, the content is available for all Reference Applications.

You can also show Content Delivery content inside Backbone Modals. To do this, add the prefixViewId 'in-modal-' to the target ID in the Content Delivery record. You can choose if the content shows only inside a modal, both inside and outside, or just outside a modal.

#### To include the Content Delivery scripts: {#procedure_N2691698}

1.  Go to _Commerce > Hosting > SSP Applications_.
    
2.  Click **Edit** next to the SuiteCommerce Advanced SSP application you use for the site with content delivery. For example, SuiteCommerce Advanced - Dev \[version\].
    
3.  In the **Libraries** subtab under **Scripts**, click **Add**.
    
4.  Go to the path of the content\_delivery\_service\_library\_v2.js file in the Content Delivery reference installation.
    
    Important:
    
    If you're using a custom SSP application, you must define this library for your custom SSP application too.
    
5.  Click **Save**.
    

### Related Topics

-   [Understanding Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2689274.html)
-   [Using Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2689412.html)
-   [SEO Considerations for Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491317607.html)
-   [Permission Validation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542647720.html)
-   [Content Delivery Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2688958.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
