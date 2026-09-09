---
id: "section_N2644262"
type: "section"
title: "Shopping.com"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Setting Up Website Product Feeds > Shopping.com"
parent: "section_N2639492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html"
anchors: ["procedure_N2644295"]
sha256: "6324f87f7d8f9fa25ae93a1e77ddce919bde5654f6a088c9423809d0f4e5b3b1"
---

You must create an account with Shopping.com to upload your product feed file. Visit [merchant.shopping.com](https://merchant.shopping.com/mac/app) to create an account and view the product feed file specifications.

You might need to change column names in the NetSuite product feed results to comply with requirements from Shopping.com. For more information, read [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html).

#### To upload your product feed file to Shopzilla: {#procedure_N2644295}

1.  Log in to your Shopping.com merchant account.
    
2.  Select the option to upload from your desktop.
    
3.  Click **CPC program**.
    
4.  Click **Product** Info.
    
5.  Click **Browse** to find the product feed file on your computer.
    
6.  Click **Continue**.
    
7.  Review the conversion of your feed file columns to the columns in the Shopping.com database.
    

The table below shows the columns displayed in your NetSuite product feed results and the columns that are required by Shopping.com. The column names that appear below with an asterisk are required. Other columns are recommended.

| NetSuite | Shopping.com | Notes |
| --- | --- | --- |
| MPN | mpn\* | The manufacturer's unique part number for the product. Do not include your own SKU. You can enter data for this field in the **MPN** field on the Basic subtab of the item record. |
| Manufacturer Name | manufacturer\* | Brand, manufacturer, or publisher for the product. |
| Product Name | product name\* | The value for this field comes from the **Item Name/Number** field on the Item record. |
| Product Description | product description\* | The value for this field comes from the **Detailed Description** from the Store subtab on the item record. Note: You must remove any control characters and embedded HTML. |
| Online Client Price | price\* | Product feed results in NetSuite display the online price level as defined on the Web Site Setup form. If you use NetSuite OneWorld, and you choose a subsidiary in the list at the bottom of the product feeds page, the price displayed is the default currency for the subsidiary. |
| Stock Availability | stock\* | NetSuite displays a value of yes or no based on the On Hand Quantity of the item. |
| Stock Description | stock description\* | Use this field to designate the state of the product. (21 characters maximum.) For example: 'Back ordered 2-3 Weeks,' or 'Ships in 2-3 Days.' |
| Product URL | product url\* | The URL displayed in product feed results is the link to the item in your web store. |
| Image URL | image url\* | The URL displayed in product feed results is the link to the image associated with the item in your web store. |
| Shopping.com Categorization | category\* | Enter the appropriate category name in the **Shopping.com Category** field on the Store subtab of the item record. Visit [Shopping.com's category page](https://merchants.shopping.com/Taxonomy.xml) to download the taxonomy guide. |
| Ground Shipping | shipping rate\* | NetSuite product feed results display the value in the **Shipping Cost** field on the Basic tab on the item record. Note: Use 0 to denote free shipping. |
| Weight | shipping weight | The weight of the item in pounds. In NetSuite, the product feed results display the value in the **Item Weight** field on the Basic tab of the item record. |

### Related Topics

-   [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html)
-   [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html)
-   [Yahoo! Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html)
-   [NexTag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html)
-   [Shopzilla](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html)
-   [Google Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
