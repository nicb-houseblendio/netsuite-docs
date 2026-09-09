---
id: "section_N2602488"
type: "section"
title: "Creating and Editing Website Layouts"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Basic Customization > Creating and Editing Website Layouts"
parent: "section_N2602412"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html"
anchors: ["bridgehead_N2602537", "bridgehead_N2602606", "bridgehead_N2602618", "procedure_N2602648", "procedure_N2602698", "procedure_N2602908", "procedure_N2603020"]
sha256: "5da6f448d85a0deb3ffbc9a4af6caae492348ac710cd89aa782e81a10defbb2e"
---

You can use Web site layouts to customize the way items and categories appear in your website.

If you use the Advanced Site Customization feature, you can attach templates for item lists and category lists on the Layout subtab. For more information, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).

If you do not use Advanced Site Customization, you can still change the number of rows, and columns applied to any layout. You can also display numbered page navigation links and links for sorting items on the page.

## Types of Web Site Layouts {#bridgehead_N2602537}

There are several layouts available for basic customization. The list below describes each layout you will find in your account by default:

-   Basic templates - A set of 24 different layouts provided by NetSuite, applicable to item, category, and tab pages.
    
-   Standard Dense List Layout - Displays items in a table format, with cells for item name, description, price, quantity and the Add to Cart button in each row.
    
-   Standard Featured Items Layout - Displays items in a vertical list and shows the image associated with the item, the item name and brief description but omits the Add to Cart button.
    
-   Standard Items/Category Layout - Displays items in a vertical list and shows the image associated with the item, the item name and brief description, and includes the add to cart button.
    

When you customize any one of the 24 Basic templates provided by NetSuite, you can only modify the fields on the [Default Chart Type](#procedure_N2602698) subtab. To modify the HTML used in each template attached to those layouts, you must enable the Advanced Site Customization feature. For more information, see [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603624.html).

## Editing Web Site Layouts {#bridgehead_N2602606}

You can edit Web site layouts that you create and the basic templates provided by NetSuite. Go to _Commerce > Site Builder > Appearance > Layouts_, and then click Customize next to the layout you want to modify. Note that without the Advanced Site Customization feature, your customization options are limited.

## Creating Web Site Layouts {#bridgehead_N2602618}

After you create a layout, you must select the layout on a tab to display it on your website. For more information, see [Customizing Presentation Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595616.html#bridgehead_N2595880). To see a new layout on your site, go to _Commerce > Websites > Preview Website_.

#### To create an item/category layout: {#procedure_N2602648}

1.  Go to _Commerce > Site Builder > Appearance > Layouts > New_.
    
2.  In the **Name** field, enter a name for the layout.
    
3.  The sections below describe the fields on each subtab.
    

#### Default Chart Type {#procedure_N2602698}

1.  In the **Border Style** field, select one of the following:
    
    -   **No Window** - this places your Welcome message in a colored box at the top of the page
        
    -   **Window With Title Bar** - this places your Welcome message and featured items in a colored box below your Welcome greeting
        
    -   **Window Without Title Bar** - this places your Welcome message and featured items in an outlined, colored box
        
        To customize colors for your layouts, go to _Commerce > Site Builder > Appearance > Color Themes_.
        
2.  In the **Column Width** field, choose **Fit to Browser Window** or select a column width. The column width options in the list are in pixels.
    
3.  In the **Number of Columns Shown** field, choose Single Column List or the number of columns you want to appear on a page.
    
4.  In the **Number of Rows Shown** field, choose the number of rows you want to appear on a page. The maximum limit is 50 rows on a page. Visitors to your site can click page links to see more items and categories.
    
5.  In the **Row Height** field, specify the height of the table cells in pixels. Enter a number in this field. You can leave this field blank to use the default value set by NetSuite.
    
6.  In the **Row Padding** field, define the space between cell content and its borders. Enter a positive number in this field to create more space, or a negative number to create less space. You can leave this field blank to use the default value set by NetSuite.
    
7.  Check the **Paginate** box to show your site visitors which page they are on if your list is on multiple pages. In the **Display** field, choose to show page numbers at the top of the list, bottom of the list, or both.
    
8.  Check the **Sort Links** box to allow your customers to sort lists alphabetically or by price. In the Display field, choose to show these links at the top of the list, bottom of the list, or both.
    
9.  In the **Items Are Laid Out** field, choose to lay out items horizontally or vertically.
    
10.  If you want to use a checkerboard effect with this custom layout, check the **Use Checkerboard Effect** box. This causes every other item in a list to have a background.
     
11.  In the **Sort By** field, choose one of the following to sort item or category lists:
     
     -   **Sequence** - Lists items in the order they appear on the tab or category record.
         
     -   **Name** - Lists items alphabetically by name.
         
     -   **Price** - Lists items by price, low to high.
         
12.  Check the **Descending** box to list prices from high to low, names from Z to A or sequenced items in reverse
     
13.  Check the **Use Templates** box to an item/category templates to format lists for this layout.
     
     Note:
     
     If you check the **Use Templates** box, the Heading and Items subtabs are removed. The settings on these subtabs should be addressed in your item/category templates.
     
14.  In the **List Template** field, select the template for the list of categories or items. This template must include the <NLITEMLIST> tag.
     
     To create a new list template from this page, click the New button next to the list Template field. For more information, see [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html).
     
15.  In the **List Cell Template** field, select the template for how categories or items in the list should display.
     
16.  If you checked the **Use Checkerboard Effect** box, in the **Alternate List Cell Template** field, select an item/category template to use for every other item or category in a list. The type of tags used in this template must match those used in the templates selected in the **List Template** field and **List Cell Template** field. Click the New button to create a new template.
     
     Note:
     
     Item templates and category templates cannot be combined on layouts.
     

#### Heading {#procedure_N2602908}

1.  In the **Heading Placement** field, choose where the category name or the brief description of a category should display.
    
2.  If you want the heading to have a backdrop, check the **Heading Backdrop** box. Checking this box applies a custom color to appear behind the category name.
    
3.  In the **Image** field, choose how the category image should display in the heading:
    
    -   **No Image** - this shows no image on the page you apply this custom layout to
        
    -   **Show Image Thumbnail** - this shows only the image thumbnail
        
    -   **Show Full-Size Image** - this shows only the full-size image
        
4.  In the **Image Placement** field, choose where the category image is placed in relation to the category description.
    
5.  Check the **Gap Between Text and Image** box to have a larger space between the image and description.
    
6.  In the **Image Alignment** field, choose how the category image should be aligned.
    
7.  In the **Title Text Alignment** field, choose how the name of the category is aligned.
    
8.  In the **Description Text Alignment** field, choose how the description of the category is aligned.
    
9.  In the **Vertical Alignment** field, choose how text is vertically aligned in the heading.
    

#### Items {#procedure_N2603020}

1.  In the **List Style** field, select one of the following:
    
    -   **Graphical Item List** - item lists span multiple rows
        
    -   **Dense Item List** - condenses your item lists into a single row
        
2.  In the **Image** field, choose how images should display in a list.
    
3.  In the **Image Placement** field, choose how category or item images are displayed in relation to the description.
    
4.  Check the **Gap Between Text and Image** box to have a larger space between the image and description.
    
5.  In the **Image Alignment** field, choose how category or item images should be aligned.
    
6.  In the **Title Text Alignment** field, choose how the names on this list should be aligned.
    
7.  In the **Description Text Alignment** field, choose how the descriptions in the list should be aligned.
    
8.  In the **Vertical Alignment** field, choose how the text for each item or category should be vertically aligned.
    
9.  Check the **Show Item Prices** box to show prices next to items in lists.
    
10.  To display the Add To Cart link next to items, check the **Show Add To Cart Button** box. If you do not check this box, the Add to Cart button does not appear next to items. Shoppers must drill down to item details to place items in the shopping cart
     
11.  To show separators between items, check the **Show Separators Between Items** box. Separators are small dots that can help differentiate your categories and items.
     

After you create your custom layouts, you can do the following:

-   Apply your layouts to specific tabs and categories in your website using the [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html) (_Commerce > Site Builder > Content Management > Content Manager_).
    
-   Set default layouts at _Commerce > Websites > Website List_.
    

### Related Topics

-   [Changing Website Color Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603251.html)
-   [Adding a 'Tell A Friend' Link](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603455.html)
-   [Basic Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602412.html)
-   [Web Site Appearance Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2564504.html)
-   [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
