---
id: "section_N2335987"
type: "section"
title: "Setting Up Items as WIP Assemblies"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > Setting Up Items as WIP Assemblies"
parent: "chapter_N2335392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html"
anchors: ["procedure_N2336006"]
sha256: "24ce1f3a24cbccbdf63a8dbde330e840c1e1933ee027cbd8efd16c68d8239622"
---

After your administrator enables the Manufacturing Work In Process (WIP) feature, you can set up assembly items to use WIP.

#### To set up an assembly item to use WIP: {#procedure_N2336006}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the existing assembly item record.
    
    Alternatively, click **New** to enter a new assembly record.
    
    Only items that use standard or average costing can be used on a WIP work order.
    
3.  On the **Basic** subtab, make a selection for the following accounts:
    
    1.  **WIP Cost Variance Account** - The expense account for actual cost or average cost assemblies. This is used when the reconciliation amount cannot be returned to the asset account because the amount has been shipped. This account is required when WIP is checked for any location.
        
    2.  **Scrap Account** - The expense account for scrap that occurs during work order completion. This account is required if WIP is checked for any location.
        
    3.  **WIP Account** - The asset account used when a work order component issue is entered. This account is required if WIP is checked for any location.
        
    
    Note:
    
    If you change the selected WIP account, the new WIP account affects only future transactions. Existing transactions continue to show the WIP account when the transaction was created.
    
4.  To create a new assembly, complete assembly item form fields. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
5.  Click **Save**.
    

When the assembly is added to a work order, you can use WIP to process the assembly.

Work orders that are only partially completed don't account for unused WIP components. They are moved into the cost of the finish goods account, even if they haven't been used.

### Related Topics

-   [Enabling the WIP Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335702.html)
-   [Setting Default WIP Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607056275.html)
-   [Using WIP on Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html)
-   [Associating Components with Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4165324435.html)
-   [Entering a Completion for an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339540.html)
-   [WIP and Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340709.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
