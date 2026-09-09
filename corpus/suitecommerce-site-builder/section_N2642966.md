---
id: "section_N2642966"
type: "section"
title: "Shopzilla"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Setting Up Website Product Feeds > Shopzilla"
parent: "section_N2639492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html"
anchors: ["procedure_N2642996"]
sha256: "da11aba5e95de3e25dc03ac19b228dfccf72032b5ca0fc16c454c502798b1ea1"
---

Use the product feed results in NetSuite to create a datafeed file for Shopzilla's Merchant Listings Service. You must create an account with Shopzilla to upload the file. Visit [merchant.shopzilla.com](https://merchant.shopzilla.com/pp/general/faqs_merchant_listings.xpml#0_1) for information about pricing and setup.

According to the requirements from Shopzilla, your file must not exceed 1 MB. If it does, you must submit your product feed in multiple files. Shopzilla processes data feeds every 36 to 48 hours. For the complete list of requirements from Shopzilla, read [Shopzilla's product inventory specifications](https://merchant.shopzilla.com/pp/product_inventory/specifications.xpml).

#### To upload your product feed file to Shopzilla: {#procedure_N2642996}

1.  Log in to your Shopzilla account.
    
2.  Select the **Product Listing** tool and choose **FullList**.
    
3.  Browse to the product feed file on your computer to upload the file to Shopzilla.
    

The table below shows the columns displayed in your NetSuite product feed results and the columns that are required by Shopzilla. All 15 columns are required in the datafeed. Please note that some columns, as indicated below, cannot be left blank.

Do not delete any of the columns or change the order. This causes your datafeed to fail when you try to submit it.

| NetSuite | Shopzilla | Notes |
| --- | --- | --- |
| Category | Category ID\* | This column must contain data. Data for this field is mapped from the **Shopzilla Category ID** field on the Store subtab on the Item record. Shopzilla's category IDs are displayed on [Shopzilla's category list](http://merchant.shopzilla.com/oa/general/taxonomy.xpml). |
| Manufacturer | Manufacturer\* | Enter data in the **Manufacturer** field on the Basic subtab of Item records. |
| Title | Title\* | This column must contain data. The value for this field comes from the **Item Name/Number** field on the Item record. |
| Description | Description\* | The value for this field comes from the **Detailed Description** field on the Store Subtab of the Item record. Do not use HTML or control characters in the data feed you send to shopzilla. Also, do not use promotional language such as 'free shipping' or 'sale item'. |
| Link | Product URL\* | This column must contain data. The URL displayed in product feed results is a link to the item in your web store. |
| Image | Image URL\* | The URL displayed in product feed results is the link to the image associated with the item in your web store. |
| SKU | SKU\* | This column must contain data. SKU stands for Stock Keeping Unit and is a unique designator for each listing in your feed. Each product in your feed must have a different SKU listed. |
| Quantity on Hand | Availability\* | This field lets your consumers know if the product is currently available on your website. Acceptable values for Availability:
-   In Stock
-   Back-Order
-   Pre-Order
-   See Site
-   Out of Stock
-   Limited Qty
-   Special Order

 |
| Condition | Condition\* | Use this field to designate the state of the product. Acceptable values for Condition:

-   New
-   Refurbished
-   Used
-   Open Box
-   OEM

 |
| Shipping Weight | Ship Weight\* | This field is used to designate the weight of your product (in pounds). This field is required if your store's shipping costs are determined based on an item's weight. |
| Shipping Cost | Ship Cost\* | This field is used to designate a flat shipping cost for the product, if desired. This field is not necessary if you plan to use the Shopzilla Shipping Tool to specify ship costs. Note:

-   To designate free shipping, please use 0.00
-   Shipping cost included in the feed file will override any rules set using the Shipping Tool on the Business Services Web site.

 |
|  | Bid\* | This is an optional field and recommended only for those merchants programmatically setting their product bids. The NetSuite product feeds results do not include this column by default. For more information, see [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html). |
|  | Promotional Code\* | This field is used to add promotional text next to your product. For a detailed list of valid promotional codes, visit [Shopzilla's product inventory specifications](https://merchant.shopzilla.com/pp/product_inventory/specifications.xpml). The NetSuite product feeds results do not include this column by default. For more information, see [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html). |
| UPC | UPC\* | UPC stands for Universal Product Code. UPC numbers have 12 digits, and are found with bar codes on product packaging. |
| Price | Price\* | This column must contain data. Product feed results in NetSuite display the online price level as defined on the Web Site Setup form. If you use NetSuite OneWorld, and you choose a subsidiary in the list at the bottom of the product feeds page, the price displayed is the default currency for the subsidiary. |

### Related Topics

-   [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html)
-   [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html)
-   [Yahoo! Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html)
-   [NexTag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html)
-   [Shopping.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html)
-   [Google Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
