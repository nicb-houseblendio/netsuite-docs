---
id: "section_N2645022"
type: "section"
title: "Google Base"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Setting Up Website Product Feeds > Google Base"
parent: "section_N2639492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html"
anchors: []
sha256: "346482d55e443c215ff200e63549bbec589becf898d56206570dbffdf9777cbe"
---

Important:

Google Base has been retired. However, you can use the information below to create a saved item search that you can export and use as a product feed. Visit the help page on the Google Merchant Center website for more information about the data feed submission process and specific requirements.

Use the saved search provided by NetSuite to create a product feed you can upload to Google Shopping. You might have to create custom fields, and then customize the saved search to comply with the latest requirements from Google Shopping. For more information about editing the saved search, see [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html).

Google Shopping requires that you enter data in the **id** and **description** columns of the product feed.

-   In NetSuite, the **id** column is blank by default. Enter the item's Internal ID after your product feed has been exported to a spreadsheet and before you turn it into a tab-delimited text file. To display the Internal ID on the Store tab of the item record, go to Home > Set preferences, and check the Show Internal IDs box.
    
-   In NetSuite, the **description** column shows information from the Detailed Description field on the Store subtab of item records.
    

The table below shows the columns in your NetSuite product feed, and some of the columns that may be required or recommended by Google Shopping. The column names that appear below with an asterisk are required. The other columns are recommended.

| NetSuite | Google Base | Note |
| --- | --- | --- |
| id | id\* | Enter the item's Internal ID. Go to Home > Set preferences, and check the Show Internal IDs box to display the **Internal ID** on the Store tab of the item record. By default, the value for this field comes from the **Item Name/Number** field on the Item record. For more information, see [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html) |
| title | title\* | The value for this field comes from the **Item Name/Number** field on the Item record. |
| description | description\* | The product feed results display the detailed description from the Store subtab on the item record. Note: You must remove any control characters and embedded HTML. |
| product\_type | product\_type | The product feed displays the tab > category where you publish the item on your website. |
| link | link\* | The URL displayed in product feed results is the link to the item in your web store. |
| image\_link | image\_link\* | The URL displayed in product feed results is the link to the image associated with the item in your web store. |
| condition | condition\* | Use this field to designate the state of the product. |
| price | price\* | Product feed results in NetSuite display the online price level as defined on the Web Site Setup form. If you use NetSuite OneWorld, and you choose a subsidiary in the list at the bottom of the product feeds page, the price displayed is the default currency for the subsidiary. |
| brand | brand | Add the brand name of the product. This attribute is required for some types of products. |

### Related Topics

-   [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html)
-   [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html)
-   [Yahoo! Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html)
-   [NexTag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html)
-   [Shopzilla](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html)
-   [Shopping.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
