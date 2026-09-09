---
id: "section_N2596427"
type: "section"
title: "Creating Site Categories"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Tabs & Categories > Creating Site Categories"
parent: "chapter_N2595349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html"
anchors: ["bridgehead_N2596507", "procedure_N2596526", "procedure_N2596718", "procedure_N2596823", "bridgehead_N2596871", "bridgehead_N2596890", "bridgehead_N2596914"]
sha256: "c16562c27602caf22b5176941ab835fe74e2ddfe55371bdb530054802f2ea2c3"
---

To organize information and items for sale on your website, place them in categories. Categories must be associated with presentation tabs for them to display on your website.

For example, a buyer can click on the **Cameras** category to see a list of products available.

Use the presentation tab record to organize which categories display on a tab and in which order. For more information, see [Arranging Web Store Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597170.html).

If your NetSuite account was created prior to 2007, you can use the Specials category to display certain items on your website. For more information, see [Using the Specials Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597344.html).

## Adding Items to Site Categories {#bridgehead_N2596507}

Use the Basic subtab on the category record in NetSuite to choose items and subcategories for display in a certain category.

To make sure your web store pages load as quickly as possible, do not place more than 50 items in each category. Set up enough categories and subcategories to make browsing easier for your customers. The Web store displays up to 1,000 items per category. Although you can add more than 1,000 items to a category, any items over that limit are displayed only in search results.

Note that when editing and saving a category with more than 10,000 items, any changes you make to the sublist are not processed or saved. Editing tasks include: adding new items, deleting old ones, and reorganizing items in the category. This is done to reduce the potential for slow Web site performance.

#### To create a category: {#procedure_N2596526}

1.  Go to _Commerce > Site Builder > Content Management > Categories_.
    
2.  You can also create new categories using the Web Site Content Manager at _Commerce > Site Builder > Content Management > Content Manager_. In the New header, click Category.
    
    For more information about the Content Manager, see [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html).
    
    Or, you can use the Import Assistant to import site category data into NetSuite from CSV file contents. See [Site Category Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433181.html).
    
3.  On the Site Category page, enter a name in the **Category** field.
    
4.  Select the site where you want the category to display.
    
5.  In the **Subcategory of** field, choose a tab or parent category from the list.
    
    For example, if this is a category you want to appear on your Catalog tab, select Catalog.
    
6.  In the **Category List Layout** field, select a layout for the list of subcategories you place in this category.
    
    Category layouts allow you to customize your site by presenting your categories and category lists in the design of your choice. For more information on layouts, see [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html).
    
7.  In the **Item List Layout** field, select a layout for the list of items you place in this category.
    
8.  In the **Related Items List Layout** field, select a layout for your related items list. Use related items to cross-sell items that complement each other. For more information, see [Related Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2586873.html).
    
9.  Check the **Display in Web Site** box to display this category to everyone who visits your site.
    
10.  Click **Save** to make the category available on your website.
     

Note:

For the fields listed under the Audience subtab, if you enable the Select All option for a field that does not have any value listed under it, the items in this category or sub category will not be displayed on your website.

To remove this category from your site, check the Inactive box on the category record or click the Delete button. To display the category in an intranet site in your NetSuite account, make a selection on the Audience subtab. For more information, see [Publishing Categories Internally](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597878.html#bridgehead_N2598069).

Use the subtabs on the category record to add content.

#### Basic Subtab {#procedure_N2596718}

1.  On the **Basic** subtab, write brief and detailed descriptions in the appropriate fields.
    
    Brief descriptions display on your website directly below the category name and can have 999 characters. Detailed descriptions can have 4,000 characters. The detailed description displays on the item list page where customers add items to the shopping cart.
    
    Description fields can have letters, numbers, punctuation, and HTML. For more information, see [Using HTML in Description Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2589998.html).
    
2.  In the **Page Title** field, enter a name for your website page. This will appear in the HEAD element of the HTML source code for the website page. For more information, see [Adding Page Titles in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636435.html).
    
3.  In the **Meta Tag HTML** field, enter a META tag for the category which is added to the HEAD element of the HTML source code for the page. For more information, see [Adding META Tags in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636604.html) **.**
    
4.  If you use the Descriptive URL feature, the **URL Component** field displays. Enter a name for this category that you want to show in the URL that points to the page. If you leave this field blank, the category name is used.
    
    Note:
    
    The name you use as a URL component cannot be a reserved character string in the NetSuite application. If you enter a reserved character string, then you will be notified with a popup alert message. You can enter a different URL component to continue.
    
    For more information see [Descriptive URLs in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2637101.html).
    
5.  In the **Search Keywords** field, enter alternate names for this category that customers can use in the Search field on your web store to find this category. For more information, see [Setting Up Alternate Search Keywords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635042.html).
    

At the bottom of the Basic subtab, add the items you want to appear in this category.

#### Media Subtab {#procedure_N2596823}

1.  Select a thumbnail image for your category in the **Thumbnail** field. This thumbnail appears with your category in your website.
    
2.  Select an image for your category in the Image field. This image only appears in your website with a layout that uses full-size images. If you select an image and do not select one of the Basic layout templates, or a custom layout template that you create, only the thumbnail image appears.
    
    For more information about layout templates, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).
    
    You can set default sizes for images. For more information on setting default sizes for images, see [Resizing Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2594819.html).
    

## Audience Subtab {#bridgehead_N2596871}

In the Audience subtab, select individual names or group names to give them access to this Category. If you select a group, employee, and a partner, the user must be a member of the group or be the employee selected or be the partner selected to access this Category.

The Groups list contains both static and dynamic groups. If you publish a category to a dynamic group, for performance reasons, the tab's audience is a snapshot of the dynamic group members. The snapshot is updated twice a day.

Don't enable the Select All option for the fields that don't have values listed under them. If you enable the Select All option for such fields, the items in this category or sub category will not be displayed on your website.

If you want to publish this category to an intranet, see [Publishing Categories Internally](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597878.html#bridgehead_N2598069).

## Translation Subtab {#bridgehead_N2596890}

If you use the Multi-Language feature, the **Translation** subtab will appear after saving a new category record. You can enter translated text for specific fields. For more information, see [Setting Up a Site for Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2463004.html).

## Tag Substitution Subtab {#bridgehead_N2596914}

If you use Advanced Site Customization, the **Tag Substitution** subtab will appear after saving a new category. See [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html) for information on substituting custom tags.

### Related Topics

-   [Arranging Web Store Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597170.html)
-   [Using the Specials Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597344.html)
-   [Publishing an Employee Directory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597708.html)
-   [Creating Website Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595492.html)
-   [Publishing Information to an Internal Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597878.html)
-   [Site Builder Tabs & Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2595349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
