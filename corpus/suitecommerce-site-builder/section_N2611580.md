---
id: "section_N2611580"
type: "section"
title: "URL Parameters for Displaying Shopping Pages"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters > URL Parameters for Displaying Shopping Pages"
parent: "section_N2611157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611580.html"
anchors: []
sha256: "af55df55e1a07bc156fbeb7253afea921d0edeb01aba311b4c16893b01ef8c64"
---

The following parameters are supported on URL, **/s.nl**. All the parameters listed below can display on web store, cart and checkout pages.

For more information about constructing a URL, see [Required Web Site URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html#bridgehead_N2611392). Note that the internal ID for any record in NetSuite displays in the address bar of your browser when you navigate to that record. For more information, see [Finding Internal IDs of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416030736.html)

| URL Parameter | Notes |
| --- | --- |
| `c` | Required to identify the NetSuite account (c.123456). Not required if you use a custom domain. **http://shop.netsuite.com/s.nl/c.123456/n.3/sc.13/.f** |
| `n` | Required to identify the site (n.3) when you use multiple websites. Not required if you use a custom domain or if you do not use multiple websites. **http://shop.netsuite.com/s.nl/c.123456/n.3/sc.13/.f** |
| `sc` | Identifies the tab (sc.42) on a tab page; `sc` stands for section. On a category or item detail page, this parameter identifies the selected tab. It also provides location context so the correct tab and category are highlighted in the site navigation portlet. For example:
-   http://shop.netsuite.com/s.nl/c.123456/n.3 `/sc.42/`.f
-   http://www.wolfeelectronics.com/s.nl `/sc.42/`.f

 |
| `category` | Identifies the category (category.13) on a category page. On an item detail page, this parameter identifies the category context of the selected item. It also provides location context so the correct tab and category are highlighted in the site navigation portlet. For example:

-   http://shop.netsuite.com/s.nl/c.123456/n.3/sc.17 `/category.13/`.f
-   http://www.wolfeelectronics.com/s.nl/sc.17 `/category.13/`.f

 |
| `id` | Identifies the item (id.100) on an item detail page. For example:

-   http://shop.netsuite.com/s.nl/c.123456/n.3/it.A `/id.100` /.f?sc=17&category=13
-   http://www.wolfeelectronics.com/s.nl/it.A `/id.100` /.f?sc=17&category=13

 |
| `it` | Identifies the item type (it.I). On an item detail page, this parameter distinguishes between sales items (A), and information items (I). Note that this parameter is optional for sales items, but required for information items. For example:

-   http://shop.netsuite.com/s.nl/c.123456/n.3 `/it.I/` id.208/.f?sc=17&category=15
-   http://www.wolfeelectronics.com/s.nl `/it.I/` id.208/.f?sc=17&category=15

 |
| `search` | This parameter makes any page in the web store a search results page. It displays the search entry field on a web store page, with the search results for that page displayed below it. For example: These URLs display a page with results for the search term, 'electronics':

-   http://shop.netsuite.com/s.nl/c.123456/sc.2/.f `?search=electronics`
-   http://www.wolfeelectronics.com/s.nl/sc.2/.f `?search=electronics`

 |
| `ext` | For use only with External Catalog (WSDK) sites to add NetSuite e-commerce functionality. When this parameter is set true, the page is displayed without any item or category tabs. Only the cart, checkout and customer center tabs appear if they are set to display in the Web site. This example displays the shopping cart page for an external catalog site (ext=T): `http://www.wolfeelectronics.com/s.nl?sc=2&ext=T` |
| `continue` | When used with the `sc` parameter identifying the cart tab, this parameter allows customization of the Continue Shopping button to go to the specified URL. In this example, the `continue` parameter sends the shopper to a specific Web Store page when they click the Continue Shopping button:

-   http://shop.netsuite.com/s.nl?c.123456&sc=3 `&continue=http://shopping.netsuite.com/s.nl/c.123456/n.3/sc.12/.f`
-   http://www.wolfeelectronics.com/s.nl?sc=3 `&continue=http://www.wolfeelectronics.com/s.nl/sc.12/.f`

 |
| `range=from,to,of` | Displays a set of items: `from` item x, `to` item y, `of` n number of pages. The `from` and `to` values start at 1 for the first item (as opposed to 0). No more than 50 items can be displayed on a page. The `to` parameter is ignored if the range includes more than 50 items. This URL displays the last three items in a list of thirteen items which spans two pages:

-   http://shop.netsuite.com/s.nl/c.123456/n.3/sc.12/category.2
    
    /.f? `range=11,13,13`
    
-   http://www.wolfeelectronics.com/s.nl/sc.12/category.2/.f? `range=11,13,13`

 |
| `logoff` | Only for use on the checkout domain. When you add `logoff=T` to the URL, this parameter logs off the current shopper. |
| `login` | Only for use on the checkout domain. When you add `login=T` to the URL, this parameter makes the current page a log in page. |
| `newcust` | Only for use on the checkout domain. When you add `newcust=T` to the URL this parameter displays the registration page with mandatory password fields. |
| `redirect` | Redirects to a URL after a process has completed. This parameter is observed by backend requests such as additemtocart.nl. |

### Related Topics

-   [URL Parameters for Adding Items to the Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html)
-   [URL Parameters for Passing Marketing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613194.html)
-   [URL Parameters for Setting Values in Your OneWorld Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2614795.html)
-   [URL Parameters for Setting the Currency on your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615184.html)
-   [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
