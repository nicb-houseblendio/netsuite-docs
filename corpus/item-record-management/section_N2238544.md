---
id: "section_N2238544"
type: "section"
title: "Building a Lot Numbered Assembly"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Lot Numbered Items > Building a Lot Numbered Assembly"
parent: "section_N2235684"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238544.html"
anchors: ["procedure_N2238608"]
sha256: "c4368352335fea84ed1d48d5760dd0046a3db129aec369c57fd5add0b871fb84"
---

In NetSuite, you can build assemblies from inventory items to increase your stock of assembly items.

Lot numbered assembly items let you build items from raw materials and then track the inventory of the finished items and raw materials separately. The completed assembly is assigned a lot number to track it as it enters and leaves your inventory.

#### To build serialized assembly items: {#procedure_N2238608}

1.  Go to _Transactions > Inventory > Build Assemblies_.
    
2.  In the **Reference #** field, you can enter a reference number to track this assembly.
    
3.  In the **Assembly** list, select the lot numbered assembly item you want to build.
    
    You must create assembly item records before you can build assemblies. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
    When you select an assembly item, the maximum number that you can build appears in the **Buildable Quantity** field.
    
4.  In the **Quantity to Build** field, enter the number of assembly items you want to build.
    
    -   You cannot enter a quantity that exceeds the number in the **Buildable Quantity** field.
        
    -   If you use locations, the quantity in the **Buildable Quantity** field represents the selected location.
        
    -   The projected value of your new assemblies appears in the **Projected Value** field.
        
        Projected value is the sum of the value of the member items times the quantity entered.
        
5.  In the **Serial Numbers** field, enter the serial number or numbers for this assembly.
    
    1.  To choose multiple serial numbered items on transactions, click the **Select Multiple** link next to the **Serial/Lot Numbers** field.
        
    2.  In the popup window, select items from the left pane to add it in the right pane.
        
    3.  Click **Done**.
        
        All items in the right pane are added to the transaction.
        
6.  In the **Lot Numbers** field, enter the lot number or numbers for this assembly.
    
7.  The preferred bin number from the assembly item record appears in the **Bin Numbers** field.
    
    1.  If assembly items from this build are stored in other bins, click the **Bins** icon. Bins must be selected on the assembly item record to appear here.
        
    2.  In the popup window, edit the quantity for each bin, and then click **Done**.
        
8.  In the **Date** field, accept today's date or enter another date.
    
9.  Enter the lot **Expiration Date**.
    
    1.  To create a warning that a lot is about to expire, go to Setup > Accounting > Accounting Preferences.
        
    2.  Click the **Items/Transactions** subtab.
        
    3.  In the **Days Before Lot Expiration Warning** field, enter the number of days that you want to receive a warning.
        
    4.  Click **Save**.
        
10.  If you use accounting periods, select a **Posting Period** for this assembly.
     
11.  Optionally, in the **Memo** field, enter any information you want to display on a register or account detail report. You can also search for this text to find this record later.
     
12.  In the Classification section, select a **Department** and **Class**, if needed.
     
13.  Select a **Location** for the built assembly items.
     
     Raw materials are taken from the inventory at this location. The built assembly items are added to the inventory at this location.
     
     To create a new location, select **New**.
     
     For a list of existing locations, go to Setup > Company > Locations.
     
14.  If the assembly contains member items that are lot numbered inventory items, enter or select the lot number for each lot member item.
     
     Lot numbers must be entered in this format: **LOT#(Quantity)**
     
     For example, to enter a quantity of 100 items as Lot number ABC1234, enter **ABC1234(100)**.
     
15.  Click **Save**.
     

After a lot numbered assembly item has been built, it is treated like an inventory item for inventory costing purposes. The lot assembly item asset/costing value is the sum of the values of the assembly's member items. This total value functions as the lot assembly item's purchase price for inventory costing calculations.

### Related Topics

-   [Enabling Lot Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163360479619.html)
-   [Creating Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236287.html)
-   [Receiving a Purchase Order With a Lot Numbered Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236584.html)
-   [Selling and Fulfilling Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236900.html)
-   [Viewing Lot Numbered Inventory Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163360798322.html)
-   [Selecting Lot Numbers on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2236107.html)
-   [Lot Auto Numbering SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162780241331.html)
-   [Allergen Statements SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1562672738.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
