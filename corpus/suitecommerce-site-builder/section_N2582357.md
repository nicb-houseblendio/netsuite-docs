---
id: "section_N2582357"
type: "section"
title: "Setting Web Store Back Order and Out-of-Stock Preferences"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Setting Web Store Back Order and Out-of-Stock Preferences"
parent: "chapter_N2576231"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2582357.html"
anchors: ["procedure_N2582377", "procedure_N2582504"]
sha256: "738d34879fe0a91b1fb04fa81ced2380d1e3f7f0d23e96859083c5664f3736b0"
---

The instructions below explain how to specify preferences for back orders and selling out-of-stock items in your Site Builder web store.

#### To set up back order preferences for the site: {#procedure_N2582377}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to a website.
    
3.  Click the **Shopping** subtab.
    
4.  In the **Webstore Out Of Stock Items** field, select how to handle items that are out of stock in your web store:
    
    -   **Allow back orders but display out-of-stock message -** Customers can purchase an out-of-stock item. A message appears beside the item in your store informing customers this item is out of stock. However, this item can be purchased and processed through your shopping cart.
        
    -   **Allow back orders with no out-of-stock message -** Customers can purchase an out-of-stock item. No message is posted saying this item is out of stock.
        
    -   **Disallow back orders but display out-of-stock message -** Customers cannot purchase an out-of-stock item. A message appears beside your item in your store informing customers this item is out of stock. The Add to Shopping Cart link is removed from beside this item.
        
    -   **Remove out-of-stock items from store -** Customers cannot purchase out-of-stock items because they are automatically removed from your store until their supply is replenished.
        
        Note:
        
        If you choose this setting and turn on the Multi-Location Inventory feature, items do not show in your web store until after they have been distributed.
        
5.  Click **Save**.
    

Note:

The **Disallow back orders but display out-of-stock message** or **Remove out-of-stock items from store** option does not prevent you from adding the out of stock items to the shopping cart using the `additemtocart.nl` request handler or the `addItem(item)` and `addItems(items)` order methods. However, when you try to place the order with such out of stock items in your shopping cart, an error message is displayed and you will not be able to place the order successfully.

You can also set the out-of-stock messages and the out-of-stock behavior for each item individually. Use the following instructions to modify settings on the item record.

#### To set up out of stock behavior on the item record: {#procedure_N2582504}

1.  Go to Lists > Accounting > Items.
    
2.  **Edit** the item record.
    
3.  Click the **Web Store** subtab.
    
4.  In the **Out of Stock Message** field, enter an out-of-stock message you want to display when this item is out of stock.
    
5.  In the **Out of Stock Behavior** field, select an option for back-ordering items that are out of stock in your web store.
    
6.  Click **Save**.
    

The settings on the item record override the preference on the Set Up Web Site page.

Note:

If you use the Advanced Inventory Management feature, you can use a NetSuite Web Site Tag to display the lead time for when you expect the item will be in stock. For example: This item will be back in stock in <%=getAttribute('item',id,'storeleadtime')%> days.

### Related Topics

-   [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html)
-   [Setting Up Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518563504.html)
-   [Setting Order Amount and Quantity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518566247.html)
-   [Best Practices for Website Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2461527.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
