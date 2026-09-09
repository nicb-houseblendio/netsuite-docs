---
id: "section_N2183023"
type: "section"
title: "Assigning a Foreign Currency Price to a Sales Item"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Using Multiple Pricing > Assigning a Foreign Currency Price to a Sales Item"
parent: "section_N2181607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183023.html"
anchors: ["procedure_N2183043", "procedure_N2183120"]
sha256: "ba7f121878c6c8700f3b121c960b3158627f44fc8f58c60943a783f6aefe16e3"
---

With the Multiple Currencies feature enabled, you can assign foreign currency prices to your sales items at each price level. You can assign prices to items for each currency for which you've created a Currency record.

These foreign currency prices remove exchange rate risk for customers who use the same currency as the item. But this means your company takes on the exchange rate risk. The foreign currency price stays the same, but the base currency price changes with exchange rates.

#### To assign a foreign currency price to a sales item with Multiple Prices turned off: {#procedure_N2183043}

1.  Go to _Lists > Accounting > Items_.
    
2.  On the Items list, click **Edit** next to the item you want to set a foreign currency price for.
    
3.  On the item's record, click the **Sales/Pricing** subtab.
    
4.  Enter the price, denominated in the foreign currency, as an **Alternate Price**.
    
    All items must have a **Base Price** entered in your base currency.
    
5.  Repeat step 4 for each price.
    
6.  Click **Save**.
    

#### To assign a foreign currency price to a sales item with Multiple Prices enabled: {#procedure_N2183120}

1.  Go to _Lists > Accounting > Items_.
    
2.  On the Items list, click **Edit** next to the item you want to set foreign currency prices for.
    
3.  Click the **Pricing** subtab.
    
4.  Click the currency subtab for which you want to set prices.
    
    ![Currency Price](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/CurrencyPrice.png)
5.  Enter a price in the selected currency for each price level.
    
6.  To enter prices in another currency, click the right currency tab and enter prices there.
    
7.  Click **Save**.
    

When you enter transactions for a customer who uses a foreign currency, their price is the one you entered for that currency. If an item doesn't have a price set in a foreign currency, NetSuite converts the base currency price into the customer's default foreign currency. If you pick a preferred vendor for an item, NetSuite shows the purchase price in that vendor's default currency.

### Related Topics

-   [Creating Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181938.html)
-   [Setting Up Items for Multiple Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182221.html)
-   [Setting Up Price Levels for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182485.html)
-   [Editing Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182796.html)
-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
