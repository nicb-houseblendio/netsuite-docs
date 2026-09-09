---
id: "section_N2612472"
type: "section"
title: "URL Parameters for Adding Items to the Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters > URL Parameters for Adding Items to the Cart"
parent: "section_N2611157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html"
anchors: ["bridgehead_N2612544", "bridgehead_N2612842"]
sha256: "a2dad3c7f41b85f9585d2104ac0579d6d9a7f87a151ed3d8b223d4d0b4004737"
---

NetSuite supports two different URLs for adding items to the shopping cart:

-   [/app/site/backend/additemtocart.nl](#bridgehead_N2612544) _\-_ Use this URL to create add to cart buttons for items in an external catalog site or in a website made of hosted HTML pages.
    
-   [/app/site/backend/intl/additemtocart.nl](#bridgehead_N2612842) _\-_ Use this URL in a web store associated with a OneWorld account. Create add to cart buttons that set multiple parameters to be processed in one request, like subsidiary and currency, for example.
    

All the parameters listed in the tables below are used in either the POST or GET action that adds an item to the shopping cart.

For example, you can use the `multi` parameter to create a URL for distribution to customers in a promotional email. This URL will add multiple items to the shopping cart when a customer clicks the link to visit your web store.

For information about adding multiple items to the shopping cart, see [Adding Multiple Items to the Shopping Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613001.html).

## /app/site/backend/additemtocart.nl {#bridgehead_N2612544}

Use the parameters below to create add to cart buttons for items in an external catalog site or in a website made of hosted HTML pages.

| URL Parameter | Notes |
| --- | --- |
| `buyid` | Passes the internal ID for the item which is added to the cart. |
| `qty` | Passes the quantity of the item to add to cart. |
| `amount` | Only functions with donation items. This parameter sets the price for the item added to the cart. |
| `category` | This parameter is required for tracking customer activity on your website. However, it is not required for successfully adding an item to the shopping cart. |
| `multi<id,qty;...>` | Adds multiple items to the cart in one request. This parameter does not support item options. For more information, see [Adding Multiple Items to the Shopping Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613001.html) |
| `redirect` | Use the redirect parameter to take shoppers to a page on your website after they add an item to the cart. This parameter is used to determine the proper page to display after an item is added to the cart. Note: Only functions when the **After Shopper Adds an Item to the Cart** preference is set to **stay on the same page**. Set this preference on the Shopping subtab of the Web Site Setup form. |
| `continue=<url>` | Sets the URL for the Continue Shopping button in an External Catalog Web site. For more information, see [Setting Up an External Catalog Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2600712.html). |
| `showcart` | When you add `showcart=T` to the URL, this parameter displays the cart after items are added to the shopping cart. |

## /app/site/backend/intl/additemtocart.nl {#bridgehead_N2612842}

You can use this URL with the same parameters as the additemtocart URL above, except that you can use `/app/site/backend/intl/additemtocart.nl` to set parameters for subsidiary, currency, and language.

| URL Parameters | Notes |
| --- | --- |
| `selcurrency` | Use the internal ID of the currency you want to set. |
| `selsubsidiary` | Use the internal ID of the subsidiary you want to set. |
| `selshopperlanguage` | Use this parameter to pass a locale key. For example: en\_US, en\_UK, or fr\_FR. Note: locale keys are not exposed in the NetSuite system. You may need to research which language code is appropriate. |

Note:

If your selected Out Of Stock Behavior option is **Disallow back orders but display out-of-stock message** or **Remove out-of-stock items from store**, you might still be able to add out of stock items to your cart using these URL parameters. However, when you try to place the order with such out of stock items in your shopping cart, an error message is displayed and you will not be able to place the order successfully.

### Related Topics

-   [URL Parameters for Displaying Shopping Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611580.html)
-   [URL Parameters for Passing Marketing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613194.html)
-   [URL Parameters for Setting Values in Your OneWorld Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2614795.html)
-   [URL Parameters for Setting the Currency on your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615184.html)
-   [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
