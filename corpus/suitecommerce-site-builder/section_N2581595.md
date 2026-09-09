---
id: "section_N2581595"
type: "section"
title: "Multiple Website Online Pricing"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Creating Multiple Websites > Multiple Website Online Pricing"
parent: "section_N2580798"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581595.html"
anchors: ["procedure_N2581614", "procedure_N2581676", "procedure_N2581718", "bridgehead_N2581795"]
sha256: "afdec7f7d23b9ae944f5d70b029b5c29e6328370ffba4e026bb9208492e02f24"
---

You can create multiple online price levels, enter different online prices for your items, and then choose which online price should display for items on your web store.

If you have multiple websites, you can display the same item on different sites with different price levels on each site. For example, you may want to display items with discount or wholesale pricing on one of your websites, while another site displays the retail price.

To apply a price level to items in your web store, first create the price level. Then, enter the price for this price level on the item record, and finally, apply the price level to your web store.

#### To create the price level you want to apply to items in your website: {#procedure_N2581614}

1.  Go to Setup > Accounting > Accounting Lists > New.
    
2.  Select **Price Level**.
    
3.  Click **New**.
    
4.  In the **Price Level** field, enter a name for your new price level. For example, you might include the website name in the price level name.
    
5.  You can enter a positive or negative percentage in the **Markup/Discount %** field to mark up or discount prices that may already exist for this price level.
    
    If you want to update all items with prices at this price level, check the **Update Existing Prices** box to apply the markup or discount.
    
6.  Check the **Online Price Level** box.
    
7.  Click **Save**.
    

#### To enter a value for the new price level on an item record: {#procedure_N2581676}

1.  Go to Lists > Accounting > Items.
    
2.  Click **Edit** next to an item.
    
    On the **Pricing** subtab, you will see a field for your new price level.
    
3.  Enter a price for the new price level.
    
4.  Click **Save**.
    

#### To choose which price level to apply to a website: {#procedure_N2581718}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to the site you want to modify.
    
3.  Click the **Setup** subtab.
    
4.  In the Multi-Site Settings section, set the **Price Level** field.
    
5.  Click **Save**.
    

Now items displayed on the site show prices from the price level you defined on the item records.

If you do not enter a price for the new price level field on an item record, that item displays the default online price. Customers who have a price level defined on their customer record continue to see their price level when they log in on any of your websites. For more information, see [Site Builder and OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2466850.html).

## Multiple Website Pricing and the Customer Center {#bridgehead_N2581795}

When a shopper enters a sales order from the My Account tab on your web store, items on the sales order form display the price level for the site.

When a shopper logs into the Customer Center from www.netsuite.com, they see the price level for the last web store they visited. If your customer has not visited any of your websites, they see the price level assigned to your primary website.

### Related Topics

-   [Publishing Content with Multiple Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581200.html)
-   [Creating Hosting Root Folders for Multiple Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581907.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
