---
id: "section_N2191818"
type: "section"
title: "Costing Methods"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Costing Methods"
parent: "chapter_N2191369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html"
anchors: ["bridgehead_N2192095"]
sha256: "f77bb09c4f2c38bdb0cf744040472427bd5236c2f61c4d802ceafc830c1d5f16"
---

The inventory costing method you choose defines how NetSuite calculates item costs. For example, it shows how NetSuite handles inventory costing calculations when you buy the same item at different purchase prices over a certain period.

NetSuite provides the following inventory costing methods:

-   **Average** - NetSuite calculates average cost as the total units available during a specific date range, then divides them by beginning inventory cost plus any additions. This is called the moving average method.
    
-   **First-In, First-Out (FIFO)** - NetSuite assumes the first goods you buy are the first ones you sell. Therefore, your ending inventory has the most recently purchased goods. This method helps you track different shipments of similar products.
    
-   **Group Average** - This costing method lets you track one average cost for an item across multiple locations within a defined group. For more information, see [Group Average Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html).
    
-   **Last-In, First-Out (LIFO)** - NetSuite assumes the last goods you buy are the first ones you sell. Therefore, your ending inventory has the first goods purchased.
    
    Note:
    
    Last-In, First-Out (LIFO) isn't available in the NetSuite Australia (AU) edition.
    
-   **Specific** - This method uses the exact cost of a serial number you enter.
    
-   **Lot Numbered** - Lot items track the purchase, stock, and sale of a group or quantity of items. It assigns a specific number to the group or quantity. For more information, see [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html).
    
-   **Standard** - This costing method lets you track standard costs for items and to track variances between these expected costs and actual costs. For more information, see [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html).
    

In NetSuite, average costing is the default inventory costing method. If inventory levels are negative, NetSuite uses the last purchase price as the inventory costing method.

Important:

You can't change the costing method after you save it on the item record.

The item cost for each costing method varies as shown in the following example.

On Monday, you buy 20 calculators at $10 each and place them to inventory.

On Tuesday, you buy 20 more at $15 each.

On Wednesday, you sell 5 calculators to a customer.

Here's how NetSuite calculates the recorded cost of the calculators based on different costing methods:

| **FIFO** | The 5 calculators post a cost of $10 each because that's the cost of the first calculators added to inventory. |
| --- | --- |
| **LIFO** | The 5 calculators post a cost of $15 each because that's the cost of the last calculators added to inventory. |
| **AVERAGE** | The 5 calculators post a cost of $12.50 because that's the average cost of all calculators in inventory. This is calculated as \[(20 x $10) + (20 x $15)\] /40 = 12.5. |
| **STANDARD** | Using standard costing, the receipt cost is fixed.
-   Monday, you buy 20 calculators at $10 each and the standard cost is $11. The item received has a unit cost of $11 and purchase price variance is generated for -$1 for each item being received.
-   Tuesday, you buy 20 calculators at $15 each and the standard cost is $11. The item received has a unit cost of $11 and the purchase price variance is generated for $4 for each item being received.
-   Wednesday, you sell 5 calculators to a customer. The recorded cost is $11.

 |
| **Group Average** | See [Group Average Costing Use Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html#bridgehead_4363954253). |
| **Lot Numbered** | See [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html). |

## When Item Cost Is Calculated {#bridgehead_N2192095}

Using any costing method, NetSuite calculates the cost for items based on the cost shown on the transaction that brings the item into inventory.

For example, you use Advanced Receiving and the workflow Purchase Order > Item Receipt > Vendor Bill. The item cost NetSuite uses is the cost shown on the item receipt.

If you change the cost used for an item, the costing timing also changes. For example, you enter an item receipt showing one cost. Later, the bill from the vendor shows another cost. If you change the cost on the vendor bill, NetSuite doesn't update item costing. Instead, it uses the receipt that brought the items into inventory. Therefore, you need to update the cost that appears on the item receipt to update the item costing.

Any variance between the receipt and the bill shows up in the Accrued Purchases account. If there are closed periods between the original receipt with the incorrect rate and the current date, you need to create an inventory adjustment. Use an inventory adjustment worksheet in the current period, and post to the adjustment account Accrued Purchases. If you reopen old periods and edit the receipt to match the bill, it'll affect your past financial records. This may cause a recalculation of inventory costs from that point forward.

### Related Topics

-   [Setting Inventory Costing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html)
-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html)
-   [Selecting a Default Cost of Goods Sold (COGS) Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2192814.html)
-   [Inventory Costing and Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194190.html)
-   [LIFO/FIFO Inventory Costing and Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html)
-   [System Cost of Goods Sold Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html)
-   [Viewing Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197076.html)
-   [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)
-   [Troubleshoot Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4447393386.html)
-   [Cost Accounting Status on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199228.html)
-   [Item Return Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
