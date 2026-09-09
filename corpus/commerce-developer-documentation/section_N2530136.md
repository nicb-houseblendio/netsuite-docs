---
id: "section_N2530136"
type: "section"
title: "promocode"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > promocode"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2530136.html"
anchors: []
sha256: "148ccb8725ab087953e08027962d02f5cf78d01c2fca8d2a6d6827db5787600d"
---

This object contains promotion code information for the order.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| discountamount | string | Currency amount of the discount applied to the order. | yes | no |
| errormsg | string | Returns the error message when a promo code is not valid. | yes | no |
| internalid | string | Internal ID | yes | no |
| isvalid | string | Indicates whether promocode is valid for the current order. Value should be T or F. | yes | no |
| promocode | string | The value of the Coupon Code ID. This corresponds to what the user sets during the checkout process. | yes | yes |
| promocodeid | string | The value of the Promocode ID. This corresponds to the promocode displayed in the NetSuite UI. Note: The value of this field is not changed when a coupon code is modified. | yes | yes |
| purchase\_discount\_amount | string | Currency amount of the discount applied to the order. | yes | no |
| purchase\_discount\_amount\_formatted | string | Discount amount formatted with currency symbol. | yes | no |
| shipping\_discount\_amount | string | Currency amount of the discount applied to the shipping cost. | yes | no |
| shipping\_discount\_amount\_formatted | string | Discount shipped amount formatted with currency symbol. | yes | no |
| promotion\_name | string | Name of the promotion associated with the applied coupon. | yes | no |
| discount\_name | string | Name of the discount associated with the applied promotion. | yes | no |
| discount\_type | string | Indicates the type of discount, and its value should be PERCENTAGE or FLAT. | yes | no |
| discount\_rate | string | Rate of the discount in percentage if the type of discount is PERCENTAGE and currency amount of the discount if the type of discount is FLAT. | yes | no |
| is\_auto\_applied | boolean | Indicates whether the promocode was automatically or manually applied for the current order. Value should be true or false. | yes | no |
| applicability\_status | string | Indicates whether the promocode is applied to the current order or not. Value should be one of the following:
-   APPLIED - Indicates that the promocode is applied to the current order and you get a discount if the promocode is valid. It also indicates that the type of promotion is SuitePromotion.
-   NOT\_APPLIED - Indicates that the promocode does not give you a discount even though it is added to the current order. It also indicates that the type of promotion is SuitePromotion.
-   NOT\_AVAILABLE - Indicates that the applicability status information is not available. You get this value in case of Standard promotions.

 | yes | no |
| applicability\_reason | string | Specifies the reason for not applying the promocode. Value should be one of the following:

-   DISCARDED\_BEST\_OFFER - Indicates that the promocode is not applied as there is another promocode or a combination of promocodes that is giving you a better discount.
-   CRITERIA\_NOT\_MET - Indicates that the promocode is not applied as it does not meet the criteria. For example, if your order does not meet the minimum order amount requirement.
-   NOT\_AVAILABLE - Indicates that the promocode is applied or the promotion is a Standard promotion.

 | yes | no |
| promotion\_type | string | Indicates the type of promotion. | yes | no |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
