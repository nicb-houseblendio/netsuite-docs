---
id: "section_N2258046"
type: "section"
title: "Converting Non-Inventory Items to Inventory Items"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Management Setup > Converting Non-Inventory Items to Inventory Items"
parent: "chapter_N2249539"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2258046.html"
anchors: ["subsect_0327032006", "bridgehead_N2258197"]
sha256: "093db7a67b9c13fda156751c4b4845492aa4342e6e7ed2ec4171d97f20beaa2e"
---

Items originally set up as a non-inventory or other charge type can be converted to inventory items to allow tracking of the item stock.

For example, an item that you sell but don't stock may become more popular over time. Eventually, it may be to your advantage to keep the item in stock.

When you convert into an inventory item, you keep all records in one place. You keep the transaction history of the item prior to conversion to an inventory item, and all inventory data after the conversion.

If you use the Advanced Inventory Management feature, then order calculations do consider past sales when the item was not an inventory item. This feature and other capabilities such as auto-calculated reorder point and preferred stock level are enabled for a converted item.

Note:

You must have **Edit** permission for Items to see the **Convert** button and be able to convert items. See [Setting Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288727.html).

## Converting into Regular, Lot, or Serialized Inventory {#subsect_0327032006}

You can convert into a regular inventory item type. If you use the Lot Tracking or Serialized Inventory feature, you can also convert into lot or serialized items, respectively.

#### To convert into regular, lot, or serialized inventory:

1.  From the Menu, go to Lists > Accounting > Items.
    
2.  From the Items page, next to the non-inventory or other charge item, click **View**.
    
3.  On the item page, from the **More Actions** submenu, select **Convert to Inventory**. Then, click one of the following options:
    
    -   To convert into a regular inventory item, click **Convert to Inventory**.
        
    -   To convert into a serialized inventory item, click **Convert to Serialized Inventory**.
        
    -   To convert into a serialized inventory item, click **Convert to Lot Numbered Inventory**.
        
4.  On the **Accounting** subtab, select the **Cost of Goods Sold** account for the inventory item.
    
    Converted inventory items must use a Cost of Goods Sold (COGS) account that's different from the expense account selected. This is because non-inventory items use an expense account only to associate the cost of buying the item. The account isn't used for inventory costing calculations, the way inventory items use them.
    
    NetSuite uses the expense account selected in inventory costing calculations. Therefore, the expense account for the inventory item cannot be identical to the COGS account.
    
    This is effective when you convert any For Resale or For Purchase non-inventory or other charge item types.
    
5.  Click **Save**.
    
    Important:
    
    After you click **Save**, the conversion is complete and cannot be undone. You can't convert inventory items to non-inventory or other charge item types.
    

## Transactions and Converted Items {#bridgehead_N2258197}

After you convert an item record, the state of the item is tracked on a per-transaction basis. Some transactions created before the conversion may remain open and still need to use the item as a non-inventory or other charge item.

Transactions created prior to the conversion that used the item as a non-inventory or other charge item continue to use the same item type. It applies to cases like sales orders that may be only partially processed.

In the transaction history of the item, past instances continue to be treated as non-inventory or other charge. Line items on these transactions include **Non-inventory** or **Other Charge** in the item name to distinguish them.

Note:

If you edit a transaction to remove and then re-add the item, the item is then treated as an inventory item.

All transactions created after the conversion that include the item treat the item the same as any regular inventory item.

View the transaction history for an item on the History subtab of the item record.

### Related Topics

-   [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html)
-   [Inventory Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161970666917.html)
-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Configuring Per-Line Locations for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162024160153.html)
-   [Setting the Inventory Level Warnings Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2254698.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
