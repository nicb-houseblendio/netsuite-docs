---
id: "section_N2606825"
type: "section"
title: "Applying Templates to Lists of Categories and Lists of Items"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Item and Category Templates > Applying Templates to Lists of Categories and Lists of Items"
parent: "section_N2606158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606825.html"
anchors: ["procedure_N2606857", "bridgehead_N2607003", "procedure_N2607023"]
sha256: "1eba55ce96f9344b040fb33c97af186002794070f3bfaf44753b6015a9e130d2"
---

After you have created a template for a category or item list, you must apply the template to a layout. A layout record requires a template for the list, and a template for each list cell. The list cell template determines how names, descriptions and images are displayed in the list.

#### To create a layout for item lists or category lists using an item/category template: {#procedure_N2606857}

1.  Go to _Commerce > Site Builder > Appearance > Layouts_. Click **New**.
    
2.  In the **Name** field, enter a name for the layout. Use a name that identifies whether this template is for lists of categories or for lists of items, for example Spring Sale Item List Template.
    
3.  Check the **Use Templates** box.
    
4.  Select the HTML templates you want to attach to this layout.
    
    1.  Select a template in the **List Template** field.
        
    2.  Select a template in the **List Cell Template** field.
        
5.  Click **Save**.
    

When your layout is complete, you can apply it to your website by selecting it on tab and category records, in your site theme, or on the Appearances subtab of the Setup Web Site page.

## Applying Templates to Item Detail Pages or Information Items {#bridgehead_N2607003}

When you use an item/category template on your item detail pages, it is not necessary to create a layout. Instead, you can select the template for the item detail page on the Set Up Web Site page. As a result, the template is applied globally to all item detail pages on your website.

Note:

You can override the global item drilldown template setting on the Set Up Web Site page by selecting a different template on an individual item record.

#### To apply item/category templates to item detail pages or information items: {#procedure_N2607023}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to a website.
    
3.  Click the Appearance subtab.
    
4.  In the **Default Item Drilldown Template** field, select the default template for all items or information items in your site.
    
    If you want to apply a template for an information item, choose your template in the Default Information Item Drilldown Template field.
    
5.  Click **Save**.
    

### Related Topics

-   [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html)
-   [Sample HTML for Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607165.html)
-   [Placing Multiple Images in an Item/Category Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607454.html)
-   [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html)
-   [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
