---
id: "section_N2529580"
type: "section"
title: "paymentmethod"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > paymentmethod"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2529580.html"
anchors: []
sha256: "f0a7d6f78db1324fae587d7f9547db323d05bf29da98fa03525c60f3c6707a7a"
---

This object includes payment method information for the order.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| internalid | string | Internal ID | yes | no |
| creditcard | string | Indicates whether payment method is a credit card Value should be T or F. If the Payments Instruments feature is enabled, this contains T if the payment method is a payment card token. | yes | no |
| creditcardtoken | string | Indicates whether payment method is a payment card token. Value should be T or F. Applicable only if the Payments Instruments feature is enabled. | yes | no |
| ispaypal | string | Indicates whether payment method is PayPal Value should be T or F. | yes | no |
| name | string | Name of the payment method | yes | no |
| paypalemailaddress | string | Primary paypal email address | yes | no |
| merchantid | string | Internal ID of the merchant account linked with the payment method | yes | no |
| isexternal | string | Indicates whether payment method is handled outside of NetSuite Value should be T or F | yes | no |
| imagesrc | string | Returns the URL of the image file used to represent the payment method. | yes | no |
| isautomatedclearinghouse | string | Indicates whether payment method is ACH. Value should be T or F | yes | no |

Note:

You cannot set an invoice as a payment method. Instead, set invoice as the paymentterms value for the [payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2528880.html) object. See [Using an Invoice as Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2528880.html#bridgehead_N2529409) for an example.

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
