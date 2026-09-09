---
id: "section_N2418831"
type: "section"
title: "Entering Landed Cost on a Transaction"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Expenses > Landed Cost > Entering Landed Cost on a Transaction"
parent: "section_N2416930"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418831.html"
anchors: ["procedure_N2418887"]
sha256: "df37f3c03ef908b38c798839d2471daf63b683afa2818242d797b579bbc0928a"
---

To track an expense as a landed cost, you must show the landed cost on an item receipt or vendor bill you enter in NetSuite. On a receipt or bill, use the Landed Costs subtab to identify the allocation method, source, and amount of the landed cost.

Landed cost values may be allocated across eligible items using one of three methods: weight, quantity or value. Eligible items are items on the transaction that have been marked to track landed cost. The allocation method you select depends on the type of landed cost being tracked.

For example, landed cost for freight charges are typically allocated by Weight because vendors often calculate shipping costs based on item weight. However, landed costs for insurance charges are commonly allocated by Value when that is the way the cost of insurance is determined.

Note:

A transaction can only allocate with one method at a time.

To determine the landed cost amounts, you can either enter the expense amount manually for each category or source an existing vendor bill.

For more information, see [Landed Cost Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2419793.html).

The Following below details define landed cost on a per-transaction level. For more information, see [Landed Cost Allocation per Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3728979515.html).

#### To enter landed cost on a transaction: {#procedure_N2418887}

1.  On an item receipt or vendor bill, click the **Landed Cost** subtab.
    
2.  When you enter landed cost on these transactions, the cost can be applied to eligible items by weight, quantity or value. For example:
    
    -   If you track a landed cost for freight charges, you can allocate the freight cost by weight.
        
    -   If you pay insurance for each item in an order, you can allocate the cost of the insurance by value.
        
3.  In the **Cost Allocation Method** field, choose **Weight**, **Quantity**, or **Value**.
    
    | Allocation Method |  | Calculation for Cost Per Eligible Line Item |
    | --- | --- | --- |
    | Weight | Allocated cost per item= | (Weight of Item / Total Weight of Eligible Items) x Total Landed Cost If the item has no weight entered, NetSuite displays an error message |
    | Quantity | Allocated cost per item= | (Total Landed Cost / Number of Eligible Items) \* Line Item Quantity |
    | Value | Allocated cost per item= | (Value of Each Item / Total Value of Eligible Items) \* Total Landed Cost |
    
    Eligible items are the items with the **Track Landed Cost** box checked on their record.
    
4.  Below the **Cost Allocation Method** field, one field shows for each landed cost category that you have created.
    
    For example, if you created a Shipping category, you will see a Shipping field and a Source field.
    
5.  In the **Source** field beside each landed cost category, choose one of the following:
    
    -   **This Transaction** - Make this selection to source items on this transaction to calculate the landed cost amount for this category. The total landed cost amount is the sum of amounts for all items on this bill or receipt associated with this landed cost category.
        
        For example, you enter an item receipt that includes 2 inventory items associated with Duty landed costs and 2 associated with Shipping landed costs. The landed cost amount is the sum of the amounts for the 2 inventory items associated with Shipping landed costs. The Duty items are excluded.
        
        Note:
        
        This option is available only on transactions when you **do not** use the Advanced Receiving feature. If you use Advanced Receiving, the allocation must occur on the inventory receipt transaction.
        
    
    -   **Other Transaction** - Make this selection to source a transaction other than the current one to calculate the landed cost amount for this category. The Transaction field appears to the right.
        
    -   **Other Transaction (exclude tax)** - Make this selection to source a transaction other than the current one excluding taxes. The Transaction field appears to the right.
        
        Note:
        
        When the cost source is based on **Other Transaction (exclude tax)**, the tax calculation depends on whether you use Legacy Tax or SuiteTax.
        
        For more information, see [Landed Cost and Taxation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554390337.html).
        
6.  In the field that appears below the **Source** field, select the transaction that includes the landed cost. Then, the total landed cost amount is the sum of the line items on the sourced bill that are associated with this landed cost category.
    
    Important:
    
    Vendor bills can be sourced to determine landed cost only if the bill includes an item that tracks landed costs. These items appear on the **Items** subtab of the bill. Bills that do not include an item that tracks landed cost do not appear in the Transaction list.
    
    The item on the bill can be one of the following:
    
    -   an inventory item that is set to track landed costs
        
    -   a landed cost item you have created specifically to track landed costs on vendor bills
        
        For more information, see [Creating a Landed Cost Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418506.html).
        
7.  Complete the transaction as necessary.
    
8.  Click **Save**.
    

When the transaction is saved, the landed cost is allocated to the eligible items in the inventory asset account.

### Additional Information

-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)
-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)

### Related Topics

-   [Landed Cost Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417056.html)
-   [Landed Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417902.html)
-   [Landed Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417902.html)
-   [Setting up an Item Record for Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418189.html)
-   [Landed Cost and Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2420792.html)
-   [Estimated Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4576786578.html)
-   [Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2416930.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
