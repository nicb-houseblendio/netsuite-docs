---
id: "section_N2297481"
type: "section"
title: "Setting Up Item Records for Inventory Count"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Count > Setting Up Item Records for Inventory Count"
parent: "section_N2296970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297481.html"
anchors: ["procedure_N2297500"]
sha256: "d54f39a3eed8e0b1e44a1a484bdaa0ad8707c90329be51e84fbc8aa2f29ce83a"
---

If you want NetSuite to calculate inventory count information for an item, you need to set up the item record to do so.

You can use the Import Assistant to create new item records or update existing ones for the inventory count fields. See [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html) or [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html).

#### To set up an item record for inventory count: {#procedure_N2297500}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the name of an inventory or assembly item.
    
3.  On the item record, click the **Purchasing/Inventory** subtab.
    
4.  On the **Purchasing/Inventory** subtab, click the **Locations** subtab.
    
5.  Enter or select values in the following inventory count fields:
    
    Tip:
    
    If you use the Multi-Location Inventory feature, you can fill out these fields for each location.
    
    -   In the **Next Count Date** field, enter the date of the next planned inventory count for this item.
        
        NetSuite uses this date to determine and calculate when a count is required.
        
    -   In the **Count Interval** field, enter the total number of days between required counts.
        
        For example, if you enter **30**, NetSuite calculates the date a count is required based on 30 day intervals.
        
    -   (Optional) In the **Classification** field, select the inventory classification.
        
        You can sort the list to create inventory counts based on classifications you select in this field.
        
6.  Click **Save**.
    

After the count date and interval are recorded for an item, NetSuite uses them to calculate when a count is required. When a new count is due to be recorded, it shows in the list on the Create Inventory Count page.

### Related Topics

-   [Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296970.html)
-   [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html)
-   [Creating Calculated Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2298951.html)
-   [Creating Manual Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299331.html)
-   [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
