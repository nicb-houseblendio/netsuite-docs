---
id: "section_N2642171"
type: "section"
title: "NexTag"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Setting Up Website Product Feeds > NexTag"
parent: "section_N2639492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html"
anchors: ["procedure_N2642204"]
sha256: "9729659c3e26d702f0bc25a168369eb88066f0f107a00fa0968c4db2565ba0e5"
---

You must create an account with NexTag to upload your product feed. Visit [merchants.nextag.com](http://merchants.nextag.com/serv/main/buyer/LoginOrRegister.jsp) to set up an account.

You might need to change some column names in the NetSuite product feed results to comply with requirements from NexTag. For more information, read [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html).

#### To upload your product feed file to NexTag: {#procedure_N2642204}

1.  Log in to your NexTag account.
    
2.  On the **Partner Dashboard**, click **Set Listing Options**.
    
3.  Choose the option, **To display your products on NexTag**.
    
4.  For **File Format**, select **Other File Format**.
    
5.  For **Upload Method**, select **Upload a Product File from your computer**.
    
6.  Click **Browse**, and then find the file on your computer.
    
7.  Click **Update**.
    

The table below shows the fields displayed in your NetSuite product feed, and the fields that are required or recommended by NexTag. The fields that appear with an asterisk are required. Other fields are recommended. Visit [NexTag's product file specifications](https://merchants.nextag.com/serv/main/buyer/ProductFileSpecs.jsp) page for more information.

| NetSuite | NexTag | Notes |
| --- | --- | --- |
| Manufacturer | Manufacturer\* | This is the brand of the product |
| Manufacturer's Part # (SKU) | Manufacturer's Part # (SKU)\* | Use the manufacturer part number or your SKU. This column displays the value in the **MPN** field on item records. If you sell books, music, or software rename this column:
-   ISBN for books.
-   MUZE ID for music.
-   DISTRIBUTOR ID for Software products.

 |
| Product Name | Product Name\* | The value for this field comes from the **Item Name/Number** field on the Item record. Nextag displays product names up to 80 characters long. |
| Description | Product Description\* | The value for this field comes from the **Detailed Description** field on the Store Subtab of the Item record. Do not use HTML or control characters in the data feed you send to NexTag. Also, do not use promotional language such as 'free shipping' or 'sale item'. |
| Item URL | Click-Out URL\* | The URL displayed in product feed results is the link to the item in your web store. |
| Price | Price\* | Product feed results in NetSuite display the online price level as defined on the Web Site Setup form. If you use NetSuite OneWorld, and you filter the list by subsidiary, the price displayed is the default currency for the subsidiary you selected. For successful upload to Yahoo Shopping, the price must be in US dollars, with a decimal point and no currency symbol. |
| Category | Category: NexTag Numeric ID\* | Enter the appropriate category information in the **NexTag Category** field on the Store subtab of the item record. Visit [NexTag's category codes](http://merchants.nextag.com/serv/main/buyer/BulkCategoryCodes.jsp) page for the complete list of category names. |
| Image URL | Image URL\* | The URL displayed in product feed results is the link to the image associated with the item in your web store. Note: NexTag requires that each row in your product feed file has an image URL. |
| Shipping | Ground Shipping | This column is used for the flat-rate ground shipping price. The value entered here in dollars is displayed with your product listings at NexTag. Entering zero indicates that the product has Free Shipping. Any rows that are left blank in your product feed display shipping as 'See Site' on NexTag. |
| Stock Status | Stock Status | States whether your product is in stock or not. Acceptable values for Stock Status:

-   In Stock
-   Out of Stock

Note that marking your products Out Of Stock does not remove them from NexTag listings. |
| Weight | Weight | In NetSuite, the product feed results display the value in the **Item Weight** field on the Basic tab of the item record. NexTag can calculate your shipping based on weight. If you use UPS, FedEx, or USPS to deliver your products, NexTag automatically displays the correct cost of shipping. |

### Related Topics

-   [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html)
-   [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html)
-   [Yahoo! Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html)
-   [Shopzilla](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html)
-   [Shopping.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html)
-   [Google Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
