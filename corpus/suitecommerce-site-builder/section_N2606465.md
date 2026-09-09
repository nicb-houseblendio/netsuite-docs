---
id: "section_N2606465"
type: "section"
title: "Creating Item/Category Templates"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Item and Category Templates > Creating Item/Category Templates"
parent: "section_N2606158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html"
anchors: ["procedure_N2606596"]
sha256: "e7ce8f5ee4131121fbb01ed309a7fd5c3f4809d6f73de09d72c3986e733091f2"
---

You can use item/category templates to customize the look and feel of several types of Web site pages:

-   category lists
    
-   item lists
    
-   lists of related items
    
-   lists of upsell items
    
-   item detail pages
    
-   information item detail pages
    

After you create an item/category template, you can attach it to a category or item list page. For more information, see [Applying Templates to Lists of Categories and Lists of Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606825.html). You can also create an item/category template that shows multiple views of an item on your site. See also, [Placing Multiple Images in an Item/Category Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607454.html).

Note:

To add graphics and apply style sheets to HTML site theme templates that you create, you must upload image and CSS files to the Web Site Hosting Files folder.

#### To create an item/category template: {#procedure_N2606596}

1.  Go to _Commerce > Site Builder > Appearance > Item/Category Templates > New_.
    
2.  In the **Name** field, enter a name for this template.
    
3.  (Optional) In the **Description** field, enter a description for your template.
    
4.  In the **Template** HTML field, enter HTML within <td> start and end tags to create your item/category template. The HTML you enter here specifies how content is displayed. Note the following:
    
    -   Use NetSuite [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html) to display information from fields on item records in the site.
        
    -   Read [Sample HTML for Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607165.html) to help you create your first template.
        
5.  (Optional) In the **Addition to <head>** field, you can enter any additional HTML you want to appear in the header of the item page.
    
6.  Click **Save**.
    

Note that when you create a template for category list pages, you must include the <NLITEMLIST> tag in the template HTML so that categories display properly on the page. For more information about Web Site Tags, see [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html).

For a list of record types and attributes, see [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html). For a complete list of the website tags available for use in item/category templates and hosted HTML pages, see [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html).

### Related Topics

-   [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html)
-   [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603624.html)
-   [Site Builder Items, Forms, & Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2582621.html)
-   [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
