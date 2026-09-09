---
id: "section_N2201836"
type: "section"
title: "Setting Up Item Records for Standard Costing"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Setting Up Item Records for Standard Costing"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html"
anchors: ["procedure_N2201860", "bridgehead_1547757295"]
sha256: "ef27cbf0cf368c2d50b5352d884f694c122d534fab5d96e40194b0624b1c01d1"
---

To use standard costing for an item, set up the item record.

#### To set up an item record for standard costing: {#procedure_N2201860}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the item record.
    
3.  On the **Purchasing/Inventory** subtab, select the **Standard** costing method.
    
    Note:
    
    The costing method can't be changed after you save the item record.
    
4.  Set the **Cost Category**.
    
    Cost categories you've created appear in the list.
    
    For more information about cost categories, see [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html).
    
5.  Enter a **Default Cost** . You can enter a cost per location. The value in this field can be used as the default when you create a planned standard cost record.
    
    To streamline data entry for setting up standard costs, you can also import values into this field using CSV import.
    
6.  In the **Purchase Price Variance Account** field, choose the account to post a variance to when a purchase transaction calculates a cost variance.
    
7.  In the **Gain/Loss Account** field, choose the account to post a variance to when an inventory transfer calculates a cost variance.
    
8.  On assembly item records, complete the following:
    
    1.  In the **Production Quantity Variance Account** field, choose the account to post a variance to. The variance posts when the assembly cost is higher or lower than expected due to the number of items used in the assembly build.
        
        For example, a variance is created if a build costs more because you use 10 widgets when you normally use 8.
        
    2.  In the **Production Price Variance Account** field, choose the account to post a variance to. The variance posts when the assembly cost is higher or lower than expected due to the expense of items used in the assembly build.
        
        For example, a variance is created if a build costs more because you use widgets that cost $30 each when you normally pay $20.
        
    3.  In the **Unbuild Variance Account** field, choose the account to post a variance to when an unbuild transaction calculates a cost variance.
        
        These fields appear only on assembly item records.
        
9.  Complete additional fields as necessary.
    
10.  Click **Save**.
     

## Deletion of Standard Cost Item {#bridgehead_1547757295}

You'll see a warning message when you try to delete an item that has a standard cost, either active or historical. This helps preserve the integrity of the data used to evaluate items' inventory costs. For example, this happens when the unit cost of an item is found in inventory revaluation transactions and not on item records. Before you can delete such an item, you should first delete the standard cost on the inventory revaluation transaction. The warning message displayed includes a link to the revaluation transaction that includes the standard cost.

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html)
-   [Entering Planned Standard Cost Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html)
-   [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html)
-   [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html)
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
