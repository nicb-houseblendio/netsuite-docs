---
id: "section_N2195087"
type: "section"
title: "System Cost of Goods Sold Adjustments"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > System Cost of Goods Sold Adjustments"
parent: "chapter_N2191369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html"
anchors: []
sha256: "a835387debeeb03eb1b8ebf2f21a052fd0811e44d5a57862eb6d4cae26403641"
---

When you sell an item that's in stock, NetSuite reduces the total in the inventory asset account, and increases the total in the COGS account. When you sell an item that's not in stock, NetSuite makes an adjustment to the on-hand value of the item. This adjustment is called a system COGS adjustment, which can show in financial reports or on transactions.

System COGS adjustments help track inventory costing used in many accounting systems. When an item isn't in stock, NetSuite estimates the cost of goods sold based on historical data. If there's no historical data, NetSuite uses the cost you entered to estimate the cost of goods sold.

Later, when you add the item to your inventory again, NetSuite creates a linked COGS adjustment entry. This COGS adjustment happens anytime a transaction creates a positive inventory level from a negative one, including the ones listed below:

-   Vendor Bill
    
-   Purchase Order Receipt
    
-   Assembly Unbuild
    
-   Inventory Adjustment
    

This COGS adjustment only changes the on-hand value using this calculation:

-   \[the estimated COGS (when you were out of stock)\] - (the cost of the item when you added it back to stock)
    

Below are example posting asset lines on item receipts and fulfillments:

| **Item #ABC100** | **Day 1** | **Day 2** | **Day 3** |
| --- | --- | --- | --- |
| **Beginning On Hand** | 0 | 0 | \-3 |
|  |  |  |  |
| **Item Receipt Quantity** | 10 | 0 | 20 |
| **Item Receipt Value** | $15.00 | $0.00 | $35.00 |
| **Item Average Cost** | $1.50 | $0.00 | $1.75 |
| **Item Fulfillment** | 10 | 3 | 0 |
| **Item Fulfillment COGS** | $15.00 | $4.50 | $0.00 |
| **Item Fulfillment COGS Adjustment** | $0.00 | $0.00 | $0.75 |
|  |  |  |  |
| **Ending On Hand** | 0 | \-3 | 17 |
| **Ending On Hand Value** | $0.00 | $0.00 | $29.75 |

Note:

For costing purposes, NetSuite considers increases to inventory before reductions to inventory.

For transactions that trigger an inventory adjustment, NetSuite considers all positive adjustments first and all negative adjustments last.

For example, you enter an invoice that includes Item A at 6:00 am. You enter a vendor bill for Item A at 7:00 am, both on the same day. After you save the vendor bill, NetSuite recalculates the item cost for the invoice as if the vendor bill had been entered before the invoice. The vendor bill added the item to the inventory, therefore was considered ahead of the invoice, which removed the item from inventory.

Note:

If you need to enter a negative adjustment that comes first before a positive one, you need to enter the two adjustments on different days. Enter the negative adjustment on one day and the positive adjustment on the next day.

When you enter transactions on the same date, they're processed by transaction type in the following order:

1.  Inventory adjustment worksheets (First-in-day)
    
2.  Purchase transactions (purchase receipts, vendor bills, adjustments)
    
3.  Assembly builds, component builds, transfers and transfer orders (including fulfillments and receipts)
    
4.  Vendor return fulfillments, assembly unbuilds
    
5.  Sale transactions (sales order fulfillments, invoices, cash sales, and inventory adjustments)
    
6.  Return transactions (credit memos and RMA receipts)
    
7.  Inventory adjustment worksheets (Last-in-day)
    

For vendor returns, differences between the vendor return authorization return cost, and the average cost of the item posts as a COGS adjustment.

### Related Topics

-   [Setting Inventory Costing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html)
-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html)
-   [Selecting a Default Cost of Goods Sold (COGS) Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2192814.html)
-   [Inventory Costing and Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194190.html)
-   [LIFO/FIFO Inventory Costing and Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html)
-   [Viewing Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197076.html)
-   [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)
-   [Troubleshoot Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4447393386.html)
-   [Cost Accounting Status on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199228.html)
-   [Item Return Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html)
-   [Group Average Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
