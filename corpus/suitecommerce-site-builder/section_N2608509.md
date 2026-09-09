---
id: "section_N2608509"
type: "section"
title: "Displaying Price Levels and Sale Prices"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Displaying Price Levels and Sale Prices"
parent: "section_N2603624"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2608509.html"
anchors: []
sha256: "2dac9c1ca34b4bc7b27d5603b3a2a6bcd73f7b55ffc51cc2245fe331025070fc"
---

You can display multiple price levels for items on website pages. This enables you to display both the original and sale prices for items. When you update price levels in your account, the items in your site are automatically updated.

Sale prices and other price levels can be added to item pages using item/category templates. Use the **<%=getCurrentAttribute('item','pricelevelx')%>** tag to display item prices, where **x** is replaced with the ID number for the price level.

For example, because the default ID for the online price is **5,** the tag attribute is **pricelevel5**. The IDs of alternate sales prices increase by one between the base price and the online price. For the price levels included in your account, the attributes are as follows:

| Price Level | Attribute |
| --- | --- |
| Base Price | pricelevel1 |
| Alternate Price 1 | pricelevel2 |
| Alternate Price 2 | pricelevel3 |
| Alternate Price 3 | pricelevel4 |
| Online Price | pricelevel5 |

If you use custom price levels in addition to the default levels, you can view their respective IDs at _Setup > Accounting > Accounting Lists_. Select Price Level in the Type filter at the bottom of the page.

Note:

Internal IDs only show in lists when you have the Show Internal IDs box checked at Home > Set Preferences.

Use the following code sample as a guide for creating an item/category template with both a sale price and an original price:

          `<td>    <h2><%=getCurrentAttribute('item','itemid')%>       <%=getCurrentAttribute('item','stockstatusmessagehtml')%>    </h2>    <br><%=getCurrentAttribute('item','storedetaileddescription')%>    <br><br>    Was <s><%=getCurrentAttribute('item','pricelevel1')%></s>!     Now Only <%=getCurrentAttribute('item','pricelevel5')%>    </h3>    <br>    <table><%=getCurrentAttribute('item','addtocarthtml')%>    </table>    <br>    <%=getCurrentAttribute('item','storedisplayimagehtml')%> </td>` 
        

### Related Topics

-   [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html)
-   [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html)
-   [Adding a Style Sheet to Your Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2608851.html)
-   [Using Web Site Text Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2609031.html)
-   [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603624.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
