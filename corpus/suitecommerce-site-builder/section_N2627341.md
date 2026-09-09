---
id: "section_N2627341"
type: "section"
title: "Checkout Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Checkout Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html"
anchors: []
sha256: "442542b485744c5fd6233a59debaefb7e22f250402630d17a0b9a8fa830a105c"
---

Use checkout attribute tags on the checkout tab at _Commerce > Site Builder > Content Management > Tabs_. Click Edit next to the Checkout tab, and use the Web Site Tags listed below in the Place Order Message field. Here, you can capture data related to the order amount, shipping, and tax.

For example, you can use the tag below to capture the total amount of an order:

          `<%=getCurrentAttribute('checkout','total')%>` 
        

| Field Name | Attribute | Notes |
| --- | --- | --- |
| Order subtotal | subtotal |  |
| Tax calculated for complete order | tax |  |
| Order shipping amount | shipping |  |
| Grand total for the order | total |  |

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
