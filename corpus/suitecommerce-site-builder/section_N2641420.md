---
id: "section_N2641420"
type: "section"
title: "Yahoo! Shopping"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Setting Up Website Product Feeds > Yahoo! Shopping"
parent: "section_N2639492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html"
anchors: ["procedure_N2641454"]
sha256: "31f3187b2fcc02b28abeafd3958e7d74487e1044c87e42d2533a2b9bbc5acc03"
---

To upload a product feed file to Yahoo! Shopping, create an account with the Product Submit service and ensure the information in your NetSuite product feed complies with the requirements. For more information, read the topics on [Product Submit](http://help.yahoo.com/l/us/yahoo/ysm/ps/index.xml) in the Yahoo! Help Center.

After you have exported your product feed data from NetSuite to a spreadsheet, for successful upload to Yahoo! Shopping, you must save the file as a Tab-Delimited Text file named 'data.txt.' For more information, see [Setting Up Website Product Feeds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639492.html).

#### To upload your product feed to Yahoo! Shopping Product Submit: {#procedure_N2641454}

1.  Log in to your Yahoo! Shopping Product Submit account.
    
2.  Select the option to upload your file using a browser.
    
3.  Click **Browse** to find the file on your computer and upload it to Yahoo! Shopping.
    

It may take several days to process your product feed and display your listings online. Visit [help.yahoo.com](http://help.yahoo.com/l/us/yahoo/ysm/ps/submit/submit-14.xml) for more information.

The table below shows the fields displayed in your NetSuite product feed, and the fields that are required or recommended by Yahoo! Shopping Product Submit. The fields that appear with an asterisk are required. Other fields are recommended.

| NetSuite | Yahoo! Shopping | Notes |
| --- | --- | --- |
| Display Name/Code | code\* | Enter the item's Internal ID. Go to Home > Set preferences, and check the Show Internal IDs box to display the **Internal ID** on the Store tab of the item record. |
| Item Name/ Number | name\* | The value for this field comes from the **Item Name/Number** field on the Item record. |
| Description | description\* | The product feed results display the detailed description from the Store subtab on the item record. Note: You must remove any control characters and embedded HTML. |
| Price | price\* | Product feed results in NetSuite display the online price level as defined on the Web Site Setup form. If you use NetSuite OneWorld, and you filter the list by subsidiary, the price displayed is the default currency for the subsidiary you selected. For successful upload to Yahoo Shopping, the price must be in US dollars, with a decimal point and no currency symbol. |
| Product URL | product-url\* | The URL displayed in product feed results is the link to the item in your web store. |
| Merchant Site Category | merchant-site-category\* | The product feed results display the category on your website for each product. |
| Custom Field | medium\* | Create a custom field in NetSuite on your item records for medium. For more information see, [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html). Then, edit the product feed search for Yahoo!Shopping to include 'medium' as a column. For more information, see [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html). This field is required for Music and Video products only. Leave this field blank for all other product types. |
| Image URL | image-url | The URL displayed in product feed results is the link to the image associated with the item in your web store. |
| MPN | manufacturer-part-no | The manufacturer's unique part number for the product. Do not include your own SKU. In NetSuite, you can enter data for this field in the **MPN** field on the Basic subtab of the item record. |
| In-Stock | in-stock | NetSuite displays a value of yes or no based on the On Hand Quantity of the item. |
| Shipping Price | shipping-price | The cost of shipping the item anywhere in the United States in US dollars, with a decimal point and no currency symbol. Use 0.00 for free shipping. You may need to add a value in this field after exporting the NetSuite product feed results. |
| Shipping Weight | shipping-weight | The weight of the item in pounds, up to one decimal place. The NetSuite product feed results display the value in the **Item Weight** field on the Basic tab of the item record. |

### Related Topics

-   [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html)
-   [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html)
-   [NexTag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html)
-   [Shopzilla](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html)
-   [Shopping.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html)
-   [Google Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
