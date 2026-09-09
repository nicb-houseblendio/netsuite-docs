---
id: "section_N2516589"
type: "section"
title: "checkoutsettings"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > checkoutsettings"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2516589.html"
anchors: []
sha256: "f98865a18944a390375ef34a6b0f6a6262e597cf754088c21b630dd575d64e6b"
---

This object contains information used for checkout.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| cancelurl | string | Full URL path for redirect after cancel action during order submission Used for PayPal Express support | no | yes |
| continueurl | string | Full URL path for redirect after order submission Used for PayPal Express support | no | yes |
| createorder | boolean | If value is set to T, backend submits current shopping order when Continue link is clicked Default value is F Used for PayPal Express support | no | yes |
| custchoosespaymethod | string | Value should be T or F. | yes | no |
| paymentauthorization | [threedsecure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2536058.html) object with fields | Settings to handle payment authorization Used for 3D Secure support | yes | yes |
| paymentmandatory | string | Indicates whether payment is required Value should be T or F. | yes | no |
| paypalexpress | Object with fields | Used for PayPal Express support Includes the following fields:
-   _available_ (boolean) (must be set to T to support PayPal Express)
-   _imageurl_ (string)

 | yes | no |
| 

requiretermsand

conditions



 | string | Indicates whether terms and conditions text is required Value should be T or F. | yes | no |
| saveccinfo | string | Indicates whether credit card should be saved by default Value should be T or F. | yes | no |
| shippingaddrfirst | string | Indicates whether shipping address should be displayed first Value should be T or F. | yes | no |
| showpurchaseorder | string | Indicates whether purchase order should be displayed Value should be T or F. | yes | no |
| showsavecc | string | Indicates whether the Save Credit Card field should be displayed Value should be T or F. | yes | no |
| termsandconditions | string | Text of Terms and Conditions field | yes | no |
| type | string | Used for integration with third party checkout providers Valid values are: paypalexpress, google | no | yes |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
