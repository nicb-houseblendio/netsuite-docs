---
id: "section_N2607454"
type: "section"
title: "Placing Multiple Images in an Item/Category Template"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Item and Category Templates > Placing Multiple Images in an Item/Category Template"
parent: "section_N2606158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607454.html"
anchors: ["procedure_N2607561", "procedure_N2607823"]
sha256: "290b3016368a2479c4b2a03ce022377bd7cabfc3f5ca4a7d0efe64d7437e4e07"
---

Web site tags and item/category templates allow you to show the items you sell on your web store from various angles or in different colors or sizes.

You can publish multiple images for items in one of the following ways:

-   Use multiple <img src> tags to publish images directly from the File Cabinet.
    
    With this approach, it is best to create an item drilldown template specific to each item, as the images may only be appropriate for a particular item. For details, see [Publishing multiple images for an item using <img src> tags](#procedure_N2607561).
    
-   Use custom item fields to store images on each item record, and then use attribute tags in a site template to publish multiple images of the item on your site.
    
    With this approach you do not need to maintain a set of templates when you want to change images for a particular item. The attribute tag you use in the item drilldown template refers to the custom field. This is so you can attach specific images to item records, but build different templates for your website that refer to the same custom field. For more information, see [Publishing multiple images for items using custom item fields](#procedure_N2607823).
    

You must have the Advanced Site Customization feature selected on the Web Presence tab of the Enable Features page (_Setup > Company > Enable Features_) to create and edit item templates. An administrator must complete this task.

#### Publishing multiple images for an item using <img src> tags {#procedure_N2607561}

1.  Go to _Commerce > Site Builder > Content > Images_.
    
2.  Click **Images** to open the Images folder.
    
    Find the image you want to use, or in the footer of the page, click Add File. See [Uploading Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592452.html#bridgehead_N2592477) for detailed information on uploading image files to NetSuite.
    
3.  Go to _Commerce > Site Builder > Appearance > Item/Category Templates_.
    
4.  Create your template file as instructed in [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html).
    
5.  To add images, in your template HTML code, use <img src> tags that refer to the image files in the NetSuite file cabinet. Use the NetSuite-generated URL for a file in the images folder. To find the URL for the image file, click Edit next to the file you want to use, and then choose a URL on the file record. Note the following example of the <img src> tag.
    
                    `<img src='/core/media/media.nl?id=2033&c=563214&h=f6a40c57d48a0e61dde7'>` 
                  
    
    -   To align the image, add the align attribute in the <img src> tag.
        
    
    -   To add a border to the image, add the border specifications to the tag.
        
6.  Click **Save**.
    
7.  After you have saved your item/category template, go to _Lists > Accounting > Items_.
    
    1.  Click **Edit** next to an item record.
        
    2.  Click the **Web Store** subtab.
        
    3.  Select the item drilldown template you created, in the **Item Drilldown Template** field.
        
8.  Click **Save** on the item record.
    

#### Publishing multiple images for items using custom item fields {#procedure_N2607823}

1.  Go to _Customization > Lists, Records, & Fields > Item Fields > New_.
    
2.  In the **Label** field, enter a name for an alternate image field on item records, such as **Alternate View Image**.
    
3.  In the **ID** field, enter a one word or number code that you will use in the tag for this field. For example, enter **altimage.** Later, you will use this ID to create an Attribute tag:
    
                    `<%=getCurrentAttribute('item','altimage')` 
                  
    
4.  In the **Type** field, select Image.
    
5.  Check the **Store Value** box.
    
6.  Check the **Show in List** box to see data for this field in the Items list.
    
7.  On the **Applies To** subtab, check the box next to each type of item you want to select additional images for.
    
8.  On the **Display** subtab, set preferences for where you want this field to appear on the item record in NetSuite.
    
9.  Click **Save**.
    
10.  On each item record, locate your new custom field, and select or upload an alternate image for the item.
     
11.  After saving each item record with an alternate image, create an Item Drilldown Template. To display the alternate image, use the tag format below enclosed in the <img src> tag in your template:
     
                     `<img src='<%=getCurrentAttribute('item','altimage')%>'>` 
                   
     
     For more information, see [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html). See also, [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html).
     
12.  After you have saved your item/category template, you can do one of the following:
     
     -   Apply it to all items for an individual theme at _Commerce > Site Builder > Appearance > Themes_.
         
     -   Apply it to all items for a site with any theme at _Commerce > Websites > Website List_.
         
     -   Apply it to individual items on item records at _Lists > Accounting > Items_.
         

### Related Topics

-   [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html)
-   [Applying Templates to Lists of Categories and Lists of Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606825.html)
-   [Sample HTML for Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607165.html)
-   [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html)
-   [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
