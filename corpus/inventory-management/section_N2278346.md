---
id: "section_N2278346"
type: "section"
title: "Bin Transfers"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Bin Transfers"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html"
anchors: ["bridgehead_N2278439", "bridgehead_N2278666"]
sha256: "962bc6a5cbf562f8e7d6af22794e27ac130551f90b33fb5cdeb094d2e630a2f7"
---

Important:

The functions discussed in this topic may require the Advanced Bin / Numbered Inventory Management feature to be enabled.

You can record a bin transfer to move items between bins within a warehouse or location that uses bins.

For example, at your East Coast location, you stock item #AB123 in two bins: bin #3003 and #4004. There are currently 100 of the item in each bin. You can enter a bin transfer to record the transfer of 50 items out of bin #3003 and into bin #4004.

Recording a bin transfer does not post to your chart of accounts and has no financial impact. The transfer only updates the quantity on hand in each bin for the items transferred.

On the bin transfer record, identify the item, the item's bin, the bin the item will move to, and the quantity to move.

Note:

Bin transfers can move items only if they are already in one or more bins. When you receive incoming items, you can initially assign them to bins. To initially assign existing items to bins, you can use the Bin Put-Away Worksheet. For more information, see [Put Away Items in Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html#bridgehead_N2270434).

If you use the Multiple Units of Measure feature, you can view and edit the **Units** field on bin transfer records. If you select a unit other than stock units, inventory item quantities are converted automatically and saved to item records in stock units.

You can complete the steps in one of the following procedures depending on which bin feature you use:

-   [To record a bin transfer using basic bin management:](#bridgehead_N2278439)
    
-   [To record a bin transfer using advanced bin/numbered inventory management:](#bridgehead_N2278666)
    

If you want to import bin transfers in bulk, see [Bin Transfer Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0319121833.html).

#### To record a bin transfer using basic bin management: {#bridgehead_N2278439}

1.  Go to _Transactions > Inventory > Bin Transfer_.
    
2.  Verify or select the date.
    
3.  If you use the Multi-Location Inventory feature, select a location.
    
    Note:
    
    You can use this form only to transfer items between bins in the same location.
    
    To transfer items between locations, you must enter an inventory transfer and set the bin at the new location. Read [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html).
    
4.  Optionally enter a memo for this transfer. Then, you can search for the text entered here to find this transfer.
    
5.  In the **Item** field, enter or select the item to transfer.
    
    If one is set, the item's preferred bin appears.
    
6.  Optionally, if you use the Multiple Units of Measure feature, select the unit of measure.
    
    By default, this field displays the primary stock unit that you select on the item record.
    
7.  In the **From Bins** field, either enter or select one or more bins the item will be taken out of. This can be done using one of the below:
    
    -   **Enter Text** - Enter a bin and quantity to transfer.
        
        For example, to move a quantity of five out of Bin #101, enter **101 (5)**.
        
    -   **Use the Bin Selector** - Click the **Open** icon to show a list of bins and enter a quantity to take out of each bin. For items that are associated with bins, only associated bins show in the list.
        
        The quantity on hand shows for each bin.
        
        Click **Done** to close the bin selector and add the amounts indicated to the transfer.
        
8.  In the **To Bins** field, either enter or select one or more bins the item will be moved into. This can be done using one of the below:
    
    -   **Enter Text** - Enter a bin and quantity to transfer.
        
        For example, to move a quantity of five into Bin #102, enter **102 (5)**.
        
    -   **Use the Bin Selector** - Click the Open icon to show a list of bins and enter a quantity to put into each bin. For items that are associated with bins, only associated bins show in the list.
        
        The total quantity of items must match the amount in the Quantity field.
        
        Click **Done** to close the bin selector and add the amounts indicated to the transfer.
        
9.  The **Quantity** field sources the amount in the **From Bins** field and displays the quantity of the item being transferred.
    
10.  Click **Add**.
     
11.  Repeat steps 6 to 9 for each item you want to transfer between bins.
     
12.  Click **Save**.
     

#### To record a bin transfer using advanced bin/numbered inventory management: {#bridgehead_N2278666}

1.  Go to _Transactions > Inventory > Bin Transfer_.
    
2.  Verify or select the date.
    
3.  If you use the Multi-Location Inventory feature, select a location.
    
    Note:
    
    You can use this form only to transfer items between bins in the same location.
    
    To transfer items between locations, you must enter an inventory transfer and set the bin at the new location. Read [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html).
    
4.  Optionally enter a memo for this transfer. Then, you can search for the text entered here to find this transfer.
    
5.  In the **Item** field, enter or select the item to transfer.
    
    If a preferred bin is set for the item, it appears.
    
6.  Optionally, if you use the Multiple Units of Measure feature, select the unit of measure.
    
    By default, this field displays the primary stock unit that you select on the item record.
    
7.  Enter the quantity of the item being transferred.
    
8.  Click the **Inventory Detail** button.
    
9.  Complete these steps in the Inventory Detail popup window.
    
    1.  If the item is serial or lot numbered, select the number to transfer.
        
    2.  In the **Bin** field, select a bin the item will be taken out of.
        
    3.  In the **To Bins** field, select a bin the item will be moved into.
        
    4.  Click **Add**.
        
    5.  Repeat the previous four steps for each transfer between bins for this item.
        
    6.  Click **OK**.
        
10.  On the Bin Transfer line, click **Add**.
     
11.  Repeat steps 5 - 9 for each item you want to transfer.
     
12.  Click **Save**.
     

### Related Topics

-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html)
-   [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html)
-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
