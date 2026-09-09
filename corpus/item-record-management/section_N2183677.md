---
id: "section_N2183677"
type: "section"
title: "Quantity Pricing Schedules"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Using Quantity Pricing > Quantity Pricing Schedules"
parent: "section_N2183333"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183677.html"
anchors: ["procedure_N2183693"]
sha256: "47669ae8693b419b334b73d2f44409544506c29d1c5c5c35cbf7fd9992e46ca5"
---

Quantity pricing schedules are templates you can use on items to set purchase and sale prices. When you apply a quantity pricing schedule to an item, prices for all price levels are created automatically.

Note:

Before you can create quantity pricing schedules, you need to enable the Quantity Pricing feature and set quantity pricing preferences. For more information, see [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html).

#### To create a pricing schedule: {#procedure_N2183693}

1.  Go to _Lists > Accounting > Quantity Pricing Schedules > New_.
    
2.  Enter a quantity pricing schedule **Name**.
    
3.  To base your quantity pricing schedule on a unit of measure instead of a number, select a **Units Type**.
    
4.  Select the related **Units** you want to base this schedule on.
    
    For example, if you select quartz as the **Units Type**, the available **Units** are Qt, Smp bx, or bx.
    
5.  To apply quantity discounts to each pricing bracket separately, check the **Use Marginal Rates** box.
    
    For example, a schedule gives no discount for the first 100 items sold and a 5% discount on all additional items sold. If 150 items are sold, the first 100 are at normal price, and the other 50 items are sold at a 5% discount.
    
    To apply the discount to all items sold, clear this box.
    
6.  To mark this pricing schedule as inactive, check the **Inactive** box.
    
7.  In the **Calculate Quantity Discounts** field, choose how you want to determine the quantity for pricing:
    
    -   **By Line Quantity** - pricing is applied according to the quantity included in the line item.
        
    -   **By Overall Item Quantity** - pricing is applied for all line items for the same item on a transaction.
        
    -   **By Overall Parent Quantity** - pricing is applied for all items with the same parent item on the transaction. This can be useful for applying quantity pricing to matrix items.
        
    -   **By Overall Schedule Quantity** - pricing is applied to all items that use the same pricing schedule that are included in the transaction.
        
    
    Note:
    
    You can only have 4 non-zero quantity levels.
    
8.  In the **Quantity** and **Discount** fields, enter the brackets for the schedule.
    
    If you enabled different discount percentages per price level while setting quantity pricing preferences, set the **Qty** and **Default Discount %** for each **Price Level**:
    
    -   **Base Price**
        
    -   **Alternate Price 1**
        
    -   **Alternate Price 2**
        
    -   **Alternate Price 3**
        
    -   **Online Price**
        
9.  Click **Save**.
    
    Tip:
    
    When you create a new item record, fill out the **Sales/Pricing** subtab and select the **Quantity Pricing Schedule** to generate prices for this item. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    

You can use quantity pricing schedules to apply prices you have negotiated with vendors.

#### To associate a pricing schedule with a vendor:

1.  Go to Lists > Relationships > Vendors.
    
2.  Click **Edit** next to the vendor record with which you want to associate a pricing schedule.
    
3.  Click the **Financial** subtab.
    
4.  Click the **Pricing Schedules** subtab, and then click **New Pricing Schedule**.
    
    The vendor quantity pricing schedule includes a **Base Discount** field.
    
5.  After you complete the vendor quantity pricing schedule, click **Save**.
    
    You can only link one vendor to each quantity pricing schedule, but you can apply a schedule to as many items as you want.
    

### Related Topics

-   [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html)
-   [Imports Using Quantity Pricing Schedules Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N380976.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
