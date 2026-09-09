---
id: "section_N2181938"
type: "section"
title: "Creating Price Levels"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Using Multiple Pricing > Creating Price Levels"
parent: "section_N2181607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181938.html"
anchors: ["procedure_N2181975"]
sha256: "f0fd6ae17711c9aa37565d7f751803870f386b365f4d6d1d8161420fdcff46fb"
---

When you use the Multiple Pricing feature, you can create different price levels for selection on the sales order, up to 1,000 active records. Setting up multiple price levels gives you more flexibility to set different prices for different customers.

For example, you want to sell items to some customers at retail prices, but offer discount prices to other customers. Set up multiple price levels to sell items at a retail price, or give discounts of 5%, 10%, or 15% off retail pricing.

#### To enable multiple pricing:

1.  Go to _Setup > Company > Setup Tasks > Enable Features._.
    
2.  Click the **Transactions** subtab.
    
3.  Check the **Multiple Prices** box.
    
4.  Click **Save**.
    

#### To create a new price level: {#procedure_N2181975}

1.  Go to _Setup > Accounting > Setup Tasks > Accounting Lists > New_.
    
2.  Click **Price Level**.
    
3.  On the Price Level page, enter a name in the **Price Level** field.
    
    This name should describe the price level you are creating.
    
4.  In the **Markup/Discount %** field, you can enter a positive or negative percentage to mark up or discount prices for this price level.
    
    Prices for this level are calculated by applying the + or - percentage to the Base Price level.
    
    Note:
    
    Any value you enter gets rounded to the nearest 0.01%.
    
5.  To update all items using this price level, check the **Update Existing Prices** box.
    
    When you create a new item record with this price level, the item price updates automatically.
    
6.  To make this your online price level, check the **Online Price Level** box.
    
7.  Check the **Inactive** box to inactivate this record.
    
    After a record is marked inactive, it won't show up in NetSuite lists and popup windows. You can still see inactive records on list pages by checking the **Show All** box.
    
    Clear the **Inactive** box if you want this price level to show up in lists.
    
8.  Click **Save**.
    

After you create price levels, enter prices for them on item records. Go to _Lists > Accounting > Items._. Then you can select the right price levels when creating invoices.

### Related Topics

-   [Setting Up Items for Multiple Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182221.html)
-   [Setting Up Price Levels for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182485.html)
-   [Editing Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182796.html)
-   [Assigning a Foreign Currency Price to a Sales Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183023.html)
-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
