---
id: "section_N2513358"
type: "section"
title: "order"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > order"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2513358.html"
anchors: []
sha256: "6d80da3044204db1713508090bdf76b477a1252d27ae6d995076c5c60b999aa8"
---

This object contains other objects, and includes the complete set of data for a web store shopping order.

| Object Name | Object Type | Description |
| --- | --- | --- |
| billaddress | JSON object (type of [address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2514053.html)) | Billing address for order |
| [customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2519129.html) | JSON object | Current shopper information |
| customfields | JSON object | List of custom fields name/value pairs set for order |
| [giftcertificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2522051.html) s | Array | Gift certificates applied to order |
| items | Array of [orderitem](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2524578.html) s | Items added to order |
| [payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2528880.html) | JSON object | Payment information for order |
| [promocode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2530136.html) s | Array | Promotion codes applied to order |
| purchaseNumber | JSON object | Purchase order number for the order |
| shipaddress | JSON object (type of [address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2514053.html)) | Shipping address for order |
| [shipmethod](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2531241.html) | JSON object | Shipping method for order |
| [status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2535212.html) | JSON object | Status of order |
| summary | JSON object (type of [ordersummary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2526142.html)) | Summary information for order (subtotal, total, tax, etc.) |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
