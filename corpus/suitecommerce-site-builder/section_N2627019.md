---
id: "section_N2627019"
type: "section"
title: "Request Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Request Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html"
anchors: ["bridgehead_4483031089"]
sha256: "172e86468528a33d5bd1d2a8b83fe6aa3ec05b54c176fbaf430619e21cefd722"
---

You can create attribute tags for website properties that aren't shown on NetSuite records, like elements from browser requests when shoppers visit your site. For example, you can use the Attribute tag below to capture cookies from visitors to your site:

          `<%=getCurrentAttribute('request','cookies')%>` 
        

Note:

When using request attributes, also use nlescapehtml in your attribute tag to avoid cross-site scripting vulnerabilities. This additional parameter is most commonly used along with the querystring attribute. For more information see, [Specifying Information for Display](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html#bridgehead_3823947633).

| Site Properties | Attribute | Notes |
| --- | --- | --- |
| Cookies associated with the current page | cookies |  |
| IP Address for the session | ipaddress |  |
| Referrer to the current page | referrer |  |
| Scheme of current page (http or https) | scheme | Use this attribute to create secure links. For more information, see [Creating Secure Links](#bridgehead_4483031089). |
| URL parameters of the current page | querystring |  |
| User Agent HTTP header | useragent | Returns the visitor's browser type and version. |

## Creating Secure Links {#bridgehead_4483031089}

When you show an image on your site that links to another site, you must use a full URL. If you use a non-secure URL (one that starts with HTTP as opposed to HTTPS) on a checkout page, visitors might see a popup warning about 'nonsecure items.' To avoid this warning, use an Attribute tag to build a link that returns HTTP or HTTPS as needed. For example:

          `<%=getCurrentAttribute('request', 'scheme')%>://www.othersite.com/file.ext` 
        

You can use this tag in a website template, and the resulting URL will always be a fully qualified URL appropriate for the page on which it displays, HTTP for shopping pages, and HTTPS for checkout pages:

`http://www.othersite.com/file.ext`

`https://www.othersite.com/file.ext`

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
