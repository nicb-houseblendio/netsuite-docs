---
id: "section_N2274433"
type: "section"
title: "Setting Up Item Records for Bins"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Setting Up Item Records for Bins"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html"
anchors: ["subsect_0604102234", "subsect_0604101807", "procedure_N2274520"]
sha256: "44271095ada07d43ac9d9e073b5f1aeb9b5fe2ca2c13f3c8944185a67ccb6c16"
---

On each inventory item record that you want to track using bins, you must enable the **Use Bins** setting. You can associate multiple bins with each item and associate multiple items with each bin.

## Adding Bin Numbers on Item Records {#subsect_0604102234}

You can choose a preferred bin when you add bins on the **Bin Numbers** subtab of an item record.

If you use basic Bin Management, you must assign at least one bin number to the item on this subtab. When a bin is associated with an item, it shows in bin lists for that item on transactions.

For example, you use basic Bin Management and enable the **Use Bins** setting for item #AB001. However, you haven't yet associated any bins. When you add item #AB001 to a transaction, no bins show in the bins list for the item. Later, you edit the item record for item #AB001 and associate Bin #20, #21, and #22. When you add item #AB001 to a transaction, you can select Bin #20, #21, or #22 from the list of bins

## Removing Bin Numbers from Item Records {#subsect_0604101807}

If you want to remove bins from the **Bin Numbers** subtab, make sure that they don't have existing quantities. Otherwise, you might see discrepancies between on-hand location quantities and bin quantities. For other information about quantity discrepancies, see [Disabling Use Bins Settings and Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0512092419.html).

#### To set up item records for bins: {#procedure_N2274520}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the name of the item.
    
3.  On the item record, click the **Purchasing/Inventory** subtab.
    
4.  Check the **Use Bins** box.
    
    If you want to disable this setting, see [Disabling Use Bins Settings and Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0512092419.html).
    
5.  On the **Bin Numbers** subtab, do the following:
    
    1.  In the **Bin Number** column, select a bin to associate with this item.
        
        Note:
        
        The Advanced Bin / Numbered Inventory Management feature does not require association of bins with items to use bins on transactions. If you do associate bins and use Multi-Location Inventory, the **Bin Number** field shows a list of available bins based on the selected location. For more information, see [Bin Management by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4713998969.html).
        
        See [Adding Bin Numbers on Item Records](#subsect_0604102234) or [Removing Bin Numbers from Item Records](#subsect_0604101807).
        
    2.  If you want to assign this bin as your preferred one, check the box in the **Preferred (Per Location)** column.
        
        You can set only one preferred bin per location.
        
        On all receiving and fulfilling transactions, as well as the putaway worksheet, NetSuite assigns the preferred bin for the item by default.
        
    3.  Click **Add**.
        
        Repeat this step to associate another bin with this item.
        
6.  Click **Save**.
    

Prior to enabling the Use Bins setting, you may have items with existing inventory transactions or quantities not tracked in bins. You can use the Bin Put-Away Worksheet to assign bins to these items and specify the quantities. For instructions, see [Updating Bin Putaway Worksheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2277819.html).

If you assign bins to components of kit items, see [Updating Kits with Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225728.html).

### Related Topics

-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html)
-   [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html)
-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)
-   [Disabling Use Bins Settings and Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0512092419.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
