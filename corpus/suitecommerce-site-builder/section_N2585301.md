---
id: "section_N2585301"
type: "section"
title: "Displaying Items and Information"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Items, Forms, & Images > Displaying Items and Information"
parent: "chapter_N2582621"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585301.html"
anchors: ["section_N2177433", "bridgehead_4466509194", "bridgehead_N2177698", "bridgehead_N2177736", "bridgehead_N2177872", "bridgehead_N2178054", "bridgehead_N2585483"]
sha256: "07ee7f873a7f5a99e9fe0dbbd292fd752e0cb22bfa679c9f3493b45faedc9c31"
---

NetSuite offers several optional methods for creating item records for the products you want to sell on your NetSuite web store:

-   Import items in CSV format at Setup > Import/Export > Import CSV Records. An administrator can perform imports.
    
-   Enter item records at _Lists > Accounting > Items_. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
-   Enter item records using the Web Site Content Manager at _Commerce > Site Builder > Content Management > Content Manager_. For more information, see [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html).
    

If you use the Web Site feature only, items you display in your site are not for sale. If you use the Web Site feature with the Web Store feature, items you display are offered for sale in your store, using the preferences on the **Web Store** subtab of item records.

You can create an information item to display contact numbers, directions, and business hours on your site. See [Information Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2589098.html).

## Setting Up Items for the Web Site {#section_N2177433}

When you set up items to display on your Web site, visitors to your site, can click a link to an item, see the item display page, and potentially submit an order for the item. To display an Item in your Web store, you must complete the following tasks on the item record:

-   On the **Pricing** subtab, enter a price for the item.
    
-   On the **Web Store** subtab:
    
    -   Select a **Site Category** to display the item.
        
    -   Check the **Display in Web Store** box.
        

After you complete the tasks above, the item displays on your Web site or Web store. Use the **Web Store** subtab on item records to set other aspects of the item page display.

1.  Go to _Lists > Accounting > Items_.
    
2.  On the item record, click the **Web Store** subtab.
    

## Web Store Display {#bridgehead_4466509194}

1.  In the **Page Title** field, enter the text you want to appear in the upper-left corner of an Internet browser when customers view this item in your Web store. This should be a descriptive title for the item page. It can help achieve better results with search engine ranking.
    
2.  In the **Web Store Display Name** field, enter the name to show in the Web site for this item.
    
3.  In the **Web Store Description** field, enter a brief description of this item to show under the web store display name.
    
4.  In the **Detailed Description** field, enter details about the item to show when a site visitor clicks the display name for the item.
    
5.  The description fields can have letters, numbers, and basic punctuation. You can also enter basic HTML codes like lists, bold characters and underlines. You can enter 999 characters in the **Store Description** field and 1,300 in the **Detailed Description** field.
    
6.  In the **Featured Description** field, if this item is displayed on the home page of your Web site, enter a featured description for this item. This description appears below the item's store display name on the Home page of your store or site.
    
7.  You can enter up to 999 characters including basic HTML code.
    
8.  Enter and format text using the formatting options, or click the **HTML Source Code** link to enter HTML.
    
9.  In the **Item Drilldown Template** field, select an HTML template to set the look and feel of the item page when displayed in your site.
    
10.  If you do not select a template here, the item template used by default is the one you select on the **Appearance** subtab of your website record at _Commerce > Websites > Website List_.
     
11.  If you use the Advanced Site Customization feature, you can create and edit HTML item templates at _Commerce > Site Builder > Appearance > Item/Category Templates_ . For more information, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).
     
12.  Use the fields listed below to choose an image to show with an item on your site. You must upload images to your NetSuite File Cabinet before you can select them on item records.
     
13.  For more information, see [Using Images in your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592719.html).
     
     -   **Item Display Image** - Select an image to show on the item display page.
         
     -   **Item Display Thumbnail** - Select an image to show with the item before a customer clicks the item for more information.
         
14.  After you have selected the appropriate settings for all necessary fields on the record, click **Save**.
     
     Note:
     
     The fields described below offer optional settings for items you publish on your Web site.
     

## Specials Display {#bridgehead_N2177698}

-   If you want to place this item on special, check the **On Special** box. The item then appears in the Specials category in your store or site. For more information, see [Using the Specials Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597344.html).
    
-   If you checked the **On Special** box, enter a specials description for this item. This description appears under the item's store display name in the Specials category of your store or site.
    
    You can enter letters, numbers and basic HTML code. To eliminate the need for HTML code, clear the **View as HTML** box, and then enter and formatted text.
    

## Stock and Pricing Behavior {#bridgehead_N2177736}

The fields listed below specify the out of stock message for a particular item. The settings here override the default behavior you set on the Web Site Setup page. For more information, see [Setting Web Store Back Order and Out-of-Stock Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2582357.html).

-   **Out Of Stock Message** - Enter a message to override the NetSuite default out of stock message. This field is only displayed if you use the Advanced Site Customization feature.
    
-   **Out of Stock Behavior** - Choose what you want to happen when a Web store shopper orders an item that is out of stock. The Default option applies the behavior you selected on the **Shopping** subtab of the Set Up Web Site page. Go to at _Commerce > Websites > Website List_.
    

Use the fields listed below if you allow customers to set the price for an item. For example, customers may be allowed to set the price they want to pay for tickets to a fund raising event.

-   **Variable Amount** - Check this box to allow the customer to set the price for the item.
    
-   **Show Default Amount** - Check this box if customers are allowed to set the price for the item, but you want to show a certain price as the default amount.
    
-   **Maximum Variable Amount** - Enter the maximum amount that can be paid or donated for this item.
    

Use the fields listed below, if you do not want to display the price of a particular item on your Web site. For global settings you can use, see [Showing Items Without Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2586122.html).

-   **Don't Show Price** - Check this box to hide the price of an item online.
    
-   **No Price Message** - Enter the message that should show on the Web site instead of the price. For example, you might enter 'Call for Price.'
    

## Search Engine Optimization (SEO) and Product Feeds {#bridgehead_N2177872}

Use the fields listed below to help customers find items in your site.

-   **Meta Tag HTML** - Enter HTML for the head section of this item page, including Meta Tag keywords. This can help achieve better ranking with search engines. For more information, see [Adding META Tags in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636604.html).
    
-   **URL Component** - Enter a descriptive name for this item to appear in the URL for the item page. For more information, see [Descriptive URLs in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2637101.html).
    
-   **Search Keywords** - Enter alternate words that customers might use to search for this item in your Web site. These can include, abbreviations, misspellings, and acronyms. For more information, see [Setting Up Alternate Search Keywords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635042.html).
    
-   **Exclude From Sitemap** - Check this box to exclude a tab, category or item page from the site map. For more information, see [Using the Sitemap Generator in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645633.html).
    
-   **Sitemap Priority** - Use the Sitemap Priority list to indicate the relative importance of your Web site URLs.
    
    You can select a priority ranging from 0.0 to 1.0 on item, category, and tab records.
    
    NetSuite assigns the default priority **Auto** to all new and existing tab, category and item records in your account. The priority is calculated based on the position of the item or category in the hierarchy of your Web site.
    
    For example, your Web site tabs automatically generate a default priority value of 1.0 because they are top level pages. A category published to a tab gets a priority of 0.5. An item published to a category on a tab gets a priority of 0.3.
    

Use the fields listed below if you want to include an item in a product feed for upload to a shopping comparison Web site. For more information, see [Setting Up Website Product Feeds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639492.html).

These are optional fields that are only displayed for the following item record types: Kit/Package, Non-inventory Item for Sale, Non-inventory Item for Resale, Assembly (lot and serialized), Inventory (lot and serialized).

-   **Product Feed** - Select the sites for which you are creating a product feed that includes this item. Press CTRL to select more than one site at a time.
    
-   **Shopping.com Category** - Enter the name of the shopping.com category where the item should be displayed.
    
-   **Shopzilla Category ID** - Enter the category ID provided by Shopzilla for the item.
    
-   **NexTag Category** - Enter the Nextag category name where the item should be displayed.
    

## Web Site Categories {#bridgehead_N2178054}

On the Web Site categories subtab, use the Site Category list to select and add each category or tab where you want to publish this item in your Web store. For more information see [Site Builder Tabs & Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2595349.html).

If this item appears in multiple categories, use the **Preferred Category** column to designate a category for the canonical URL that points to this item on your Web site. The canonical URL is favored by Google for indexing your site and it eliminates exposure of duplicate content to any search engine indexing your Web site.

For more information, see [Using Canonical URLs in NetSuite Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636921.html).

## Publishing Items and Information to Tabs and Categories {#bridgehead_N2585483}

After you have set up item records and information item records, you must publish tabs and categories on your web store. Items and information are displayed in site in categories. Each category you create must be placed on a tab. Your website comes with two tabs-Catalog and Information. However, you can edit the names of these tabs and create new tabs to display in your website.

1.  Create a **presentation tab**. For more information, see [Creating Website Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595492.html).
    
    To publish information to the default Catalog or Information tabs, you can skip step one and go directly to creating categories.
    
2.  Create **categories** to publish on that tab. For more information, see.[Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html).
    
3.  Publish items to web store categories. For more information, see [Adding Items to Web Store Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585643.html).
    

Alternatively, you can create and edit tabs and categories using the Site Content Manager. For more information, see [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html).

You can now continue to create tabs and categories to publish information to your website. You can also create more specific subcategories to place in the categories you have already published.

For example, you can create a tab named Return Policies and a category for that tab, Cash Refunds. Then, create a category named Returns with a Receipt, and select Cash Refunds in the Subcategory of field. Returns with a Receipt is now a subcategory of Cash Refunds. You can then create other subcategories, such as Returns without a Receipt, each with specific information.

In addition to publishing tabs and categories to your website, you can publish them in the following places:

-   **Intranet Only** - If you have the Intranet feature enabled, clear the **Display in Web Site** box when creating a tab or category to display the information to only those people you select on the **Audience** subtab. Audience members you select must log in to your account to see the tab or category. If you select a particular role, that person must be logged in with that role to see the tab or category.
    
-   **Both Web Site and Intranet** - Select the **Display in Web Site** box and choose individuals or groups on the **Audience** subtab. The tab or category then shows both internally to those you select on the **Audience** subtab and to everyone who visits your website.
    

### Related Topics

-   [Adding Items to Web Store Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585643.html)
-   [Featuring Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585769.html)
-   [Customizing Items in Your Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2586028.html)
-   [Related Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520957621.html)
-   [Information Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2589098.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
