---
id: "section_N2273755"
type: "section"
title: "Setting Bin Preferences"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Setting Bin Preferences"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html"
anchors: []
sha256: "35a339e4cc36280a91291c226508e234f3ef58ccc849bd3caef86459821e13b5"
---

You can set the following preferences available for basic and advanced Bin Management:

-   Require Bins on All Transactions Except Item Receipts
    
-   Use Preferred Bin on Item Receipts
    

#### To set bin preferences:

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **Items/Transactions** subtab.
    
3.  Choose one of the following for the **Use Preferred Bin on Item Receipts** preference:
    
    -   When you enable this preference, the **Bin** field on item receipts defaults to the preferred bin instead of leaving the field blank.
        
    -   Disable this preference if you prefer the **Bin** field to remain blank by default.
        
4.  Choose one of the following for the **Require Bins on All Transactions Except Item Receipts** preference:
    
    -   With this preference enabled, transactions that change inventory levels and include binned items must have a bin selected to save the transaction. If there is no bin field on a transaction, such as sales orders and purchase orders, bins are not required.
        
        Editing a previously existing sale transaction that has a bin item but no specified bin require bin specification on the transaction.
        
        Item Receipts do not require a bin selection with this preference enabled.
        
    -   Disable this preference to allow transactions to be created that include items with no bin selected.
        
        Note:
        
        With this preference disabled, NetSuite always requires bins on transactions where an item quantity is reduced. For example, on cash sales, item fulfillments, or negative inventory adjustments.
        
        Bins are not required on transactions where an item quantity is increased, such as purchases and positive inventory adjustments.
        
        For example, cash sales with bin items that specify locations requires the items to have at least one bin in that location. Also, when you enter an inventory adjustment, any line that deducts a quantity of an item that uses bins will require a bin.
        
5.  Click **Save**.
    

### Related Topics

-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html)
-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
