---
id: "section_N2522520"
type: "section"
title: "item"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > item"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2522520.html"
anchors: []
sha256: "ce5fcbcaec6504f32f53866cab35bdacba8c842f032ada4059938a3b28ca9734"
---

This object contains basic information about an item that can be included in the order.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| featureddescription | string | Featured description | yes | no |
| internalid | string | Internal ID for item Unique identifier that should be used when adding an item to the cart | yes | yes (reqd) |
| isavailable | string | Indicates whether item is available for web store order Value should be T or F. | yes | no |
| isdonationitem | string | Indicates whether item is donation item Value should be T or F. | yes | no |
| isdropshipitem | string | Indicates whether item is a dropship item Value should be Yes or No. | yes | no |
| isspecialorderitem | string | Indicates whether item is a special order item Value should be Yes or No. | yes | no |
| isstorespecial | string | Indicates whether item is on special in the web store Value should be T or F. | yes | no |
| istaxable | string | Whether the item is taxable Value should be Yes or No. | yes | no |
| itemtype | string | Type of the item, such as inventory, kit/package, etc. | yes | no |
| nopricemessage | string |  | yes | no |
| nopricemessage2 | string |  | yes | no |
| outofstockmessage | string |  | yes | no |
| outofstockmessage2 | string |  | yes | no |
| 
outofstocknobackorder

message



 | string |  | yes | no |
| pagetitle | string |  | yes | no |
| pagetitle2 | string |  | yes | no |
| quantityavailable | string | Number of items available for ordering | yes | no |
| rate | string | Unit price | yes | no |
| rate\_formatted | string | Unit price formatted with currency symbol | yes | no |
| storedetaileddescription | string | Store detailed description | yes | no |
| storedescription | string | Store description | yes | no |
| storedisplayimage | string |  | yes | no |
| storedisplayname | string | Store display name | yes | no |
| storedisplayname2 | string | Second store display name | yes | no |
| storedisplaythumbnail | string |  | yes | no |
| freegiftpromotionid | string | ID of the free gift promotion this item belongs to | yes | no |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
