---
id: "section_N2564504"
type: "section"
title: "Web Site Appearance Preferences"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Web Site Record Settings > Web Site Appearance Preferences"
parent: "chapter_N2561820"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2564504.html"
anchors: ["bridgehead_N2565829", "bridgehead_N2566088", "bridgehead_N2566480", "bridgehead_N2566782", "bridgehead_N2567005", "bridgehead_10113502472", "bridgehead_N2567315"]
sha256: "ad23e1753da259d2fdc8781b68b8e6773e869738246f32c26caf75c68a8b35d8"
---

Go to _Commerce > Websites > Website List_ and click Edit next to your website. Then click the Appearance subtab to set appearance preferences for your **Site Builder** website. Here you can select the color theme, site theme, and a logo for your site.

In **SuiteCommerce Advanced**, the appearance of your web site is entirely controlled by site template files that you create or install as part of your implementation. None of the settings on the Appearance subtab are supported by SuiteCommerce Advanced.

To learn more about your options for Site Builder site customization, see [Site Builder Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2601007.html), and [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html).

Note:

Appearance preferences set for external web sites (WSDK) are applied only to the shopping cart and checkout pages.

Refer to the following tables for detailed descriptions of appearance settings for Site Builder web sites:

-   [Colors and Logo](#bridgehead_N2565829)
    
-   [Web Site Templates](#bridgehead_N2566088)
    
-   [Page/Fonts](#bridgehead_N2566480)
    
-   [Portlets and Navigation](#bridgehead_N2566782)
    
-   [Shopping Cart](#bridgehead_N2567005)
    
-   [Adding a 'Tell A Friend' Link](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603455.html)
    
-   [Web Site Language Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2567348.html)
    
-   [Site Builder: Tabs](#bridgehead_N2567315)
    

## Colors and Logo {#bridgehead_N2565829}

Set preferences for the color theme on your web site, your web site logo, and the page or site shoppers see when they click on your logo image.

| Preference | Description |
| --- | --- |
| Web Site Color Theme | Select a color theme for your site. This preference overrides the color set by the site theme. In an External Catalog site (WSDK), this setting only affects the shopping cart and checkout pages. For more information, see [Changing Website Color Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603251.html). |
| Web Site Logo | Select a logo from the File Cabinet to appear in the header of your site. For more information, see [Uploading and Setting Your Logo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542584.html). In an External Catalog site (WSDK), this setting only affects the shopping cart and checkout pages. |
| Logo Link URL | Enter the URL you want to link your logo to. If you don't want to link your logo, leave this field blank. |
| Web Site Logo Alignment | Choose to align your logo to the center, right or left side of the page. In an External Catalog site (WSDK), this setting only affects the shopping cart and checkout pages. |

## Web Site Templates {#bridgehead_N2566088}

Select the web site templates for your site. You can use the basic NetSuite templates, or use the Advanced Site Customization feature to create your own. For more information, see [Site Builder Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2601007.html).

| Preference | Description |
| --- | --- |
| Web Site Theme | Select the template, or style, you want to use for your web site. Click Preview to see what a theme looks like in a new window. If you use Advanced Site Customization, you can view, edit, and create themes at _Commerce > Site Builder > Appearance > Themes_. For more information, see [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html). Select None to use a basic site without customization. |
| Default Item Drilldown Template | Select a template that defines how items you sell should appear in your web site. If you use Advanced Site Customization, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html). This preference overrides the default template for the site theme. |
| Default Info Item Drilldown Template | Select an item/category template that defines how information items should appear in your site. This preference overrides the template set for a theme. |
| Default Item List Layout | Choose a default layout for item lists. Changing this setting overrides the default layout for the site theme. For more information on setting up layouts, see [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html). |
| Default Category List Layout | Choose a default layout for category lists. Changing this setting overrides the default layout for the site theme. |
| Default Related Items Layout | Choose a default layout for your lists of related items. Changing this setting overrides the default layout for the site theme. |
| Default Upsell Items Layout | Choose a default layout for your lists of Upsell items. Changing this setting overrides the default layout for the site theme. |

## Page/Fonts {#bridgehead_N2566480}

Set preferences for page width, alignment, and font for your web site.

| Preference | Description |
| --- | --- |
| Page Width | Enter a width in pixels to keep your site content at a static, unchanging width. |
| Page Alignment | Select how to align your site content in the browser window. |
| Website Font | Select the text font to use for all text in your site. In an External Catalog site (WSDK), this setting only affects the shopping cart and checkout pages. |
| Description Font Size | Enter the font size for your tab, category, and item description text. |
| Title Font Size | Enter the font size for item and category titles in your site. |
| Zoom | Select magnification for customers viewing your site. |

## Portlets and Navigation {#bridgehead_N2566782}

Choose which portlets are displayed on your site.

| Preference | Description |
| --- | --- |
| Show Search | Check this box to display the Search portlet, which customers can use to search your site. You can select custom search forms on the Search subtab. |
| Show Web Site Currency | Check this box to let your shoppers choose the currency to use when shopping in your store. When you check this, your customers select their currencies on your site's Home page. After a currency is selected, all item prices will appear in the currency your customer has chosen. In an External Catalog site (WSDK), you can add a link so shoppers on your site can see prices in a certain currency. For example: **http://yourstore.com/site/index.html?currencykey=2**. Note the currency key is the ID for the currency record. |
| Show Navigation Portlet | Check this box to show a menu of your categories and items on the left side of your web site so that customers can navigate through your categories and items. If you do not have legacy settings for your navigation and use the Advanced Site Customization feature, you can set preferences for this portlet on site themes. |

## Shopping Cart {#bridgehead_N2567005}

Select preferences for your Site Builder shopping cart display on the Web Site Setup page.

In SuiteCommerce Advanced, the appearance of your shopping cart and checkout is entirely controlled by site template files that you create or install as part of the checkout reference implementation. For more information, see [Set Up SCA Developer Tools](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2673589.html).

For more configuration options for Site Builder shopping cart and checkout, see [Shopping Cart and Checkout Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2571737.html).

| Preference | Description |
| --- | --- |
| Show Cart Summary | Check this box to include the Shopping Cart portlet in your web site. This portlet shows what customers currently have in their shopping carts. |
| Site Uses Cart Summary Tags | Check this box if you use Advanced Site Customization and your site uses shopping cart summary tags. For more information, see [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html). |
| Show Shipping Estimator in Cart | Check this box to give customers an estimate of shipping costs before they complete shipping information in checkout. The lowest estimated shipping cost is displayed by default. If you offer real-time rates, a customer can enter a zip code to receive an estimate. If the order qualifies for free shipping, 'Free Shipping' is displayed. |
| Show Extended Cart | Check this box to enable customers to add coupon code, gift certificate, and shipping information on the shopping cart page. |
| Display Order of Cart Items | To customize the order of items in the shopping cart, select one of the following: **Most Recently Added First** - Every time an item is added to the cart, it is added to the top of the list of items in the shopping cart. **Most Recently Added Last** - Every time an item is added to the cart, it is added to the bottom of the list of items in the shopping cart. |

## Tell a Friend {#bridgehead_10113502472}

Checking the Show 'Tell a Friend' Link box adds a 'Tell A Friend' link to the detailed description page for each item.

For more information, see [Adding a 'Tell A Friend' Link](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603455.html).

## Site Builder: Tabs {#bridgehead_N2567315}

On the Tabs subtab, only available for Suite Builder, you can arrange the tabs in your web site to appear in the order you want. For more information, see [Organizing Presentation Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595616.html#bridgehead_N2596056).

### Related Topics

-   [Web Site Setup Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2562624.html)
-   [Web Site Language Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2567348.html)
-   [Site Builder Web Site Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2561820.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
