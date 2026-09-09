---
id: "section_N2613194"
type: "section"
title: "URL Parameters for Passing Marketing Information"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters > URL Parameters for Passing Marketing Information"
parent: "section_N2611157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613194.html"
anchors: []
sha256: "08cae147ed34e518ed2f299fb28cb97185cf62c2a5ca35d3061f9470ee92a93d"
---

The listed parameters are useful for marketing your web store. You can provide discount codes for your customers and track campaigns. You can also track partners who refer shoppers to your site.

For more information about constructing a URL, see [Required Web Site URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html#bridgehead_N2611392).

| URL Parameter | Notes |
| --- | --- |
| `c` | Identifies the NetSuite account (c.123456). Not required if you use a custom domain. `http://shop.netsuite.com/s.nl/c.123456/n.3/sc.13/.f` |
| `n` | Identifies the site when you use multiple websites. Not required only if you use a custom domain. `http://shop.netsuite.com/s.nl/c.123456/n.3/sc.13/.f` |
| `leadsource` | Passes campaign information to your web store. You can create a campaign that drives shoppers to your web store with the `leadsource` parameter in the URL. This way, you can capture the campaign ID on the lead record created when a shopper registers on your web store and track the success of the campaign. These are examples of campaign URLs entered in NetSuite:
-   http://shop.netsuite.com/s.nl?c=123456&leadsource=great\_sale
-   http://www.wolfeelctronics.com **?leadsource=great\_sale**

 |
| `promocode` | Use any valid coupon code with this URL parameter. This parameter passes the discount item associated with a promotion code into the session and keeps it there until the shopper arrives on the last page of checkout. Use this parameter, to drive shoppers to your web store with a URL that provides them with a discount at checkout. For more information about creating promotion codes, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html). The URLs below include the `promocode` parameter:

-   http://shop.netsuite.com/s.nl?c=123456 `&promocode=discount`
-   http://www.wolfeelectronics.com `?promocode=discount`

 |
| `partner` | Passes the ID of the referring partner. If the partner field is exposed on your Sales Order form, this partner is saved on the transaction and on the customer record created from that transaction. Both URLs below track partner information:

-   http://shop.netsuite.com/s.nl?c=123456 `&partner=slconsulting`
-   http://www.wolfeelectronics.com `?partner=slconsulting`

You can also use the partner parameter with the Partner Code instead of the Name. It lets you keep the partner relationship transparent to the web store visitor. |

### Related Topics

-   [URL Parameters for Displaying Shopping Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611580.html)
-   [URL Parameters for Adding Items to the Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html)
-   [URL Parameters for Setting Values in Your OneWorld Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2614795.html)
-   [URL Parameters for Setting the Currency on your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615184.html)
-   [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
