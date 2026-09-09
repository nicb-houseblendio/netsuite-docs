---
id: "section_N2199328"
type: "section"
title: "Item Return Costing"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Item Return Costing"
parent: "chapter_N2191369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html"
anchors: ["bridgehead_N2199407", "procedure_N2199431"]
sha256: "385da438539bd573afbaf5fdb7a510436230d044db81e54cc516fc100e43d432"
---

When a customer returns an item, NetSuite needs to account for that item in the books by assigning it a return cost. You can do this in two ways:

-   **Calculated Costing** - If you use calculated costing, you allow NetSuite to calculate the return cost of the item. If you allow the return cost to be calculated, it might not be the same cost every time.
    
-   **Fixed Costing** - If you use fixed costing, you assign a fixed return cost for an item. This cost is always used when the item is returned and overrides any calculated cost.
    
    You can set a default cost to use when an item is returned. This provides an alternative method to relying on NetSuite calculations to set the return cost, which might be a varying amount.
    

Use one of the following methods to set a fixed return cost for an item:

-   [Fixed Return Cost on Item Records](#bridgehead_N2199407)
    
-   [Customizing Return Receipts](#procedure_N2199431)
    

## Fixed Return Cost on Item Records {#bridgehead_N2199407}

Inventory item and assembly item records show the field **Default Return Cost**. In this field, enter the rate you want to default to show as the cost for this item when it's returned. The value you enter automatically appears in the **Override Rate** field on item receipts. You can change this value after it appears on the item receipt.

-   If you use Multiple Units of Measure, this rate is always based on the stock unit.
    
-   If you use Multi-Location Inventory, this field appears on the **Inventory** subtab of item records in the location list without being customized.
    
-   If you don't use the Multi-Location Inventory feature, this field is hidden by default. You need to customize the item record to display the field.
    

## Customizing Return Receipts {#procedure_N2199431}

You can customize return receipts forms to display the fields **Override Rate** and **Override Rate Currency**.

#### To customize return receipts:

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  Next to **Item Receipt**, click **Customize**.
    
3.  In the **Screen Fields** subtab, click the **Columns** subtab.
    
4.  Check the **Override Rate** box.
    
5.  Click **Save**.
    

When you use the custom receipt page, you'll see these fields:

-   **Override Rate** - This field defaults to show the value entered on item records. If the item being returned doesn't have a value in this field, it shows up blank. You can enter a value as needed.
    
    If you use Multiple Units of Measure, the rate in this field is based on the units on the originating transaction.
    
-   **Override Rate Currency** - This field always shows the base currency.
    
    This field shows only if you use the Multi-Currency feature.
    

If you use Multi-Location Inventory, when you select a location on the receipt, the rate and currency from the item record appear in these fields. For more information, see [Returned-Item Costing Using Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2307937.html).

If you leave the **Override Rate** field blank on the item receipt, NetSuite calculates the cost of the returned item.

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
-   [Group Average Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
