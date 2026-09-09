---
id: "section_N2296970"
type: "section"
title: "Inventory Count"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Count"
parent: "chapter_N2250682"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296970.html"
anchors: ["subsect_0319025034", "subsect_0319025259"]
sha256: "a3869b779600eb172680bd98bddb0e659a3bc3e08b7ee13d9157fa4a2196cffe"
---

The Inventory Count feature enables improved tracking of inventory and tighter control over assets. You can enter regular periodic counts of on-hand item quantities to maintain inventory accuracy. Keeping an accurate item count can help reduce required safety stock, which lowers your overhead costs.

The Advanced Bin/Numbered Inventory Management feature must be enabled to support inventory counts of serialized or lot numbered items.

## Calculated vs Manual Counts {#subsect_0319025034}

You can create an inventory count in two ways:

-   [Creating Calculated Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2298951.html) - Use the NetSuite calculated list of items to create one or more inventory counts that are due.
    
    To use this feature, first define the Next Count Date and your intended Count Interval in days in their appropriate fields on the item record. NetSuite uses these details to calculate when that item needs to be counted.
    
    The Create Inventory Count page shows a list of items that are due to be counted. You can select the items you want to count within a location.
    
    When you view the item record of an item you have completed a count for, the Inventory subtab shows count data, including the last count date and next count date.
    
-   [Creating Manual Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299331.html) - Manually enter inventory counts for items in your location at any time.
    

When you create and start a count, NetSuite takes a snapshot of the on-hand quantity of the items to be counted. After you complete the physical count, you can enter the count data on the Inventory Count page. You can edit and change the count data on a count form multiple times until the count is marked Complete.

A completed count can be reviewed, and then approved or rejected. A rejected count must be counted again. An approved count generates variances to account for any quantity differences between the original snapshot and the final count.

## Processing Transactions During a Count and Recalculating Snapshot Quantities {#subsect_0319025259}

NetSuite compares the results of a count with on-hand quantities from the inventory snapshot. If you continue to process transactions with inventory changes during the time that the counting activities are occurring, you must note these changes. Include these changes when you enter the Count Quantity into the inventory count transaction. Without including quantity changes due to processed transactions, you might encounters issues when approving counts. For more information, see [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html).

Inventory Count provides the **Recalculate Snapshot** preference that enables you to account for updates to on-hand quantities from processed transactions. Without recalculating the inventory snapshot, a mismatch might appear between the snapshot quantity and snapshot details. You cannot approve a count that results to zero or negative inventory. For more information, see [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html).

### Related Topics

-   [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html)
-   [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
