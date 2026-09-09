---
id: "section_N2524578"
type: "section"
title: "orderitem"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > orderitem"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2524578.html"
anchors: []
sha256: "2041b04e050bbfc1e43ffb04b3e776604699b8e4b3ed011d6438eb68133318d5"
---

The orderitem object is a subtype of [item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2522520.html).

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| amount | string | Currency amount for items | yes | no |
| amount\_formatted | string | Amount formatted with currency symbol | yes | no |
| internalid | string | Internal ID for item Unique identifier that should be used when adding an item to the cart | yes | yes (reqd) |
| name | string | Display name | yes | no |
| options | JSON object | List of name/value pairs | yes | yes |
| orderitemid | string | Unique ID for an item in an order | yes | yes |
| promotionamount | string | Amount after any line-level discounts | yes | no |
| 
promotionamount\_

formatted



 | string | Amount after any line-level discounts formatted with currency symbol | yes | no |
| promotiondiscount | string | Amount of discount related to promotions | yes | no |
| promotiondiscount\_formatted | string | Amount of discount related to promotions formatted with currency symbol | yes | no |
| quantity | string | Number of items in order | yes | yes |
| rateschedule | string | Price schedule for quantity pricing | yes | no |
| shipaddress | string | ID of shipping address for item | yes | yes |
| shipcarrier | string | Shipping carrier Note: Valid values that can be set for shipcarrier are `ups` or `noups`. | yes | no |
| shipmethod | JSON object of type [shipmethod](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2531241.html) | ID of shipping method for item Used when the Multiple Shipping Routes feature is enabled | yes | yes |
| taxamount | string | The total tax amount for the line item. Applicable only for tax calculations using SuiteTax. Tax calculation using SuiteTax is available only for US and Canada. | yes | no |
| taxdetailsreference | string | The ID that links the tax details returned by `getTaxDetails()` with the item to which they apply. Applicable only for tax calculations using SuiteTax. Tax calculation using SuiteTax is available only for US and Canada. | yes | no |
| taxtype1 | string | Type of the item tax. For example, GST/VAT/WET. Not applicable if SuiteTax is enabled. | yes | no |
| taxrate1 | string | Rate of the tax in percentage. Not applicable if SuiteTax is enabled. | yes | no |
| taxtype2 | string | For Canada only. Currently returns `PST`. Not applicable if SuiteTax is enabled. | yes | no |
| taxrate2 | string | For Canada only. The rate of PST tax in percentage when applicable. Not applicable if SuiteTax is enabled. | yes | no |
| tax1amt | string | The total tax amount for the line item. Not applicable if SuiteTax is enabled. | yes | no |
| fulfillmentPreferences | JSON object of type [fulfillmentPreferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4804194943.html) | Fulfillment preference for item | yes | no |
| discounts\_impact | JSON object of type [discounts\_impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4805931347.html) | Per line discount impact for the line item. | yes | no |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
