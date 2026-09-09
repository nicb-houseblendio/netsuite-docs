---
id: "section_N2536058"
type: "section"
title: "threedsecure"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > threedsecure"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2536058.html"
anchors: []
sha256: "90adc6ab26cc5afe5a2891c2ba8824e729a6108764ffcf4ed636a9f20eac386e"
---

This object contains information used for 3D Secure payment integration.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| noredirect | string | Default is F If set to T, when 3D Secure authorization is required, instead of a redirect, a status object that includes fields for 3D secure integration is returned. | no | yes |
| servicehtml | string | Complete HTML for IFrame that triggers 3D Secure service | yes | no |
| termurl | string | URL for page or handler where 3D Secure POST is sent | no | yes |
| threedsecurekey | string | Key used by backend to identify currenct 3D Secure data object | yes | yes |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
