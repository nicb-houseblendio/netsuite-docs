---
id: "section_N2321340"
type: "section"
title: "Building Assembly Items"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Items > Building Assembly Items"
parent: "chapter_N2319010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321340.html"
anchors: ["kaltura_player_178", "procedure_N2321414", "subsect_0402021443"]
sha256: "8c0bf89c46c9c1734bef1cb25da19bbe522baba5b744f7a80d508371fda36247"
---

Each time you physically manufacture assemblies in a production run, you increase your stock of the assembled items. Record each production run and update stock levels by entering an assembly build record.

<a id="kaltura_player_178"></a>

For each assembly build you record:

-   the assembly item stock levels increase
    
-   the member items' individual stock levels decrease
    

Entering an assembly build for each production run updates your inventory levels.

Note:

If you use work orders and have entered work orders for assemblies, see [Building Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331860.html) to complete builds for those assemblies.

#### To enter an assembly build: {#procedure_N2321414}

1.  Go to _Transactions > Manufacturing > Build Assemblies_.
    
2.  Under the **Primary Information** section, complete the following fields:
    
    1.  The **Reference #** field displays a system generated number.
        
        You can enter a different reference number to track this transaction.
        
    2.  In the **Assembly** list, select the assembly item you want to build.
        
        You can enter an assembly build only for assembly items on record. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
        
    3.  The **BOM Revision** is defaulted based on the transaction date.
        
        The revision record effective date determines when this item is included as a member for an assembly.
        
        When you select an assembly item, the maximum number that you can build appears in the **Buildable Quantity** field.
        
        If you use locations, the quantity for the selected location is displayed in the Buildable Quantity field.
        
    4.  In the **Quantity to Build** field, enter the number of assembly items you want to build.
        
    5.  The **Projected Value** of your new assemblies is displayed.
        
        Projected value is the sum of the value of the member items times the quantity entered.
        
    6.  To add assemblies to other bins, click the **Inventory Detail** icon.
        
    7.  If you use serialized inventory, enter serial numbers for the assemblies you are building.
        
    8.  In the **Date** field, enter a transaction date.
        
    9.  Select the account **Posting Period** you want to post this transaction to.
        
        You cannot post to closed periods.
        
    10.  If you use bin management, the assembly item record preferred bin number is displayed in the **Bin Numbers** field. By default, all assemblies are added to the preferred bin. To add some assemblies to other bins, click the Bins icon or the Inventory Detail icon.
         
         When you build this assembly, the bin quantity on hand for the assembly increases and the bin quantity on hand for each member item decreases.
         
    11.  If you are building a lot numbered assembly item, enter the lot **Expiration Date** field.
         
         1.  To receive a warning that a lot is about to expire, go to Setup > Accounting > Preferences > Accounting Preferences.
             
         2.  On the **Items/Transactions** subtab, in **Days Before Lot Expiration Warning**, enter the number of days before a lot item's expiration to display a warning.
             
         3.  Click **Save**.
             
    12.  Enter a **Memo**. You can search for this text later to find this entry.
         
3.  In the **Classification** section, complete the following fields:
    
    1.  If you use NetSuite OneWorld, select a **Subsidiary**.
        
    2.  If you track departments, select a **Department** for this transaction.
        
    3.  If you track classes, select a **Class** for this transaction.
        
    4.  If you track locations, select a **Location** for this transaction.
        
4.  On the **Components** subtab, accept the default quantity of each component needed to complete the assembly. This number is taken from the assembly Item record.
    
    You can adjust component quantities on a build-by-build basis to allow for fluctuations in material usage. For example, a member item record shows a component quantity of 2. You can create a build that has 3 of the component to fill a particular order. As the quantity changes, your projected value is updated.
    
    Note:
    
    You can change the quantity of members on a serialized or lot numbered assembly. Use the assembly serial or lot numbers to track assembly items created with special member quantities. You cannot track non-serial or non-lot assemblies that could have special quantities of member items. Therefore, you may want to build non-serial or non-lot assemblies with special quantities. You can build when your available quantity of that assembly is zero and you are building assemblies with special quantities for a customer order.
    
5.  Click the **Communication** subtab.
    
    1.  Enter events on the **Events** subtab. For example, maintenance, repair, or setup.
        
        1.  Enter the event name or **Title**. For example, Assembly Work Center Setup.
            
        2.  Enter the event **Location**. For example, West Coast Assembly.
            
        3.  Accept today's **Date** or use the calendar to enter a different date.
            
        4.  If this is an all day event, check the **All Day** box.
            
        5.  Enter event **Start** and **End Times**.
            
        6.  Click **Add**.
            
            To add more events, repeat this procedure.
            
            For example, Setup could start at 7:00 am and end at 7:30 am. Then, Assembly could start at 7:30 am and end at 3:30 pm. Finally, Breakdown could start at 3:30 pm and end at 4:30 pm.
            
    2.  On the **Tasks** subtab, view or enter CRM tasks records. For information about tasks, see [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html).
        
    3.  The **Phone Calls** subtab enables you to view or enter phone calls.
        
    4.  The **Files** subtab enables you to attach files from the NetSuite File Cabinet, your computer, or the internet.
        
        -   To add a file from the File Cabinet, select one from the **Attach File** list.
            
            After the file loads, NetSuite fills the **Folder**, **Size**, **Last Modifed**, and **File Type** fields.
            
        -   To add a new file, in the **Attach File** list, select **New**.
            
            Complete the List window.
            
    5.  On the **User Notes** subtab, add and track notations.
        
6.  Click **Save**.
    

After an assembly item is built, it is treated like an inventory item for inventory costing purposes. The built assembly item asset/costing value is the total value of the assembly's member items. These values act like the assembly item's purchase price for inventory costing calculations.

Note:

If you use NetSuite OneWorld, you can select the purchase currency on non-inventory items for purchase and resale.

Inventory costing is tracked for the assembly item based on the inventory costing method chosen at _Setup > Accounting > Preferences > Accounting Preferences_. For information about inventory costing, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

## Copying an Assembly Item {#subsect_0402021443}

An assembly item is an inventory item made of several components, but identified as a single item. Assemblies are manufactured by combining raw materials you stock. Some assembly items have similar components or an assembly may be updated with some new slightly different components.

Instead of building a new assembly item, NetSuite enables you to copy an existing assembly item that you can then edit to reflect the differences in your new assembly.

For example, your organization's flagship road bicycle is the RD Tour series. This year, the RD Tour 5000 line is being built with an improved chain and gear components. Instead of building a new assembly for two new components, copy the previous RD Tour 5000 assembly item and update the component list.

#### To copy an assembly item:

1.  Go to Lists > Accounting > Items.
    
2.  Beside the assembly item you want to copy, click **View**.
    
3.  Click **Actions** > **Make Copy**.
    
4.  Rename your new assembly item.
    
5.  Complete the new assembly inventory item page.
    
6.  Click **Save**.
    

### Related Topics

-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Enabling Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319428.html)
-   [Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319594.html)
-   [Assemblies on Purchase Transactions, Web Sites, and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161487042976.html)
-   [Matrix Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4249789892.html)
-   [Phantom Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4714298883.html)
-   [Assemblies and Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2320172.html)
-   [Unbuilding Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321882.html)
-   [Marking Work Orders Built](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2322811.html)
-   [Printing an Item Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323540.html)
-   [Bill of Materials Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324073.html)
-   [Costed Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160730538.html)
-   [Printing Assembly Item Materials on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324339.html)
-   [Printing Assembly Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324547.html)
-   [Running the Component Where Used Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511882961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
