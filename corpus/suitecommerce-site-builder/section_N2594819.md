---
id: "section_N2594819"
type: "section"
title: "Resizing Images"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Items, Forms, & Images > Images > Resizing Images"
parent: "section_N2592452"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2594819.html"
anchors: ["procedure_N2594850", "bridgehead_N2595068"]
sha256: "89b13450065cf3deb6796c04f85b3161ab2f9539f5e623837bf3476f1522d58e"
---

When you set up image resizing, you can upload one image per item or record and set size limits for thumbnail and drilldown images. This prevents you from uploading the same image in multiple sizes.

The resize process maintains the aspect ratio of the image and the image is scaled, so that the height and width are never greater than the dimensions you specify on the Image Resizing Setup page. For example, if you start with an image that is 800 x 500, and resize it to thumbnail size, which is 80 x 80, the image retains its rectangular shape.

Warning:

Images with an original length or width greater than 5 megapixels cannot be resized and will not display in your site. Please resize larger images before uploading them to the File Cabinet.

#### To set default sizes for your images: {#procedure_N2594850}

1.  Go to _Commerce > Site Builder > Content > Image Resizing_.
    
2.  Check the **Enabled** box if you want to use automatic image resizing for the following circumstances:
    
    -   **Dense List Drilldown Image** - Applies to images displayed when you drill down on an item displayed in a dense list.
        
        Dense Lists display basic information about items in a table format. The fields displayed in a Dense List layout are description, price, options, quantity, and the add to cart button. You choose dense or graphical lists when you create or edit Layouts at _Commerce > Site Builder > Appearance > Layouts_.
        
    -   **Dense List Image** - Applies to images displayed with items in dense lists.
        
    -   **Employee Image** - Applies to employee images when you publish an employee directory with images.
        
    -   **Web Site Drilldown Image** - Applies to images displayed when a thumbnail image is clicked or when customers view the item detail page in the website.
        
    -   **Web Site Category Thumbnail Image** - Applies to category images for categories or subcategories in a list.
        
    -   **Web Site Featured Item Thumbnail Image** - Applies to featured item images on the Home page tab.
        
    -   **Web Site Related Item Thumbnail Image** - Applies to item images in lists of related items.
        
    -   **Web Site Thumbnail Image** - Applies to images displayed in graphical lists in your website.
        
3.  In the Maximum Height Column, enter the maximum height for each type of image in pixels.
    
4.  In the Maximum Width Column, you can accept the size given to keep the image in scale or enter the maximum width in pixels that each image can be.
    
    You can size your images from 10-999 pixels.
    
5.  Click Save.
    

You can upload images to your File Cabinet and select them on item, information item and category records. The images will display in your web store according to your settings on the Image Resizing Setup page.

## Resizing Images and Advanced Site Customization {#bridgehead_N2595068}

If you use the Advanced Site Customization Feature, you can use the attributes listed below in the HTML of your custom themes and templates to display resized images.

| Item Attributes | Notes |
| --- | --- |
| storedisplaythumbnailhtml | Returns the item/category thumbnail image. The default image size is 80 by 80 pixels. |
| storedisplayimagehtml | Returns the item/category image. The default image size is 240 by 240 pixels. |
| categorythumbnailhtml | Returns the category image. The default image size is 80 by 80 pixels |
| relateditemthumbnailhtml | Returns item display image. The default image size is 80 by 80 pixels. |
| featureditemthumbnailhtml | Returns item display image. The default image size is 120 by 120 pixels. |

### Related Topics

-   [Using Images in your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592719.html)
-   [Deleting Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595264.html)
-   [Make Images Available Without Login](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162137415332.html#subsect_162137429522)
-   [Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592452.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
