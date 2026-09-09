---
id: "section_N2288536"
type: "section"
title: "Setting Up Demand Planning"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Demand Planning > Setting Up Demand Planning"
parent: "section_N2286970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html"
anchors: ["subsect_0811062111", "bridgehead_N2288606", "bridgehead_N2288707"]
sha256: "ea679e1ba6dcbf5eca50864654e473fa3e9d1ec9a1b26eb2bb1d7750a504af17"
---

To create demand plans and supply plans for items using demand planning, follow these steps:

1.  [Enabling Features for Demand Planning](#subsect_0811062111)
    
2.  [Set Inventory Preferences](#bridgehead_N2288707)
    
3.  Set up [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html)
    

## Enabling Features for Demand Planning {#subsect_0811062111}

To create plans, you need to first turn on the demand planning features.

#### To enable demand planning features: {#bridgehead_N2288606}

1.  Go to _Setup > Company > Enable Features_.
    
2.  On the **Items & Inventory** subtab, check **Demand Planning** box.
    
    Note:
    
    Ensure Advanced Inventory Management is enabled.
    
3.  To use demand planning for assembly items, ensure Work Order feature is enabled. Check **Work Orders**.
    
4.  Click **Save**.
    

## Set Inventory Preferences {#bridgehead_N2288707}

You can set preferences that affect affect how Demand Planning works:

-   **Transactions to Consider**
    
    On the Inventory Management Preferences page, choose a setting for Transactions to Consider. This setting controls which transactions are included in demand planning calculations.
    
    -   Select the **Orders** setting to use approved, non-canceled sales orders to calculate demand. If the feature is enabled, then Work Orders are also included.
        
    -   Select the **Actual Sales** setting to use only cash sales and invoices in demand calculations. Sales orders aren't used to calculate demand. If the Assemblies feature is enabled, then Assembly builds are also included.
        
    
    Inventory demand calculations consider only transactions that decrease an item's stock level. For example, an assembly build increases the stock level for the assembly item but decreases the stock level for the assembly item's components. The demand plan calculation counts the assembly build only for the assembly item's components, not for the assembly item itself.
    
    Note:
    
    If you use both sales orders and standalone cash sales or invoices, select the **Actual Sales** option.
    
    To set this preference, go to _Setup > Accounting > Inventory Management Preferences_.
    
    For detailed steps on setting up this preference, see [Setting Up Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2285514.html).
    
-   **Allow Purchase of Assembly Items**
    
    Use this preference to let NetSuite create purchase orders instead of work orders for assemblies. You can also set purchase pricing on assembly item records.
    
    This preference also lets you add assembly items to purchase orders, vendor bills, checks, credit card transactions, and vendor credits.
    
    To set inventory preferences, go to _Setup > Accounting > Accounting Preferences_.
    
-   Click the **Order Management** subtab.
    
-   **Demand Planning and Allocation**
    
    If you use the Demand Planning feature, consider using automated allocation as well. For more information, see [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html).
    
-   **Demand Planning and Routing**
    
    If you use the Manufacturing Routing and Work Center feature, see [Setting Routing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950900044.html).
    
-   **Demand Time Fence**
    
    Enter the number of days (0-365). This number is the default demand time fence, and it appears in the Demand Time Fence field on new item records. If needed, you can change this number when you create each item record. The default is zero.
    
-   **Planning Time Fence**
    
    Enter the number of days (0 - 365). This number is the default demand time fence, and it appears in the Planning Time Fence field on new item records. If needed, you can change this default number when you create each item record. The default is zero.
    

### Related Topics

-   [Calculating Item Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html)
-   [Monitoring the Demand Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291615.html)
-   [Viewing, Editing, and Deleting a Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291961.html)
-   [Manually Entering an Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2292418.html)
-   [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html)
-   [Monitoring the Supply Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293790.html)
-   [Viewing, Editing, and Deleting a Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294140.html)
-   [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html)
-   [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html)
-   [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html)
-   [Distribution and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296427.html)
-   [Time Fences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3848058018.html)
-   [Planning Action Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3865354301.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
