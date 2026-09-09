---
id: "section_N2630406"
type: "section"
title: "Tags for Use in HTML Pages and Site Templates"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Tags for Use in HTML Pages and Site Templates"
parent: "chapter_N2615371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html"
anchors: []
sha256: "7e0751368bc75d31a1c444c07f783fd3a73f2caeae2e779cf4dde65dcd449056"
---

NetSuite Web Site Tags let you to show tab, category, and item information in HTML files you host in the file cabinet or in custom HTML for your Web Site Themes.

To use Web Site Tags, the Advanced Site Customization feature must be enabled in your NetSuite account. To host HTML files in the file cabinet, you'll need to use the Host HTML Files feature. To enable these features, go to the Web Presence subtab at Setup > Company > Enable Features.

Important:

Web Site tags aren't supported in SuiteCommerce Advanced websites.

You can use Web Site Tags to:

-   Edit or customize site themes
    
-   Connect a site you host in NetSuite with a NetSuite shopping cart, checkout or other presentation tabs
    

The table below shows each Web Site Tag, where you can use the site theme fields, and what it does. Each tag is shown in two formats. You can use tags in HTML files hosted in NetSuite or in site themes, in either format shown below.

| **Tag** | **Site Theme Field** | **What it Does** |
| --- | --- | --- |
| 
<NLTABID>

<%=getTabID()%>



 | Active Tab Inactive Tab | Returns the unique internal ID for the current tab |
| 

<NLTABLABEL>

<%=getTabLabel()%>



 | Active Tab Inactive Tab | Replaces the default label of a tab with the name you have chosen for the tab. |
| 

<NLTABLINKURL>

<%=getTabLinkURL()%>



 | Active Tab Inactive Tab | Places a navigation URL to view a page under a tab. Use this tag within an href of an <a> tag. |
| 

<NLTABLINKATTRIBS>

<%=getTabLinkAttribs()%>



 | Active Tab Inactive Tab | Gives rollover attributes to your tab. Use within an href of an <a> tag. |
| 

<NLADDTOCARTOPTIONS>

<%=getAddToCartOptions()%>



 | Add To Cart Button | Lists item options that have been selected on the Add to Cart button. |
| 

<NLADDTOCARTITEMID>

<%=getAddToCartItemID()%>



 | Add To Cart Button | Lists the item name on the Add to Cart button. |
| 

<NLADDTOCARTCLICKSCRIPT>

<%=getAddToCartClickScript()%>



 | Add To Cart Button | Adds JavaScript to make your custom Add To Cart button add the item to the shopping cart. A mandatory tag if you are customizing the button. |
| 

<NLADDTOCARTQUANTITY>

<%=getAddToCartQuantity()%>



 | Add To Cart Button | Shows the quantity of items that will be added on the Add To Cart button. |
| 

<NLADDTOCARTSUBMITSCRIPT>

<%=getAddToCartSubmitScript()%>



 | Add To Cart Button | Adds JavaScript to check mandatory fields for adding the item, such as item options. Not for use with buttons on dense lists. |
| 

<NLCOMPANYID>

<%=getCompanyId()%>



 | Any | Adds your company ID. Use this tag to generate company-relative URLs in accounts that copies are made from. Do not hard code the company ID. |
| <NLPROCESSONCE> | Any | Use this tag to surround HTML code in all areas of the site theme. When the page is displayed, only the first portion of HTML surrounded by the NLPROCESSONCE tag is shown. Subsequent blocks of HTML surrounded by the NLPROCESSONCE tag will not be displayed. For example, when you customize a site theme, you may see an image or a greeting message displayed twice. Use the NLPROCESSONCE to resolve the problem. |
| <%=getOnlineFormLinkHtml( _formid_ )%> | Any | Renders the <href> to create a link from a hosted HTML page, or a tab, or category record to an online form. This tag preserves incoming URL parameters, such as lead source, partner, and promotion code. Using this tag ensures that analytics data is automatically transferred across domains. For more information, see [Web Analytics and Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2654243.html).

Replace **formid** with the number found in the form's URL after "formid=.' Use this syntax to create a link to an online form:

**<%=getOnlineFormLinkHtml(7)%></a>**



 |
| <%=getOnlineFormLinkHtml( **formid, subsidiary ID** )%> <%=getOnlineFormLinkHtml( **formid**, 'default')%> | Any | If you use a OneWorld account, use the tag that includes the **subsidiary ID**, to record a subsidiary on the form.

For example, use this syntax to create a link to an online form:

**<%=getOnlineFormLinkHtml(7, 99)%></a>**

When a visitor to the site submits the online form, the subsidiary (with ID=99) is recorded on the form.

Use **'default'** in the tag to record the subsidiary ID of the account where you created the online form, for example,

**<%=getOnlineFormLinkHtml(7,'default')%></a>**



 |
| <%=getOnlineFormUrl( **formid** )%> | Any | Use within an <href> in a hosted HTML page on your website, to render a link to an online form. Use this tag instead of a hard-coded link to the online form, as this tag preserves incoming URL parameters you may want to pass on to the online form, such as lead source, partner, and promotion codes.

Replace **formid** with the number found in the form's URL after "formid=.' Use this syntax to render a link to an online form:

**<a href='<%=getOnlineFormUrl(7)%>'></a>**



 |
| <%=getOnlineFormUrl( **formid, subsidiary ID** )%> <%=getOnlineFormUrl( **formid**, 'default')%> | Any | If you use a OneWorld account, use the tag that includes the **subsidiary ID**, to record a subsidiary on the form.

For example, use this syntax to create a link to an online form:

**<a href='<%=getOnlineFormUrl(7,99)%>'></a>**

When a visitor to the site submits the online form, the subsidiary (with ID=99) is recorded on the form.

Use **'default'** in the tag to record the subsidiary ID of the account where you created the online form, for example,

**<a href=**

**'<%=getOnlineFormUrl(7,'default')%>'></a>**



 |
| 

<NLITEMLIST>

<%=getItemList()%>



 | Content Area | Returns the list of items or categories for the page. When you create a template for category list pages, you must include the <NLITEMLIST> tag in the template HTML so that categories display properly on the page. |
| 

<NLCOLUMNCONTENTS>

<%=getColumnContents()%>



 | Content Area Left-Side Navigation Right-Side Navigation | Adds lists of items according to the tab being viewed. This tag is **required** for your site to display content from your account. |
| 

<NLCURRENCYSELECTHTML>

<%=getCurrencySelectHTML()%>



 | Currency Select Portlet | Returns the currency selector portlet. |
| 

<NLPORTLETTITLE>

<%=getPortletTitle()%>



 | Default Portlet | Place this tag within HTML for a portlet template to add a title for the portlet. You must use this tag between <table> and </table> tags. |
| 

<NLPORTLETCONTENTS>

<%=getPortletContents()%>



 | Default Portlet Cart Summary Portlet Currency Select Portlet Language Select Portlet Search Portlet Search Form Portlet Site Navigation Portlet | Place this tag within HTML for a portlet template to add the contents of the portlet. You must use this tag between <table> and </table> tags. |
| 

<NLCARTTOTAL>

<%=getCartTotal()%>



 | Header Sidebar | Adds the monetary total for all items in the cart, including the currency symbol, for the current site visitor. |
| 

<NLCARTITEMCOUNT>

<%=getCartItemCount()%>



 | Header Sidebar | Adds the number of items in the cart for the current site visitor. |
| 

<NLCARTSUMMARYHTML>

<%=getCartSummaryHTML()%>



 | Header Sidebar | Adds the Cart Summary portlet for the current customer's shopping cart. This tag must be used between <tr> and </tr> tags. |
| 

<NLCARTDISCOUNTEDTOTAL>

<%=getCartDiscountedTotal()%>



 | Cart Summary Portlet | Shows the discounted total before tax. The amount shown equals the item subtotal minus the applied discount. Note: This tag only calculates discounts related to promotion codes. Gift certificates are not included. |
| 

<NLCARTAPPLIEDDISCOUNT>

<%=getCartAppliedDiscount()%>



 | Cart Summary Portlet | Shows the discount applied to the order. This tag only calculates discounts related to promotion codes. Gift certificates are not included. The discount amount displayed using this tag matches the discount amount displayed on the Review & Submit page. Note: The tax amount displayed with this tag depends on whether the discount associated with the promotion code is marked Before Tax or After Tax. |
| 

<NLCARTAPPLIEDGC>

<%=getCartAppliedGC()%>



 | Cart Summary Portlet | Shows the gift certificate applied to the order. This is the total amount of gift certificates applied. |
| 

<NLCARTSHIPPING>

<%=getCartShipping()%>



 | Cart Summary Portlet | Shows the estimated shipping amount for the order. This tag shows the shipping cost. Handling is not included. Note: This tag includes tax on shipping items, only for Australian companies that collect tax on shipping. |
| 

<NLCARTSHIPPINGHANDLING>

<%=getCartShippingHandling()%>



 | Cart Summary Portlet | Shows estimated shipping and handling. This tag shows the shipping and handling cost. This amount matches the amount displayed on the Review & Submit page. Note: This tag includes tax on shipping items, only for Australian companies that collect tax on shipping. |
| 

<NLCARTTAX>

<%=getCartTax()%>



 | Cart Summary Portlet | Shows the estimated tax on the order. This tax amount matches the tax amount displayed on the Review & Submit page. |
| 

<NLCARTGRANDTOTAL>

<%=getCartGrandTotal()%>



 | Cart Summary Portlet | Shows the grand total in the shopping cart. This total amount matches the total amount displayed on the Review & Submit page. |
| 

<NLLANGUAGESELECTHTML>

<%=getLanguageSelectHTML()%>



 | Left-Side Navigation | Shows a field where visitors can select another language for viewing your site. You must have the Multi-Language feature enabled and set up to use this tag. |
| 

<NLPAGELINKS>

<%=getPageLinks()%>



 | Logo and Tabs | Creates links for customers to register or log in. This tag must be used between <tr> and </tr> tags. |
| 

<NLUSERINFO>

<%=getUserInfo()%>



 | Logo and Tabs | Places a greeting with the customer's name who is currently logged in, or places text and a link, 'Returning customers click here to log in.' This tag must be used between <td> and </td> tags. |
| 

<NLUSERINFO2>

<%=getUserInfo2()%>



 | Logo and Tabs | This tag returns Register and Log In links for site visitors who are not recognized and returns recognized visitors' first and last names in a Welcome message. |
| 

<NLPAGETOP>

<%=getPageTop()%>



 | Logo and Tabs | Adds your logo, default tabs and default links to the top of the page. This tag must be used within <table> and </table> tags. |
| 

<NLPAGEHEAD>

<%=getPageHead()%>



 | Logo and Tabs | Adds your custom HTML and META tags in the HEAD element of the HTML page. This replaces NetSuite header information. Note: Without this tag, the HEAD element of the HTML in your custom site will not be used. |
| 

<NLPAGEFULLHEAD>

<%=getPageFullHead()%>



 | Logo and Tabs | Accesses your custom page head and META tag information in addition to NetSuite page head text, script file inclusions and stylesheets. Use this tag instead of <NLPAGEHEAD> if your site uses NetSuite forms, custom fields or portlets. |
| 

<NLWELCOMEIMAGEHTML>

<%=getWelcomeImageHTML()%>



 | Logo and Tabs | Adds the image you have selected on the tab record for the Welcome tab. |
| 

<NLCRUMBTRAIL>

<%=getCrumbTrail()%>



 | Logo and Tabs | Shows breadcrumbs in the top part of website pages. This tag can be added to your Logo and Tabs template. Note: To display all breadcrumbs on all pages, you may need to use or alter a style sheet to ensure the breadcrumb links are a different color from the site background. |
| 

<NLSITELOGOHTML>

<%=getSiteLogoHTML()%>



 | Logo and Tabs | Returns the HTML for the site logo. |
| 

<NLCARTURL>

<%=getCartUrl()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to the Shopping Cart page when you use it with an href. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLCARTLINKHTML>

<%=getCartLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for a link to the shopping cart. For example: `<NLCARTLINKHTML>Shopping Cart</a>`. Note: If you set analytics link attributes at _Commerce > Websites > Website List_, on the Setup subtab, the attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLCHECKOUTURL>

<%=getCheckoutUrl()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to the Checkout page when you use it with an href. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLCHECKOUTLINKHTML>

<%=getCheckoutLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for a link to the Checkout page. For example: `<NLCHECKOUTLINKHTML>Checkout</a>` Note: If you entered analytics link attributes at _Commerce > Websites > Website List_, on the Setup tab, those attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLCUSTOMERCENTERURL>

<%=getCustomerCenterUrl()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to the My Account tab when used within an href. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLCUSTOMERCENTERLINKHTML>

<%=getCustomerCenterLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for a link to the My Account tab. For example: `<NLCUSTOMERCENTERLINKHTML>Customer Center</a>` Note: If you entered analytics link attributes at _Commerce > Websites > Website List_, on the Setup subtab, those attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLLOGINURL>

<%=getLoginUrl()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to the Login page for the web store when used within an href. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLLOGINLINKHTML>

<%=getLoginLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for the login link. For example: `<NLLOGINLINKHTML>Log In</a>`. Note: If you entered analytics link attributes at _Commerce > Websites > Website List_, on the Setup subtab, those attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLLOGOUTURL>

<%=getLogoutUrl()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to log out the current customer and redirect them to your Home page when you place the tag within an href. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLLOGOUTLINKHTML>

<%=getLogoutLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for the logout link. For example: `<NLLOGOUTLINKHTML>Sign Out</a>`. Note: If you entered analytics link attributes at _Commerce > Websites > Website List_, on the Setup subtab, those attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLRELOGINURL>

<%=getReloginURL()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to log out the current customer and redirect them to the Login page when used within an href. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLRELOGINLINKHTML>

<%=getReloginLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for the link to log out the current customer and redirect them to the Login page. For example: `<NLRELOGINLINKHTML>Sign Out</a>`. Note: If you entered analytics link attributes at _Commerce > Websites > Website List_, on the Setup subtab, those attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLREGISTRATIONURL>

<%=getRegistrationUrl()%>



 | Logo and Tabs Left-Side Navigation | Creates a link to the Registration page where customers can enter their preferred login contact information. Place this tag within an href tag. This tag must be used instead of a hard-coded link to ensure security. |
| 

<NLREGISTRATIONLINKHTML>

<%=getRegistrationLinkHtml()%>



 | Logo and Tabs Left-Side Navigation | Use this tag to create an HREF for a link to the Registration page where customers can enter their preferred login contact information. For example: `<NLREGISTRATIONLINKHTML>Register</a>` Note: If you entered analytics link attributes at _Commerce > Websites > Website List_, on the Setup subtab, those attributes are included when bridging from the shopping server to the checkout server on your web store. |
| 

<NLPAGETABS>

<%=getPageTabs()%>



 | Logo and Tabs Left-Side Navigation | Adds HTML for the individual tabs. Use this tag in the Logo and Tabs field for horizontal navigation across the top of the page. Use this tag in the Left-Side Navigation field to display tabs vertically. Must be used between <table> and </table> |
| 

<NLSIDEBARWIDTH>

<%=getSidebarWidth()%>



 | Logo and Tabs Left-Side Navigation Right-Side Navigation Footer | Places a sidebar navigation section in the default width. Use within the width=param or a <td> or <table> to obtain the correct width. |
| 

<NLGLOBALSEARCHHTML>

<%=getGlobalSearchHTML()%>



 | Logo and Tabs Left-Side Navigation Right-Side Navigation Footer Content Area | Includes the standard Search portlet in your website, including hosted pages. This tag returns a <td> of the search form HTML. The search form may be used one time on any page. |
| 

<NLGLOBALSEARCHFORMHTML>

<%=getGlobalSearchFormHTML()%>



 | Content Area Template Search Portlet Search Form Portlet | When you add this tag to a Web Site theme, it displays the search form on all store pages. On order forms in the customer center, and list pages, such as the sales order list on the My Accounts tab or Customer Center, this tag displays a link to the published search form. Note: When a shopper on your site runs the search on any of the following tabs: My Account, Shopping Cart, or Checkout, the search results are displayed on your Home page tab. |
| 

<NLSITENAVIGATIONHTML>

<%=getSiteNavigationHtml()%>



 | Site Navigation Portlet | Returns the navigation portlet. |

### Related Topics

-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)
-   [Declare Attribute Tags for Tags Within Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628302.html)
-   [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html)
-   [Using the Server-Side Include Tag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2629027.html)
-   [Tags for Information Unavailable on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2634674.html)
-   [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
