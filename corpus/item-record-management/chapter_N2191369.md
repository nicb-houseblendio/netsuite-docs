---
id: "chapter_N2191369"
type: "chapter"
title: "Item Costing"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing"
parent: "book_N2164398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html"
anchors: ["bridgehead_N2191486", "bridgehead_N2191502", "subsect_0707085636", "bridgehead_1499433467", "bridgehead_N2191545", "procedure_N2191564"]
sha256: "bcbebf6da8744084ad523b856617fead4a50a0d74e23ef294bed3a3657d52a73"
---

If you use both the Accounting and Inventory features, you need to track the total value of your assets and to calculate profits you make. You can set up your NetSuite account to track inventory costing, which are the costs associated with goods and services you sell.

Each time you buy and sell inventory items, you need to track the cost of your items throughout the purchase and sale processes. The cost of an item you buy or sell affects your general ledger accounts.

## Cost of Goods Sold (COGS) and the General Ledger {#bridgehead_N2191486}

A Cost of Goods Sold (COGS) account isn't an expense account, but it works like one. To calculate your company's gross profit, subtract the inventory costing total from the income total before expenses.

The cost of an item is associated with income and expenses (overhead) and aren't directly tied with the sale of an item.

## Item Cost {#bridgehead_N2191502}

Item cost comes from the price of the item on the purchase order.

When you determine the cost of an item, account for costs associated with buying the same items at different purchase prices over time. For example, sometimes you pay your vendor $10 for each calculator, and other times it's $15. You can choose a costing method to decide how NetSuite handles these variances.

The exact cost assigned to an item depends on the costing method you choose. For more information, see [Setting a Default Inventory Costing Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703007.html) and [System Cost of Goods Sold Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html).

## Initial Average Cost {#subsect_0707085636}

If you use the Multi-location Inventory feature, on item records, you can set the initial average cost when no transactional cost exists yet. For instructions and guidelines, see [Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504284372.html#bridgehead_1504292539).

If you use the Costed Bill of Materials SuiteApp, the initial average cost of component items included in a costed BOM applies only if the material cost is set to **Per Costing Method**. On the **Material Costs** subtab, it appears in the **Unit Cost** column for each component item. The initial average cost is used when calculating estimated assembly costs if no transactional cost exists. For requirements and more information, see [Costed Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160730538.html) or [Per Costing Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0614024050.html).

By default, the first transaction created for the item applies the initial average cost that you specify. However, if the first transaction results to underwater inventory, zero is used for the actual cost instead. Your initial cost applies to the estimated cost only.

## Inventory Costing Preferences {#bridgehead_1499433467}

You can select your preferences for handling inventory costing. For more information, see [Setting Inventory Costing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html).

## Costing and Verifying Decimal Precision {#bridgehead_N2191545}

NetSuite calculates and reports inventory costs using decimal precision that's based on your chosen currency's format.

The decimal precision shown in the **Format** field of a currency record is used for inventory costing calculations and can't be changed. This keeps your inventory costing and reporting consistent.

For example, you selected USD (United States Dollar) as the currency for an item on the item record and the format is USD. The decimal precision for that item's costing and reporting is two decimal places.

Note:

Standard Costing is an exception. NetSuite calculates Standard Costing with decimal precision to seven places. For example, 9.87654321 is calculated as 9.8765432. For more information, see [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html).

#### To verify the decimal precision for a currency: {#procedure_N2191564}

1.  Go to _Lists > Accounting > Currencies_.
    
2.  Click the name of the currency.
    
    The selected format shows in the **Format** field.
    
    The decimal precision for that format shows in the **Format Sample** field.
    

### Related Topics

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
-   [Inventory Cost Accounting Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0420024853.html)
-   [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html)
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)
-   [Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2211898.html)
-   [Bar Codes and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)
-   [Customer Part Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4575965810.html)
-   [Effective Date Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1536354469.html)
-   [Item Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2164398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
