---
id: "section_N2234538"
type: "section"
title: "Building a Serialized Assembly"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Serial Numbered Items > Building a Serialized Assembly"
parent: "section_N2230290"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234538.html"
anchors: ["procedure_N2234642"]
sha256: "a2093f6a29d939bc8263a23d3693bb083c09634eb6f562dfa931f9b7ce799a1b"
---

Serialized assembly items enable you to build items from raw materials and track the inventory of both the finished items and the raw materials separately. The completed assembly is assigned a serial number to track it as it enters and leaves your inventory.

The serial number lets you access the history of any serialized assembly item. The history lets you track the cost of the assembly or check its status. You can also choose a specific serial numbered assembly item to fulfill an order.

Only inventory items can be members of an assembly.

Serialized assembly items are available on sales transactions and inventory adjustment transactions. They are not available on purchase transactions.

Build assemblies in NetSuite from inventory items to increase your stock of those assembly items.

You must create serialized assembly item records before you can build serialized assemblies in NetSuite. To create a new assembly item record, go to _Lists > Accounting > Items > New_. Under Assembly/Bill of Materials, click Serialized.

#### To build serialized assembly items: {#procedure_N2234642}

1.  Go to _Transactions > Inventory > Build Assemblies_.
    
2.  In the **Reference #** field, enter a reference number to track this assembly.
    
3.  Select the serialized assembly item you want to build from the **Assembly** list.
    
    After selecting an assembly item, the **Buildable Quantity** field displays the maximum number that you can build.
    
4.  In the **Quantity to Build** field, enter the number of assembly items you want to build.
    
    -   You can't enter a quantity that exceeds the number in the Buildable field.
        
    -   If you use locations, the quantity that appears in the Buildable field is for the selected location.
        
    -   The **Projected Value** field displays the projected value of your new assemblies.
        
        Projected value is the sum of the value of the member items times the quantity entered.
        
5.  In the **Serial Numbers** field, enter the serial number or numbers for this assembly.
    
    1.  To choose multiple serial numbered items on transactions, click the **Select Multiple** link next to the **Serial/Lot Numbers** field.
        
    2.  In the popup window, click an item from the left pane to add it to the right pane list.
        
    3.  Click **Done** to add the selected items to the transaction.
        
    
    The preferred assembly item record bin number is displayed in the **Bin Numbers** field.
    
6.  If assembly items from this build are stored in other bins, click the Bins icon.
    
    Bins must be selected on the assembly item record to be displayed here.
    
7.  In the popup window, edit the quantity for each bin, and then click **Done**.
    
8.  In the **Date** field, accept today's date or enter another date.
    
9.  If you use accounting periods, select a **Posting Period** for this assembly.
    
10.  Optionally, in the **Memo** field, enter any information you want to display on a register or account detail report. You can also search for this text to find this record later.
     
11.  In the Classification section, do the following:
     
     1.  Select a department and **Class**, if needed.
         
     2.  Select a **Location** for the built assembly items.
         
         Raw materials are taken from the inventory at this location. The built assembly items are added to the inventory at this location.
         
         To create a new location, select **New** from the list.
         
         To view the list of existing locations, go to Setup > Company > Locations.
         
12.  If the assembly contains serialized inventory items, enter or select the serial number for each serialized member item.
     
     Separate each serial number with a space or comma, or press Enter after each number. You must enter a serial number for each serialized item. For example, if you enter a quantity of 2, then you must enter two serial numbers.
     
13.  Click **Save**.
     

After a serialized assembly item has been built, it is treated like an inventory item for inventory costing purposes. The asset/costing value of a serialized assembly item is the sum of the values of the assembly's member items. This total value functions as the serialized assembly item's purchase price for inventory costing calculations.

### Related Topics

-   [Enabling Serial Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230646.html)
-   [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html)
-   [Track Serialized Inventory on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231339.html)
-   [Add New Serial Numbers to Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231739.html)
-   [Searching for Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508171622.html)
-   [Receiving a Purchase Order With a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233116.html)
-   [Serialized Items on Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233510.html)
-   [Fulfilling a Sales Order with a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233933.html)
-   [Memorizing Transactions with Serialized Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234305.html)
-   [Adjusting Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235043.html)
-   [Removing Serial Numbers on Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235383.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
