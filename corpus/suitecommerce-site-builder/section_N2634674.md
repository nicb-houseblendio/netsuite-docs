---
id: "section_N2634674"
type: "section"
title: "Tags for Information Unavailable on Records"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Tags for Information Unavailable on Records"
parent: "chapter_N2615371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2634674.html"
anchors: []
sha256: "eea1f93f3e30c60b9b75633c4e472ed407391ee191a6d5037da97336b97bd083"
---

You can add attributes that do not exist on records, such as an Add to Cart button or an Out Of Stock message. Web Site tags arent supported in SuiteCommerce Advanced websites.

Note:

To include the stock status message with an Add to Cart button, you must use the stock status message attribute in a tag that appears before the attribute tag for the add to cart button.

For example:

          `<%=getCurrentAttribute('item','stockstatusmessagehtml')%><%=getCurrentAttribute('item','addtocartdrilldownhtml')%>` 
        

| Additional Features | Item | Info Item | Category | Site | Request | Attribute |
| --- | --- | --- | --- | --- | --- | --- |
| Cookies associated with the current page |  |  |  |  | X | cookies |
| IP Address for the session |  |  |  |  | X | ipaddress |
| Referrer to the current page |  |  |  |  | X | referrer |
| Scheme of current page(http or https) - used to create secure links |  |  |  |  | X | scheme |
| URL parameters of the current page |  |  |  |  | X | querystring |
| User Agent HTTP header - visitor's browser type & version |  |  |  |  | X | useragent |
| HTML to publish the entire page | X | X | X | X |  | storepagehtml |
| Copyright message with © symbol, year, and store display name |  |  |  | X |  | copyrighthtml |
| Display name of the store |  |  |  | X |  | name |
| Home page URL |  |  |  | X |  | homepageurl |
| Logo alignment - returns left, right or center |  |  |  | X |  | logoalignment |
| Logo image <img> tag or |  |  |  | X |  | logoimagehtml |
| Logo image URL |  |  |  | X |  | logoimageurl |
| Tab name currently being |  |  |  | X |  | currenttablabel |
| Welcome page image<img> tag or HTML |  |  |  | X |  | welcomeimagehtml |
| Welcome page image/flash URL |  |  |  | X |  | welcomeimageurl |
| Add to Cart button | X |  |  |  |  | addtocarthtml Use between <table> and </table> tags. |
| Add to Cart button (HTML for how it appears on an item drilldown | X |  |  |  |  | addtocartdrilldownhtml |
| Add to Cart button (HTML for how it appears on an item list page) | X |  |  |  |  | addtocartlisthtml |
| Add to Cart button (HTML for how it appears in dense lists) | X |  |  |  |  | denselistaddtoccartbuttonh |
| Add to Cart button with options | X |  |  |  |  | addtocartoptionshtml |
| Add to Cart quantity (HTML for how quantity field for add to cart appears on dense lists) | X |  |  |  |  | denselistaddtocartquantityh |
| "Out of Stock" message if the quantity on hand is at or below 0 | X |  |  |  |  | stockstatusmessagehtml |
| 'Tell A Friend' link | X |  |  |  |  | tellafriendlinkhtml |
| Upsell related items together with item you add to the Related Items subtab on item records. | X |  |  |  |  | allrelateditemshtml |
| URL Address of the item referenced | X |  |  |  |  | storeurl |

### Related Topics

-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)
-   [Declare Attribute Tags for Tags Within Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628302.html)
-   [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html)
-   [Using the Server-Side Include Tag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2629027.html)
-   [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html)
-   [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
