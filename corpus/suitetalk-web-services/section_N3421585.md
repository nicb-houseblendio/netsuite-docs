---
id: "section_N3421585"
type: "section"
title: "Effects of Account Configuration in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Setup > SOAP Web Services Development Considerations > Effects of Account Configuration in SOAP Web Services"
parent: "section_N3421363"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421585.html"
anchors: []
sha256: "a36ce05d9d2135aef9c4d1b18f49130ab5a03298d50ee836d5d0000fad08a7e8"
---

Form customization or enabling/disabling features can add required fields to various forms used on records. Each SOAP request validates fields against submitted data, returning errors for failed validation. However, for get, add, addList and search requests, it is possible that the field requirements change mid-request, resulting in errors for a **subset** of the request.

For example, you want to submit 20 new customer records using the addList operation. The request passes field validation initially. However, after the first 15 customers are added, the required fields may be changed within your NetSuite account, causing an error to be returned for the 5 remaining items.

Note:

For more specific information about working with NetSuite records, fields, and forms in SOAP web services, see [Records, Fields, Forms, and Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3428523.html).

### Related Topics

-   [Development Considerations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421458.html)
-   [NetSuite Features in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421552.html)
-   [SOAP Web Services Reliability Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540364662.html)
-   [Enumerations, Special Characters, and Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421860.html)
-   [Image References in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421872.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
