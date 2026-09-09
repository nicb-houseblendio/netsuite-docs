---
id: "section_N2639492"
type: "section"
title: "Setting Up Website Product Feeds"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Setting Up Website Product Feeds"
parent: "chapter_N2635817"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639492.html"
anchors: ["procedure_N2639717"]
sha256: "aa11bdcdb0b2ab0fc2e457894bbee6117b384e74b665cf81c4e1b5dba8302082"
---

NetSuite enables you to use Product Feed search results to generate a list of items that you can upload to various shopping comparison sites.

For example, if you sell printers in your web store, you can upload a product feed file to Google Base. When shoppers search Google Base for printers, the printers on your web store show in the list of results. Shoppers can see images of your printers, get pricing information and click links from the search results to your web store.

The topics listed below provide detailed information for uploading your product feed to each search engine:

-   [Yahoo! Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html)
    
-   [NexTag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html)
    
-   [Shopzilla](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html)
    
-   [Shopping.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html)
    
-   [Google Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html)
    
    Important:
    
    Google Base has been retired. However, you can still create a saved item search that you can export and use as a product feed. Visit the help page on the Google Merchant Center website for more information about the data feed submission process and specific requirements.
    

If you use NetSuite OneWorld, or multiple websites, see [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html).

The NetSuite product feed results include all items that are associated with a product feed, and marked online in your account. To add an item to a product feed, select the search engine in the **Product Feed** field on the Store subtab of the item record.

Each shopping search engine requires specific information in a product feed file. NetSuite provides the following fields on item records where you can enter this information.

-   **On the Basic subtab:**
    
    -   Manufacturer
        
    -   MPN (Manufacturer's Part Number)
        
    -   Stock Description
        
-   **On the Store subtab:**
    
    -   Shopping.com Category
        
    -   Shopzilla Category
        
    -   NexTag Category
        

The following types of items are included in product feed results: Kit/Package, Non-inventory Item for Sale, Non-inventory Item for Resale, Assembly (lot and serialized), Inventory (lot and serialized).

#### To create a product feed file for upload to a shopping search engine: {#procedure_N2639717}

1.  Go to _Commerce > Site Builder > Marketing/Upsell > Product Feeds_.
    
2.  Select a product feed from the list. The data for your product feed displays on the results screen.
    
    NetSuite provides the basic required fields. However, if you want to add additional fields, or you need to provide information specific to the products you sell, such as MUZID for music, or ISBN for books, you can edit the saved search. For specific steps describing how to add or rename columns, see [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html).
    
3.  Click the Excel icon to export the list in CSV file format.
    
4.  Verify that the data in the spreadsheet complies with the requirements from the search engine to which you plan to export the product feed.
    
    Note:
    
    Click the links at the top of this page to verify data requirements for each search engine.
    
5.  After you have the correct column names and your spread sheet is complete, select the **Save As** option from the **File** menu.
    
6.  Save the file in the file format required by the search engine to which you plan to export the list.
    
    For most search engines, choose Text (Tab delimited) in the **Save as type** field. Shopping.com gives you the option to save the file in Excel or CSV format.
    
7.  Enter a file name based on instructions for the search engine to which you plan to upload the product file.
    
    For example: Yahoo! Shopping requires that the file is named **data.txt**.
    
8.  If you see an alert when saving your file, indicating that your file may contain features that are not compatible with the Text (Tab delimited) format, ignore it. Click **Yes** to save the file.
    

Note:

Use Inline Editing to quickly enter product feed information on your items list. Go to Lists > Items > Search. On the **Criteria** tab, add **Display in Web Site**, select **Yes**, and also add the item type. On the **Results** tab, add the fields that require data for your product feeds.

### Related Topics

-   [Editing Product Feed Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2640999.html)
-   [Using Product Feeds with Multiple Websites and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641217.html)
-   [Yahoo! Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2641420.html)
-   [NexTag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642171.html)
-   [Shopzilla](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2642966.html)
-   [Shopping.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2644262.html)
-   [Google Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645022.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
