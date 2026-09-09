---
id: "section_N2615537"
type: "section"
title: "Creating Attribute Tags"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags"
parent: "chapter_N2615371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html"
anchors: ["bridgehead_N2615664"]
sha256: "6f5b60a92cd20d7bd587685462444d5e48fcc280e736b064bc49253349bebd58"
---

Use Attribute tags to display information from item, information item, category, and customer records in site themes, item/category templates, and hosted HTML pages.

For example, you might use Attribute tags to display an image in the store detailed description field of your NetSuite generated site, or to capture information retrieved from browser requests, or to display an item from your NetSuite account on a hosted HTML page.

Attribute tags are supported in HTML files hosted in your NetSuite file cabinet, item/category templates, site themes, and email messages generated from orders. To customize email messages go to _Commerce > Site Builder > Content > Customize Text_.

Important:

Web Site tags are not supported in SuiteCommerce Advanced websites.

Important:

Attribute tags are not supported in System Email Templates.

Use the table below, in [Using recordType in Attribute Tags](#bridgehead_N2615664), to find reference information for creating Attribute tags.

-   For sample code, and links to other topics on creating Themes and Item/Category Templates, read [Using Attribute Tags in Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616422.html).
    
-   For sample code you can use to display items from your NetSuite account on hosted HTML pages, read [Using Web Site Tags in Hosted Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616592.html).
    
-   To learn how to create Attribute tags for custom records and custom fields, read [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html).
    
-   To learn how to create Attribute tags for standard NetSuite records, read [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html).
    

Note that you can use Attribute tags in most description fields on standard NetSuite records, however, to use website themes, customize item/category templates, and use Attribute tags in hosted HTML pages, you must enable the Advanced Site Customization feature.

## Using recordType in Attribute Tags {#bridgehead_N2615664}

To create an Attribute tag, use the tag component for recordType and an attribute for the information you want to display from the record. For example:

          `<%=getCurrentAttribute('item','storedisplayname')%>` 
        

To learn more about the syntax for creating attribute tags read the following topics:

-   [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html)
    
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)
    

The table below provides a guide to finding more information about which fields on NetSuite records are available for use in Attribute tags and how to construct them.

| Record Type | Tag Component for recordType | Notes |
| --- | --- | --- |
| Item | item | For more information, see [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html). |
| Information Items | infoitem | Only Text and Image or Formatted Text records are available for use in Attribute tags. For more information see, [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html). |
| Category | sitecategory | For more information, see [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html) |
| Color Theme | colortheme | Tags with the **colortheme** component return colors for the current color theme in #RRGGBB form. For more information, see [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html). |
| Customer | customer | For more information, see [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html). |
| Custom record | record ID | For more information see [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html). |
| Order Email Messages | salesorder | For more information, read the topic, [Attribute Tags for Use in Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4428732431.html). |
|  | site | Used for site-wide properties, such as capturing referrer information from visitors on your site. For more information, see [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html) |
|  | request | Used for returning information about the session to include in any custom JavaScript. For more information, see [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html). |
|  | checkout | Used in the Order Script Tracking HTML field at _Commerce > Websites > Website List_ on the Analytics subtab. [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html) capture data related to the order amount, shipping, and tax. |
| Thank You page | confirmation | Used to capture data from orders placed on your website, and to send this data to third-party reporting tools. For more information, see [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html). |

### Related Topics

-   [Declare Attribute Tags for Tags Within Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628302.html)
-   [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html)
-   [Using the Server-Side Include Tag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2629027.html)
-   [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html)
-   [Tags for Information Unavailable on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2634674.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
