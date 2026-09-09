---
id: "section_N2369863"
type: "section"
title: "Associating an Item With Multiple Vendors"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Configuration > The Multiple Vendors Feature > Associating an Item With Multiple Vendors"
parent: "section_N2369578"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369863.html"
anchors: ["procedure_N2369875"]
sha256: "f460112993bc8b9af8094ef65b809f4e72644c7232e64445c241802766f42b90"
---

After you have created a vendor record, you can select that vendor on an item record to associate the vendor with the item.

#### To associate an item with multiple vendors: {#procedure_N2369875}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to an item.
    
3.  On the **Purchasing/Inventory** subtab, click the **Vendors** subtab.
    
4.  In the **Vendor** column, choose a vendor.
    
    If you use OneWorld and the vendor is shared with multiple subsidiaries, you can add the vendor multiple times. You can specify an item price for each subsidiary level. This lets you set a different item price per subsidiary to the same item record. For more information about globally shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
    
5.  For each vendor, you can identify the following (depending on the features enabled in your account):
    
    1.  **Code** - Enter this vendor's code for this item.
        
    2.  **Currency** - Choose a currency. If you use the Multiple Currencies feature, this column is not shown. You can enter prices in multiple currencies in the **Purchase Price** column.
        
        If you use both Multiple Vendors and Multiple Currencies, when you associate a vendor as preferred for an item, note the following. If you change the vendor's primary currency, the new primary currency is retained and calculates a price for the item.
        
        Note:
        
        In NetSuite OneWorld, the purchase price for an item uses the designated currency of the preferred vendor.
        
        If an item has more then one vendor but no preferred vendor, the currency is based on the subsidiary of the most-recently added preferred vendor.
        
        You should associate one or more vendors with an item including a currency and purchase price for each vendor. This helps ensure that the correct purchase price is used on purchase orders for each vendor.
        
    3.  **Schedule** - Select a quantity pricing schedule, if you use them.
        
    4.  **Preferred** - Check the box to identify the vendor as the preferred vendor. The preferred vendor defaults to show on forms when the item is added.
        
        -   When using the Order Items form, if a preferred vendor is associated with an item, it defaults on each line when the item is added.
            
        -   When viewing the item list, the preferred vendor associated with the item shows by default.
            
        -   If an item has a preferred vendor, then the purchase price is shown on the item record in the preferred vendor currency.
            
    5.  **Purchase Price** - Enter the price you pay this vendor for this item.
        
        If you use the Multiple Currencies feature, click **Set** ![Screenshot of the Multi-Currency icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/VendorsPurchasingReceiving/Vendors/multi-currency_vacant.png), and then enter the prices for this vendor's transaction currencies. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
        
6.  Click **Add**.
    
7.  Repeat these steps for each vendor you want to associate with this item.
    
8.  Click **Save**.
    

After vendor information is entered for items, it is used on forms and transactions where the item appears.

Tip:

When you use Multiple Vendors and then create an item saved search, use the search filter **Name (Internal)**, not the filter **Name**. The **Name (Internal)** filter returns the expected results. For more information, see [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html).

### Related Topics

-   [Enabling the Multiple Vendors Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369744.html)
-   [Multiple Vendors Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4115931525.html)
-   [The Multiple Vendors Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369578.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
