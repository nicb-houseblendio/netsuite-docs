---
id: "section_N2205923"
type: "section"
title: "Manually Entering an Inventory Cost Revaluation"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Revalue Standard Cost Inventory > Process a Revaluation Transaction > Manually Entering an Inventory Cost Revaluation"
parent: "bridgehead_N2205507"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205923.html"
anchors: ["procedure_N2205993"]
sha256: "7d77567d65858026fa9d0724e5090f9dfda073f28c18d163c1fe1a92d4978578"
---

The Revalue Standard Cost Inventory page lets you activate a standard cost version in production, and recalculate the value of inventory items. For information about inventory revaluation for standard costing items, see [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html).

#### To manually revalue standard cost inventory: {#procedure_N2205993}

1.  Go to _Transactions > Accounting > Revalue Inventory Cost_.
    
2.  Select or enter the **transaction date**. This is the date after which the cost indicated on this page is used for costing calculations.
    
3.  Optionally select a **posting period**.
    
4.  Optionally enter a **reference number**.
    
5.  Select an **adjustment account**.
    
6.  Select the item you want to process for revaluation.
    
7.  Optionally enter a **memo**. Text you enter in this field can be searched to find this transaction.
    
8.  In the **Subsidiary** field, select one or multiple subsidiaries. To select multiple subsidiaries, press and hold the Ctrl key.
    
    This field appears only in NetSuite OneWorld.
    
9.  Select a **department** and **class** if you track them.
    
10.  Select a **location**. The location you choose determines where you can push this version to production and use it for standard costing calculations.
     
11.  Select a **Cost Category**. This category defines how NetSuite tracks cost variances.
     
12.  In the **Cost** field, enter the standard cost for the item to be associated with the selected category. This is the fixed cost you expect to pay for the component on this line.
     
13.  Select a **component**.
     
14.  Enter a **quantity**. This is the number of this component you expect to use in a build.
     
15.  Enter a **unit of measure**.
     
16.  Click **Add**.
     
17.  Repeat these steps for each cost category you need to track for this assembly item.
     
     You can associate multiple cost categories to track costs for assembly items. If you select only one category, the entire standard cost of the item is tracked in that category.
     
18.  Click **Save**.
     

After you submit the page, NetSuite recalculates the inventory value and uses the indicated standard price for transactions from the transaction date. For more information, see [Inventory Cost Revaluation Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3743317066.html).

### Related Topics

-   [Revaluing Standard Cost Inventory in Bulk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2205569.html)
-   [Deleting a Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163275017694.html)
-   [Process a Revaluation Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2205507.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
