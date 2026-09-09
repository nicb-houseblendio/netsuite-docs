---
id: "section_N2297156"
type: "section"
title: "Setting Up Inventory Count"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Count > Setting Up Inventory Count"
parent: "section_N2296970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html"
anchors: ["procedure_N2297247", "procedure_N2297325"]
sha256: "cb66e770b8c3d396313f4393cc4a921a659044721a9f332d8c6372dc0a95b6a8"
---

To use the inventory count feature complete the following procedures:

-   [To enable inventory count:](#procedure_N2297247)
    
-   [To set up preferences:](#procedure_N2297325)
    
-   [Setting Up Item Records for Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297481.html)
    

#### To enable inventory count: {#procedure_N2297247}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Items & Inventory** subtab.
    
3.  Check the **Inventory Count** box.
    
4.  If you want to count lot and serialized items, check the **Advanced Bin/Numbered Inventory Management** box.
    
5.  Click **Save**.
    

#### To set up preferences: {#procedure_N2297325}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  On the **Items/Transactions** subtab, you can enable the following inventory count preferences:
    
    Note:
    
    You can enable the Show Display Name with Item Codes preference to view both the item name and display name of an item on inventory count records. To set this preference in your account, go to _Setup > Company > General Preferences_. For more information, see [Setting General Account Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N243797.html).
    
    -   **Default Inventory Count Account** - Select the default account to which you want to post inventory count variances to. It is typically an expense account.
        
        When you create inventory counts, the **Account** field automatically shows your selected default account.
        
    -   **Recalculate Snapshot on Inventory Count Reject** - Check this box if you want to automatically take a new snapshot of item quantities when you reject a count.
        
        If you process transactions during inventory counts, this preference enables you to include transaction updates to on-hand quantities. When you reject a count, NetSuite updates the snapshot, adjustment quantity, and variance details based on the new snapshot. For more information, see [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html).
        
    -   **Display Current Count on Adjustments** - If you tend to create counts with a large number of item lines, you can set this preference to prevent slowness that may occur when adjustments are generated. For more information, see [Entering an Inventory Adjustment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161981111273.html) or [Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html#bridgehead_N1387462).
        
3.  Click **Save**.
    

### Related Topics

-   [Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296970.html)
-   [Creating Calculated Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2298951.html)
-   [Creating Manual Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299331.html)
-   [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
