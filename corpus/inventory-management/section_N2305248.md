---
id: "section_N2305248"
type: "section"
title: "Manual Inventory Distribution"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Management Setup > Distributing Inventory > Manual Inventory Distribution"
parent: "section_N2304534"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305248.html"
anchors: ["procedure_N2305347"]
sha256: "4d760c2ae6cd76c77698271525ec6901cb950eb568c2ee5216d33035aa719993"
---

A Manual Inventory Distribution enables you to enter specific details to distribute particular items and amounts to specific locations. This method requires more time than the Simple Distribution method, which means more time before you can enter inventory transactions. For more information, read [Simple Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304987.html).

Using the Manual method is ideal if you want to specify quantities for each location before inventory transactions are entered for individual locations.

You can alternatively choose to enter a Simple Inventory Distribution. For more information, read [Simple Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304987.html).

Warning:

You should not delete or change inventory transactions dated prior to an inventory distribution, as this can cause difficulties maintaining accurate inventory data.

#### To enter a Manual Inventory Distribution: {#procedure_N2305347}

1.  Go to _Transactions > Inventory > Distribute Inventory_.
    
2.  Click **Manual**.
    
3.  The **Date** field autofills with the current date. You can select or enter another date.
    
    If you postdate this distribution transaction, be sure that the date you choose is after the date of any other postdated inventory transactions, especially transactions not associated with locations.
    
4.  Choose a posting period for this transaction.
    
    Note:
    
    You cannot post to a closed accounting period.
    
5.  In the **Ref. No.** field, enter information to identify this distribution in a list of other transactions. If you have enabled auto-generated numbering, this field autofills with a value.
    
6.  In the **Variance Account** field, select an account for this distribution.
    
    Usually, an expense account is assigned for inventory distribution.
    
7.  Select a **Department** or **Class** if you track them.
    
8.  In the **Memo** field, enter a memo to identify this inventory distribution.
    
    If you use the Search Transactions feature, you can search for specific words and phrases in the **Memo** field.
    
9.  The table at the bottom of the page shows the following information about undistributed items.
    
    -   The **Item** column shows all items in your initial inventory, 50 items at a time.
        
    -   The **Total Stock** column shows the stock count for each item in your initial inventory.
        
    -   There is a column for each of your company location records with a data-entry field beneath it.
        
10.  In the field beneath each location, enter the quantity you want to allocate to that location.
     
     For each item, if the total of quantities entered for all locations is not equal to the number in the **Total Stock** column, the variance quantity appears in the **Variance** column.
     
     The variance amount for each item appears in the **Variance Amount** column.
     
     The total variance of your inventory distribution appears in the **Total Variance Amount** field at the top of the page.
     
11.  If you are distributing lot-numbered items or serialized items, enter these numbers in the **Serial/Lot Numbers** field.
     
     -   Separate each serial number with a space, comma or by pressing Enter after each one.
         
         You must enter a serial number for each of the quantity on hand that you enter. For example, if you enter a quantity on hand of 2, then you must enter two serial numbers.
         
     -   Lot numbers must be entered in this format: **LOT#(Quantity)**
         
         For example, to enter a quantity of 100 items as Lot number ABC1234, enter **ABC1234(100)** in the **Lot Numbers** column.
         
12.  Click **Save**.
     

For any items with an undistributed stock quantity, you can distribute inventory again at a later time.

Note:

These Distribute Inventory changes are permanent. Your stock counts entered as of the date specified are not changed as of that point, even if you enter transactions with dates prior to the worksheet date.

For example, you can enter an inventory distribution dated 10-25-08 and allocate 10 of item number UNV21200 to Location One. You then create an invoice dated 10-24-08 which sells two of item UNV21200 from Location One. The quantity of the item at Location One on 10-25-08 remains at 10 as determined by the inventory distribution.

After you have distributed an item, if you enter a transaction that is dated before the distribution and includes the distributed item, the transaction will not have location impact. This is true even if you choose a location on the transaction.

From the previous example, the UNV21200 items sold on the invoice created on 10-24-08 would not be able to be tracked by location, because the invoice date is prior to the distribution date of that item on 10-25-08.

### Related Topics

-   [Multi-Location Inventory Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html#bridgehead_162032472912)
-   [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html)
-   [Simple Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304987.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
