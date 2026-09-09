---
id: "section_N2181018"
type: "section"
title: "Setting Up Item Pricing"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Setting Up Item Pricing"
parent: "chapter_N2180614"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181018.html"
anchors: ["procedure_N2181026"]
sha256: "aa69342df864ce75f67d836599e3e0801ba025d223f4b35c8c94dbad8b1d2369"
---

Here's how you can set up pricing for items.

#### To set up pricing for items: {#procedure_N2181026}

1.  Open an item record in edit mode, and then click the **Sales/Pricing** subtab.
    
    Note:
    
    To let customers choose the amount of an item, such as a donation or a gift certificate, skip this subtab. Instead, click the **Store** subtab, and then check the **Variable Amount box**.
    
    If you enter a price on the **Sales/Pricing** subtab, and then check the **Variable Amount** box, that price becomes the default amount.
    
2.  Under Pricing, if you use quantity pricing schedules, select the pricing schedule you want for this item. When you select a schedule, it sets the **Use Marginal Rates** and **Calculate Quantity Discounts** fields.
    
    You can create pricing schedules at _Lists > Accounting > Quantity Pricing Schedules > New_.
    
3.  Check the **Use Marginal Rate** box if you want the quantity discounts to apply to each pricing bracket separately.
    
    For example, if a schedule gives no discount for the first 100 items and a 5% discount for anything over 100, selling 150 means the first 100 are at the normal price and the other 50 get a 5% discount.
    
    Leave this box unchecked if you want the discount to apply to all items sold.
    
4.  In the **Calculate Quantity Discounts** field, choose how you want to determine the quantity for pricing:
    
    -   **By Line Quantity** - pricing is based on the quantity in the line item.
        
    -   **By Overall Item Quantity** - pricing is based on all line items for the same item on a transaction.
        
    -   **By Overall Parent Quantity** - pricing is based on all items with the same parent item on the transaction. This can be useful for applying quantity pricing to matrix items.
        
    -   **By Overall Schedule Quantity** - pricing is based on all items using the same pricing schedule in the transaction.
        
5.  In the **Pricing Group** field, select the pricing group for this item. Using pricing groups lets you set customer-specific price levels for a group of items.
    
6.  Click **Save**.
    

### Related Topics

-   [Using Multiple Prices or Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1493655077.html)
-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)
-   [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html)
-   [Creating Pricing Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184077.html)
-   [Updating Item Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184312.html)
-   [Updating Item Purchase Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184741.html)
-   [Swapping Prices Between Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185052.html)
-   [Creating Item Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185383.html)
-   [Generating Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html)
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)
-   [Last Purchase Price](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html#bridgehead_1499865237)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
