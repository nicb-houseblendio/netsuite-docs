---
id: "section_N2595616"
type: "section"
title: "Presentation Tabs"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Tabs & Categories > Creating Website Tabs > Presentation Tabs"
parent: "section_N2595492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595616.html"
anchors: ["procedure_N2595660", "bridgehead_N2595880", "bridgehead_N2596056", "procedure_N2596069"]
sha256: "4997437e4958a41b68d79ea0f26319c7bc974a64008782f22dc6ef2303db5b3b"
---

You can create presentation tabs in NetSuite for display on your website or intranet site. Presentation tabs are pages on your website. If you use the Advanced Site Customization feature, select a custom template for displaying content on your site. For more information, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).

After you create presentation tabs for your website, use the Setup Web Site page to change the order in which they display. For more information, see [Organizing Presentation Tabs](#bridgehead_N2596056).

The following steps only describe how to enter data in the required fields to display a presentation tab on your website. To learn more about the different ways in which you can customize presentation tabs and apply SEO tools, read [Customizing Presentation Tabs](#bridgehead_N2595880).

#### To create a presentation tab for display on your website: {#procedure_N2595660}

1.  Go to _Commerce > Site Builder > Content Management > Tabs_.
    
2.  Click **New Presentation Tab**.
    
    You can also create a tab while using the Web Site Content Manager at _Commerce > Site Builder > Content Management > Content Manager_. For more information about the Content Manager, see [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html).
    
3.  In the **Label** field, enter a name for this tab. Your customers click what you enter here to view the items on that tab.
    
    You can enter up to 30 characters of letters and numbers. You cannot enter HTML in this field.
    
4.  Choose the website where you would like the tab to display in the **Site** field.
    
5.  Check the **Display in Web Site** box.
    
6.  Click **Save**. Your tab now automatically appears in your website.
    

You can add information using the subtabs on the presentation tab record.

-   The **Audience** subtab lets you publish the tab to everyone that visits your web store, or to a select group of customers. If you publish a tab to a dynamic group, for performance reasons, the tab's audience is a snapshot of the dynamic group members. The snapshot is updated twice a day.
    
    For information about publishing a presentation tab in your NetSuite account, and not in your web store, see [Publishing Information to an Internal Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597878.html).
    
-   If you use Advanced Site Customization, the **Tag Substitution** subtab will appear after you save a new tab. See [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html) for information on using custom tags to substitute values on a presentation tab.
    
-   After saving your new tab, the **Content** subtab appears. Here you can add items for display on the tab, or see the categories attached to the tab. For more information about categories, see [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html).
    
-   If you use the Multi-Language feature, the **Translation** subtab will appear after saving your new tab. Here, you can enter translated text for specific fields on your tab. For more information see, [Setting Up a Site for Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2463004.html).
    

## Customizing Presentation Tabs {#bridgehead_N2595880}

You can use the fields listed below on the tab record to customize the look and feel of your website. You don't need to fill in these fields when you first create a presentation tab record.

If you use the Advanced Site customization feature, create a custom HTML template and select that template in any of the List Layout fields on the tab record. For more information, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).

-   **Category List Layout** - Select a layout for the list of categories displayed on this tab. For more information, see [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html).
    
-   **Item List Layout** - Select a layout for the item lists you place on this tab.
    
-   **Related Items List Layout** - Select a layout for your related items list. Use related items to cross-sell items that complement each other. For more information, see [Related Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2586873.html).
    
-   **Welcome Page Portlet Alignment** - Choose where the link to this tab will appear on the Home tab of your web store. You can set the alignment to the left column, the right column, or choose not to display a link to this tab on the Home tab.
    
-   **Greeting** - Enter a greeting for this tab. This greeting appears above your tab message. You can enter up to 4,000 characters of letters, numbers, and HTML.
    
-   **Message** - Enter a message for this tab. This message appears below the greeting on your tab. You can enter up to 4,000 characters of letters, numbers, and HTML. On your Home tab, the message appears below content in the Flash® or image field.
    
-   **Page Title** - Enter a page title for this tab which is added to the HEAD element of the HTML source code for this page. For more information, see [Adding Page Titles in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636435.html).
    
-   **URL Component** - This field is displayed only after you turn on the Descriptive URLs feature. Enter a name which will appear in the URL for this page. If you do not enter a URL component, the text in the Label field is used in the URL.For more information see [Descriptive URLs in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2637101.html).
    
    Note:
    
    The name you use as a URL component cannot be a reserved character string in the NetSuite application. If you enter a reserved character string, then you will be notified with a popup alert message. You can enter a different URL component to continue.
    
-   **Meta Tag HTML** - Enter a META tag which is added to the HEAD element of the HTML source code for this page. For more information, see [Adding META Tags in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636604.html).
    

## Organizing Presentation Tabs {#bridgehead_N2596056}

After you create presentation tabs for your web store, you can set the order in which they display on your website.

#### To organize presentation tabs: {#procedure_N2596069}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to the site you want to organize.
    
3.  Click the **Appearance** subtab.
    
4.  On the **Tabs** subtab, select a row, and drag it to the position where you want it to appear.
    

When shoppers view your website, the tabs appear in the order you set here.

### Related Topics

-   [Hosted Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596130.html)
-   [Creating Website Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595492.html)
-   [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html)
-   [Publishing Information to an Internal Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597878.html)
-   [Site Builder Tabs & Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2595349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
