---
id: "section_N1083860"
type: "section"
title: "Absolute Pricing for Customers"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Customers > Creating a Customer Record > Entering Financial Information for the Customer > Absolute Pricing for Customers"
parent: "section_N1078064"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1083860.html"
anchors: ["procedure_N1083900"]
sha256: "ac5c9013f85cb296ab54a2c1920f1bbd8075285c323e8477e6542fcd548882df"
---

On customer records, you can set an absolute price for each item that is specific to the customer. An absolute price always overrides any other pricing that's been set up, such as a price level. The absolute price is always used on sales transactions for the customer.

To set absolute prices for customers, an administrator must first enable the Multiple Prices feature. You can set up to a maximum of 1,000 price levels. For information, see [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html).

If you use the Multiple Currencies feature, you can enter absolute prices in any of a customer's transaction currencies. For information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

#### To set an absolute price: {#procedure_N1083900}

1.  Go to _Lists > Relationships > Customers_.
    
2.  Click **Edit** next to the customer name.
    
3.  On the customer record, click the **Financial** subtab.
    
4.  On the **Item Pricing** subtab, select the item you want to price.
    
5.  In the **Price Level** field, select **Custom**.
    
6.  If you use the Multiple Currencies feature, select the currency you want to set an absolute price in.
    
7.  Enter a price in the **Unit Price** field.
    
    Enter the price you want to always charge this customer for this item. Absolute prices you set here override all other prices.
    
8.  Click **Add**.
    
9.  Repeat these steps for all items and currencies you want to set an absolute price for.
    
10.  Click **Save**.
     

The absolute price for an item and currency's used in every transaction or price list for that customer with that item. Search results for the customer and item also display the absolute price.

Without an absolute price for an item, regular pricing for items, such as price levels, is used.

For general information about items and pricing, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

### Related Topics

-   [Entering Financial Information for the Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1078064.html)
-   [Managing Customer Credit Limits and Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1080144.html)
-   [Tracking Customer Credit Card Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
