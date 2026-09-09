---
id: "section_N2201059"
type: "section"
title: "Creating Cost Categories"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Creating Cost Categories"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html"
anchors: ["procedure_N2201428"]
sha256: "24a1dea2775743f44c2879f47e676092183c80bd2405faddd37f1cdba297b91e"
---

Cost category records are used to classify different types of costs associated with your items. Using cost categories helps you track costs and variances in the manufacturing workflow.

For example, you manufacture widgets to sell to your customers. When you manufacture a widget, you assemble materials made of wood and metal and then paint the widget after it's placed together. For accounting purposes, you want to track the cost of each material and service you use to create each widget. To do so, you can create cost categories that define several kinds of costs you might incur during widget manufacturing.

You might create cost category records such as the following:

-   Material: Metal
    
-   Material: Wood
    
-   Labor: Painting
    

After creating the cost category records, you can then assign a cost category to each item and material you use. Cost category assignment might look like the following:

| Item Name | Description | Cost Category |
| --- | --- | --- |
| Item AB1001 | Wooden Widget Component 1 | Material: Wood |
| Item AB1002 | Wooden Widget Component 2 | Material: Wood |
| Item AB1003 | Metal Widget Component 1 | Material: Metal |
| Service Item XY2002 | Widget Painting | Labor: Painting |

After each item has a cost category specified, it's easier to track total costs for each category. When you process a production run of widgets, you know how much you spent on wooden materials, metal materials, and service labor to produce the widgets you created.

Additionally, when there are variances in production costs for assembly items, the variances can be tracked by cost categories. For example, you process a production run of widgets and the cost for that run is much higher than you expected. You know that a higher cost for the components in the Material: Wood category were the cause of the cost overrun.

Cost categories can be specified on each item record.

The **Cost Category** field is available only for these item types: Inventory, Non-inventory, Service, and Other Charges.

-   Inventory items can have only one material cost category.
    
-   Service items can have only one service cost category.
    
-   Assembly items can have more than one cost category because assembly costs are defined by the component members. NetSuite uses the cost amount and cost category of each component member of an assembly to calculate the assembly's cost and identify the related categories. This calculation process is called a cost rollup for assemblies. For more information, see [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html).
    

When the Standard Cost feature is first enabled, NetSuite automatically creates one cost category. This category is used by default for all new inventory, assembly, and service item records you create. You can add more cost categories as needed.

#### To create a cost category: {#procedure_N2201428}

1.  Go to _Setup > Accounting > Setup Tasks > Accounting Lists > New_.
    
2.  Click **Cost Category**.
    
3.  Enter a name for the category.
    
4.  Select a **Cost Type**.
    
    The Landed option is only available when you enable the Landed Cost feature.
    
5.  In the **Expense Account** field, select the appropriate default expense account to be used as a clearing account for the landed cost of items. Then, after the item is sold, the cost of goods sold is accurately reflected.
    
    This field appears only when you select Landed as your Cost Type. An expense account can't be associated with a material or service type cost category. You don't have to associate a landed cost category with a Cost Of Goods Sold (COGS) account. The landed cost category account is intended as a holding account.
    
    When landed cost is allocated, it posts to two accounts:
    
    -   the asset account of the item
        
    -   the landed cost category account
        
    
    That posting is balanced out by a purchase line, either on the same bill or another purchase transaction, such as a shipping bill. The costing is accounted for in the COGS account of the item after the item is sold.
    
    Important:
    
    If you set the Expand Accounts preference, you can choose any account, including bank accounts or expense accounts.
    
6.  Check the **Inactive** box only if you don't want this category to show in lists.
    
    A cost category can only be inactivated if there are no items associated with that category.
    
7.  Click **Save**.
    
    Now, you can select this cost category on item records and landed costs are included on receiving transactions.
    

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
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
