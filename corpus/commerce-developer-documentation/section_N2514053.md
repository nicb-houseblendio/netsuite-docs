---
id: "section_N2514053"
type: "section"
title: "address"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > address"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2514053.html"
anchors: []
sha256: "ab4b9df9de8fe4ff581f68f21f1d09f0498464fb92d4ce9134281e58dd10e61d"
---

This object contains address information for a web store shopping order.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| addressee | string | Person to which order is sent | yes | yes (reqd) |
| addr1 | string | First line of address | yes | yes (reqd) |
| addr2 | string | Second line of address | yes | yes |
| addr3 | string | Third line of address | yes | yes |
| attention | string | Text for ATTN: line of address | yes | yes |
| city | string | City | yes | yes (reqd) |
| country | string | Country | yes | yes (reqd) |
| defaultbilling | string | Indicates whether address is default billing address Value should be T or F. | yes | yes |
| defaultshipping | string | Indicates whether address is default shipping address Value should be T or F. | yes | yes |
| internalid | string | Internal ID | yes | yes |
| isresidential | string | Indicates whether address is residential Value should be T or F. | yes | yes |
| phone | string | Phone number Note: Address forms on Reference Checkout 2.04 and earlier **require** the phone number field. | yes | yes |
| state | string | State for address | yes | yes (reqd) |
| zip | string | Zip code | yes | yes (reqd) |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
