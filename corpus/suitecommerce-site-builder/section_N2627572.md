---
id: "section_N2627572"
type: "section"
title: "Order Confirmation Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Order Confirmation Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html"
anchors: []
sha256: "642fb82a607e6632cc97da7f865d6d2d0a5214d806be6aad2f80579958176643"
---

Use the attributes listed in the table below to capture data from orders placed on your website and send it to third-party reporting tools. For more information and a code sample, see [Working with Google Analytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2653735.html).

Capture order amount, shipping, and tax data by adding attribute tags to your tracking script HTML on the Analytics subtab of the website record.

For best results, enter all your analytics information in one place at _Commerce > Websites > Website List_ on the Analytics subtab. The confirmation attribute is only used on the Thank You page, which shows up after a shopper submits an order on your site.

The sample attribute tag below captures data from the items on the order:

          `<%=getCurrentAttribute('confirmation','orderitems')%>` 
        

| Order component | Attribute | Notes |
| --- | --- | --- |
| Order subtotal | subtotal |  |
| Tax calculated for complete order | tax |  |
| Order shipping amount | shipping |  |
| Grand total for the order | total |  |
| order number | ordernumber |  |
| Promotion code ID | promotioncoderef | Only supported on the order confirmation page. |
| Partner ID | partner |  |
| Shipping method | shipmethodref |  |
| Promotion code name | promocode |  |
| Lead Source | leadsource |  |
|  | orderitems | Returns data for each item in the order, including item name, quantity, and price. |
|  | shiptocity | Returns the city where the order was shipped. |
|  | shiptostate | Returns the state (or province?) where the order was shipped. |
|  | shiptocountry | Returns the country where the order was shipped. |

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
