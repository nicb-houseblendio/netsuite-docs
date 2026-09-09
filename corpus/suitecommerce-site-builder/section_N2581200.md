---
id: "section_N2581200"
type: "section"
title: "Publishing Content with Multiple Websites"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Creating Multiple Websites > Publishing Content with Multiple Websites"
parent: "section_N2580798"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581200.html"
anchors: ["procedure_N2581254", "bridgehead_N2581436"]
sha256: "2a9bae9458e7f53c777bd2d61a55fe4693b3b41aead26f28b4fdaec8d6c17ec8"
---

When you have multiple websites, you can choose which website you want to publish a tab, a category or an item to. When visitors view a page of a site, they can only access the tabs assigned to that site.

Categories are only assigned to one tab and therefore only to one site. However, you can publish items to more than one site in the categories and tabs you choose. You can also reuse tab and category names across sites if needed. Because you must select a site before selecting a category, you are prevented from selecting the wrong category or tab when you reuse a name.

Before publishing content to a site, you must set up a site record at _Commerce > Websites > Website List_. For more information, see [Creating Multiple Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2580798.html).

#### To publish content to a NetSuite site: {#procedure_N2581254}

1.  To create tabs for your site, go to _Commerce > Site Builder > Content Management > Tabs > New_.
    
2.  If you are creating a hosted tab for a combination site, click **New Hosted** Tab.
    
    If you are creating a tab with items or information from your NetSuite account, click **New Presentation** Tab.
    
3.  On the tab record, in the **Site** field, select the site where the tab should show, and fill in other information for the tab. For more information about creating tabs, see [Creating Website Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595492.html). A tab can only show in one site. If you need a tab with the same name in two sites, you can create a second tab with the same name and select the other site name.
    
4.  Repeat these steps for each tab you need in each site.
    
    You can now add categories to organize the tab.
    
5.  Go to _Commerce > Site Builder > Content Management > Categories > New_.
    
6.  On the category record, in the **Site** field, select the site where this category should show.
    
    Selecting a site filters the list of categories you can select in the Subcategory of field. It does not publish a category or saved search only.
    
7.  In the **Subcategory of** field, select the tab or category where this category should be placed. Only tabs and categories set to show in the site you chose can be selected.
    
    Important:
    
    If you are editing the location of a category or a published saved search, remember to change the category in this field. Changing the site in the **Site** field only does not change the location.
    
8.  At the bottom of the **Basic** subtab, select and add each item that should show in this category on this site. You can add information items for posting text, you can select items to sell, or select files from the file cabinet to share. To select more than one item, click **Add Multiple**. Items are not shown online until they are added to a published category.
    
    Categories are published when they meet the following criteria:
    
    -   The **Display in Web Site** box is checked or an audience is selected on the **Audience** subtab.
        
    -   The parent category is a tab that is displayed in the website or includes the same audience.
        
9.  Fill in other information for this category. For more information, see [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html).
    

Your tabs, categories, and items are now added your site. When you create or edit items in the future, you can add them or remove them from a site on the Store subtab of the item record.

## Previewing Websites {#bridgehead_N2581436}

If you have a single website, you can preview it using the Preview Web Sites page at _Commerce > Websites > Preview Website_.

If you have multiple websites, you can use the Preview link next to each website in the Web Sites list at _Commerce > Websites > Website List_. You can also use the Preview Web Sites page to preview your first website.

### Related Topics

-   [Multiple Website Online Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581595.html)
-   [Creating Hosting Root Folders for Multiple Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581907.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
