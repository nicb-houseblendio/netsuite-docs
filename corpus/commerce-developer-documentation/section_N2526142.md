---
id: "section_N2526142"
type: "section"
title: "ordersummary"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > ordersummary"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2526142.html"
anchors: []
sha256: "cfa7166d15722eaa050476b11fda0e0336a7c57fe256854d8e83cc4a3fe9ca31"
---

This object contains summary information for the order.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| discountedsubtotal | number | Item subtotal - any applicable discount | yes | no |
| 
discountedsubtotal\_

formatted



 | string | Item subtotal - any applicable discount formatted with currency symbol | yes | no |
| discountrate | string | Raw discount | yes | no |
| discounttotal | number | Total amount of discounts applied | yes | no |
| discounttotal\_formatted | string | Total amount of discounts applied formatted with currency symbol | yes | no |
| giftcertapplied | number | Total amount of gift certificates applied | yes | no |
| giftcertapplied\_formatted | string | Total amount of gift certificates applied formatted with currency symbol | yes | no |
| handlingcost | number | Amount of handling cost | yes | no |
| handlingcost\_formatted | string | Amount of handling cost formatted with currency symbol | yes | no |
| itemcount | number | Returns the quantity of items in the cart. Important: Use this argument with the `getOrderSummary` method for the most optimized call. Note that the value returned equals the total quantity of items in the cart which may differ from the total lines in the cart. For example, if a shopper has three of the same items in the cart, the call returns 3. | yes | no |
| shippingcost | number | Amount of shipping cost | yes | no |
| shippingcost\_formatted | string | Amount of shipping cost formatted with currency symbol | yes | no |
| subtotal | number | Total of quantity \* rate per line item | yes | no |
| subtotal\_formatted | string | Total of quantity \* rate per line item formatted with currency symbol | yes | no |
| tax2total | number | Total secondary tax on taxable elements of the order (items + shipping + handling) - effect of any discounts. Not applicable if SuiteTax is enabled. | yes | no |
| tax2total\_formatted | string | Total secondary tax on taxable elements of the order (items + shipping + handling) - effect of any discounts formatted with currency symbol. Not applicable if SuiteTax is enabled. | yes | no |
| taxondiscount | number | For VAT countries, currency amount of the tax rate \* the discount amount | yes | no |
| taxondiscount\_formatted | string | For VAT countries, currency amount of the tax rate \* the discount amount formatted with currency symbol | yes | no |
| taxonhandling | number | Currency amount of the tax rate \* taxable handling amount | yes | no |
| taxonhandling\_formatted | string | Currency amount of the tax rate \* taxable handling amount formatted with currency symbol | yes | no |
| taxonshipping | number | Currency amount of the tax rate \* taxable shipping amount | yes | no |
| taxonshipping\_formatted | string | Currency amount of the tax rate \* taxable shipping amount formatted with currency symbol | yes | no |
| taxtotal | number | Total tax on taxable elements of the order (items + shipping + handling) - effect of any discounts | yes | no |
| taxtotal\_formatted | string | Total tax on taxable elements of the order (items + shipping + handling) - effect of any discounts formatted with currency symbol | yes | no |
| totalcombinedtaxes | number | A grand total of all the tax components (taxtotal + tax2total) associated with an order | yes | no |
| totalcombinedtaxes\_formatted | string | A grand total of all the tax components (taxtotal + tax2total) associated with an order formatted with currency symbol | yes | no |
| total | number | Order subtotal + shipping, handling, and all tax, less the effect of any discounts | yes | no |
| total\_formatted | string | Order subtotal + shipping, handling, and all tax, less the effect of any discounts formatted with currency symbol | yes | no |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
