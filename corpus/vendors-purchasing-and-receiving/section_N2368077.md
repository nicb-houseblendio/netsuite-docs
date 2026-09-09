---
id: "section_N2368077"
type: "section"
title: "Importing a Vendor Price List"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Configuration > Importing a Vendor Price List"
parent: "article_161952107343"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368077.html"
anchors: ["procedure_N2368098"]
sha256: "63fccdefee4c1e04dd669f73bb628a8a740969bbee3bab0a5b34a4f5a3f9119b"
---

On the vendor record, you can list items available from that vendor and specify the vendor codes and prices for that item. You also can use CSV import to import vendor price lists from an existing comma delimited file.

If you use the Multiple Currencies feature, you can import prices for an individual item in multiple currencies.

For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).

#### To import a vendor price list: {#procedure_N2368098}

1.  Create the import file.
    
    The import file should contain the following fields in order, with no header row:
    
    Note:
    
    For the import to succeed, each row of the CSV file must contain values separated by commas or other supported column separators. For example, semicolon, pipe, space, and tab.
    
    -   **Item Name** (For initial import, the item name must be present. For later updates, it is not required as the vendor code is used to identify each item.)
        
    -   **Vendor Code** (If your vendor uses a name for this item that is different from the name you use, note the following. You can enter up to 60 characters as the vendor's name for this item.)
        
    -   **Purchase Price**
        
    -   **Price Schedule** (optional)
        
    -   **Currency** (This field is present only if you use the Multiple Currencies feature.)
        
    
    Important:
    
    The items listed in the file must already exist in your NetSuite account and the names must exactly match those in your account.
    
2.  Go to _Lists > Relationships > Vendor_.
    
3.  Click **Edit** next to the vendor record.
    
4.  Click the **Financial** subtab.
    
5.  Click the **Items** subtab.
    
6.  Click **Import Price List**.
    
    The Import Vendor Price List popup window opens.
    
    Note:
    
    You must use the Multiple Vendors feature to import a price list.
    
7.  Click **Browse** and go to the vendor price list file.
    
8.  Click **Save**.
    

Upon successful import, each item from the imported vendor price list is listed on the Items subtab with the associated vendor codes and prices. The vendor record also is displayed on the Vendor subtab of each item's record with the vendor name, vendor's item code and purchase price.

### Related Topics

-   [Vendor Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161951406143.html)
-   [Enabling the Vendor Access Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952527878.html)
-   [The Vendor Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369118.html)
-   [Assigning a Role to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2363606.html)
-   [Giving Vendors Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364581.html)
-   [Vendor Records for 1099 Contractors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364122.html)
-   [Vendor Credit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2365918.html)
-   [Associating a Vendor With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367376.html)
-   [Associating a Vendor With a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367472.html)
-   [Preferred Transaction Delivery on Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368449.html)
-   [The Multiple Vendors Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369578.html)
-   [Vendor Record Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952107343.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
