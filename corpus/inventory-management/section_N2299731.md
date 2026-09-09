---
id: "section_N2299731"
type: "section"
title: "Working with an Inventory Count"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Count > Working with an Inventory Count"
parent: "section_N2296970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html"
anchors: ["procedure_N2299784", "procedure_N2299861", "procedure_N2299945", "procedure_N2300072", "bridgehead_N2300173"]
sha256: "faff8c84d8856c798a9c55fcc469c62ba78d7411b79f538529b8034b5e2ef4bf"
---

After an inventory count is recorded, you must complete these steps:

1.  Start the count to begin the process of recording count data.
    
2.  Edit the count record to enter count numbers for items.
    
3.  Complete the count to record the final number counted for each item on the count.
    
4.  Approve or reject the final count.
    

#### To start an inventory count: {#procedure_N2299784}

1.  Go to _Transactions > Inventory > Enter Inventory Count > List_.
    
2.  Click **View** next to the count you want to start.
    
3.  Click **Start Count**.
    
    When you click **Start** on an Open status inventory count, NetSuite takes a snapshot of the on-hand count of the items to be counted by bin and serial number. This data is recorded on the count.
    
    An inventory count with a status of Started can be reviewed and edited by the warehouse manager. Data in quantity fields can be edited, but items cannot be added to or deleted from the count.
    

#### To edit the count record: {#procedure_N2299861}

1.  Go to _Transactions > Inventory > Enter Inventory Count > List_.
    
2.  Click **Edit** next to the count you want to work with.
    
3.  Based on the physical count numbers taken in your warehouse, record the number counted in the **Count Quantity** field.
    
    Note:
    
    When the inventory count transaction status is set to **Started**, a snapshot of the inventory on hand quantity is taken from the system for comparison. If you continue to process inventory changes during the time that the counting activities are occurring, record the changes and include them when you enter the **Count Quantity** into the inventory count transaction.
    
4.  In the **Unit** field, select the item's unit that you want to count.
    
5.  For lot items, serialized items, or items with inventory statuses, in the **Count Detail** column, click the inventory detail icon to open its popup window. On this popup window, you can enter the quantity for each lot, serial number, or inventory status.
    
6.  Click **OK**.
    
    To enter your count for another item, repeat from step 3.
    
7.  After entering data on a started count, click **Save** to return and complete the count later.
    

#### To complete an inventory count: {#procedure_N2299945}

1.  Go to _Transactions > Inventory > Enter Inventory Count > List_.
    
2.  Click **View** next to the count you want to complete.
    
3.  Click **Complete Count**.
    
    Until an inventory count is completed, you cannot start a new inventory count for that item.
    

After a count transitions to the Completed/Pending Approval status, a supervisor can approve or reject it.

#### To approve or reject an inventory count: {#procedure_N2300072}

1.  Go to _Transactions > Inventory > Enter Inventory Count > List_.
    
2.  Click **View** next to the count you want to complete.
    
3.  On the Inventory Count page, you can review the count results on the **Items** subtab. In view mode, aside from the count quantity, you can review the following details:
    
    Tip:
    
    Review these details to make sure that the inventory count does not result to zero or negative inventory.
    
    -   **Snapshot Detail** - Click **View** to check the breakdown of the snapshot quantity based on applicable inventory details.
        
    -   **Adjusted Quantity** - The total quantity of the adjustment calculated from the snapshot and count quantities.
        
    -   **Variance Detail** - Click **View** to check the breakdown of the adjusted quantity based on applicable inventory details.
        
4.  Do one of the following:
    
    Tip:
    
    You cannot edit quantities or results of a count in Completed/Pending Approval status.
    
    -   Click **Reject** - The count status returns to Started and the warehouse manager must conduct another count.
        
    -   Click **Approve** - The count is final and the status becomes Approved.
        
    
    If you process transactions during counts, they may increase or decrease on-hand quantities and result to variances with counted quantities. Without reflecting updated quantities from transactions, the count cannot be approved if it results to zero or negative inventory. You can set the **Recalculate Snapshot** preference to include transaction updates to on-hand quantity snapshots. When you reject a count, NetSuite takes a new inventory snapshot and updates the snapshot, adjustment quantity, and variance details accordingly. These automatic updates enable you to approve the rejected count. Otherwise, you can re-create a count based on the transaction updates before you can approve it. To set this preference, see [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html).
    

Two inventory adjustment transactions may be created for the count:

-   One positive inventory adjustment to increase the on-hand quantity
    
-   One negative adjustment to decrease the on-hand quantity
    

When you return to the item record of an item you have completed a count for, the Inventory subtab shows the following:

-   Last Count Date - Date when the last count occurred
    
-   Next Count Date - System calculated next date to enter an item count
    
-   Count Interval - Preset count interval
    

## Inventory Count History {#bridgehead_N2300173}

After Approval, the Inventory Count record shows a History subtab that includes an Inventory Adjustments subtab which shows all adjustments related to this count.

### Related Topics

-   [Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296970.html)
-   [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html)
-   [Creating Calculated Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2298951.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
