---
id: "section_N2194190"
type: "section"
title: "Inventory Costing and Assembly Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Inventory Costing and Assembly Items"
parent: "chapter_N2191369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194190.html"
anchors: ["bridgehead_N2194214", "bridgehead_N2194271"]
sha256: "8eac971f2af10d1a044f675e5d3063882def741566e28e5d87a2382c0c247ec0"
---

After you build an assembly item, NetSuite treats it like an inventory item for costing purposes. The asset or inventory cost of each built assembly item is the total value of the assembly's member items.

These values act like the assembly item's purchase price for inventory costing calculations. NetSuite tracks inventory costing for the assembly item based on the inventory costing method you select on the item record. For more information about assemblies and component costing, see [System Cost of Goods Sold Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html).

## Inventory Costing Using the Standard Costing Feature {#bridgehead_N2194214}

For information about inventory costing calculations when you enable the Standard Costing feature, see [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html) and [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html).

## Inventory Costing and Serialized Assemblies Without Standard Costing {#bridgehead_N2194271}

If the cost of a serialized component in an assembly is unknown, NetSuite uses the historical average cost for the component item when you unbuild the assembly and return it to stock. The total cost of unbuilt items might not match the total purchase cost of the assembly.

For example, you have a serialized assembly in stock that costs $12, which is composed of a single serialized component and has a current historical average cost of $15. When you unbuild the assembly, the accounting posts as follows:

-   Asset account of assembly: -$15
    
-   Asset account of component: +$15
    
-   Asset account of assembly: +$3
    
-   COGS account of assembly: -$3
    

You now have the component in stock at a value of $15. The $3 difference between the assembly value and the unbuilt component value is pulled out of the COGS account of the assembly. It then posts back to its asset account. The total amount reduced from the assembly's asset account to create the component is $12, or the value of the assembly.

### Related Topics

-   [Setting Inventory Costing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html)
-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html)
-   [Selecting a Default Cost of Goods Sold (COGS) Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2192814.html)
-   [LIFO/FIFO Inventory Costing and Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html)
-   [Viewing Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197076.html)
-   [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)
-   [Troubleshoot Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4447393386.html)
-   [Cost Accounting Status on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199228.html)
-   [Item Return Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html)
-   [Group Average Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
