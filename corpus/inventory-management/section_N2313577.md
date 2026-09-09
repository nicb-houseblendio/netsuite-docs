---
id: "section_N2313577"
type: "section"
title: "Intercompany Inventory Transfers - Non-Arm's Length"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Intercompany Inventory Transfers - Non-Arm's Length"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html"
anchors: ["procedure_N2313662", "procedure_N2313742"]
sha256: "2939a31c8cc493d4f7b7bdbd297bfad2b65f150a170b8b27b84c88699100932f"
---

In NetSuite OneWorld accounts, you can enter an Intercompany Transfer Order to move and track inventory between subsidiary locations within your company.

Use Intercompany Transfer Orders for non-arm's length transactions.

-   For arm's length intercompany inventory transfers, see [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html).
    
-   For intercompany drop ship orders, see [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html).
    

Enter an Intercompany Transfer Order to schedule items to be shipped out of one subsidiary location and received into the inventory at another subsidiary location. Intercompany transfer orders enable you to track items in transit between the two subsidiary locations.

For example, you have a surplus of widgets in Japan Subsidiary: Location A, but not enough stock of widgets in US Subsidiary: Location U. You can enter an Intercompany Transfer Order to move the widgets from Japan Subsidiary: Location J to US Subsidiary: Location U, where they are needed.

## Permissions {#procedure_N2313662}

To enter an intercompany transfer, you must have permission to access to the following:

-   the source subsidiary
    
-   the source location
    
-   the common parent of the source subsidiary and destination subsidiary
    

To enter an intercompany transfer that is set to pending approval, you must have permission to access the destination subsidiary in addition to the above.

To fulfill an intercompany transfer or set it to pending fulfillment, you must also have permission to access the destination location.

If your access to subsidiaries or locations is restricted, and you may only process intercompany transfers between locations you are able to access. For details about restricted access, read [Restricting Access to Records by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265799.html).

#### To enter an intercompany transfer order: {#procedure_N2313742}

1.  Go to _Transactions > Inventory > Enter Intercompany Transfer Orders_.
    
2.  Complete the steps as described in the sections below.
    
3.  Click **Save**.
    

After being saved, an intercompany transfer order can be processed.

The Transfer Order Register report shows details for the source subsidiary and destination subsidiary.

#### Primary Information

1.  The **Order #** field shows the correct number if autonumbering is activated. Otherwise, enter the order number in this field.
    
2.  The current **Date** autofills. You can select or enter a different date.
    
3.  In the **Subsidiary** field, select the source subsidiary. The selection you make in this field determines which locations are available to be selected in the **From Location** field.
    
    For example, you select Subsidiary A. Then, you choose a source location from a list of locations limited to only those associated with Subsidiary A.
    
4.  In the **To Subsidiary** field, select the subsidiary where the items are to be received. The selection you make in this field determines which locations are available to be selected in the **To Location** field.
    
    For example, you select Subsidiary B. Then, you can choose a destination location from a list of locations limited to only those associated with Subsidiary B.
    
5.  In the **From Location** field, select the originating location for the transfer. Items are taken out of this location and the inventory count for the item is decreased at the location when the order is fulfilled.
    
    Note:
    
    When you enter an Intercompany Transfer, you must make a selection in the From Location field. The transfer cannot be approved without a source location identified.
    
6.  In the **To Location** field, select the receiving location for the transfer. The inventory count and asset value for the item is increased at this location when the items are received.
    
    You are required to make a selection in the **To Location** field to enter or approve a transfer order.
    
    The **Ship To Address** of the transfer order defaults to the address of the destination location.
    
7.  Optionally choose an **Employee** to associate with this transfer order.
    
8.  The **Status** field shows the current status of the transfer. The default status shown may be pending Approval or Pending Fulfillment, depending on the preference setting. For details on setting this default, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).
    
9.  When the **Firmed** box is checked, the line items are no longer eligible for reallocation to another order. The items must remain committed to the firmed order. Firmed transfer orders are not available to be rescheduled or cancelled.
    
10.  In the **Memo** field, optionally enter information to identify this transaction in a list of other transactions. When you use the Search Transactions feature, you can search for specific words and phrases in the **Memo** field.
     
11.  You can choose a setting for the **Use Item Cost as Transfer Cost** preference to apply to this transaction. However, an intercompany transfer order uses the transfer cost, instead of the item cost for costing calculations. For details about this preference, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).
     
     Note:
     
     If you use approval routing, this setting can be changed on a transfer order if the transfer order is not yet approved. After the transfer order is approved, this setting cannot be changed.
     
12.  Use **Incoterms** to define when the transfer of ownership occurs for items being transferred between locations:
     
     -   Ex Work (EXW) - inventory ownership is transferred at the shipping point
         
     -   Delivered at Place (DAP) - inventory ownership is transferred at the destination point
         
     
     Be aware that the incoterm you select impacts accounting and inventory information. See [Inventory and Accounting Impact of Incoterms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4813066512.html#bridgehead_4813042316).
     
     When creating a transfer order, you can only select **EXW** or **DAP**. After the order status is pending approval or pending fulfillment, you can choose another incoterm.
     

#### Classifications

1.  If you track **Departments** or **Classes**, the form defaults to show the department or class associated with the source subsidiary.
    
    You can select another department or class if necessary.
    

#### Items subtab

1.  In the **Item** field, select the item you want to transfer. Only inventory and assembly items can be added to a transfer order. You can also click the **Add Multiple** button to enter more than one item at a time.
    
    The description of this item shows in the **Description** field.
    
    Only available stock can be committed to transfer orders. The item to transfer must be available for both the source and destination subsidiaries.
    
2.  In the **Quantity** field, enter the quantity of items you want to transfer to another location.
    
    Note:
    
    You should not enter an item quantity that exceeds the item's quantity on hand at the location you are pulling items from inventory. Please review the quantity on hand at that location before entering a value in this field.
    
3.  The **Transfer Price** field defaults to the value in the **Transfer Price** field on the item record. This is based on the currency of the root parent subsidiary. After you enter an intercompany transfer order, the transfer price converts from the root parent subsidiary currency to the currency of the source subsidiary.
    
    You can accept the default value or enter a new one for this order.
    
4.  The unit of measure for the item is displayed in the **Units** field. You can select another unit of necessary.
    
5.  If the item you are transferring is a serial or lot numbered item, enter the serial or lot numbers.
    
    Note:
    
    By entering a specific serial or lot number, you are designating a specific item and NetSuite attempts to allocate the specific item for this order.
    
    Tip:
    
    To enter these details in the Inventory Detail popup window, see [Entering Inventory Details on Transactions or Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0326021504.html).
    
    If you do not enter a specific serial or lot number, NetSuite allocates only the specified quantity of this item to the order. Then, you can designate the specific serial or lot number for the item later.
    
    -   Separate each serial number with a space, comma or by pressing Enter after each one.
        
        You must enter a serial number for each serialized item. For example, if you enter a quantity of 2, then you must enter two serial numbers.
        
    -   Lot numbers must be entered in this format: **LOT#(Quantity)**
        
        For example, to enter a quantity of 100 items as Lot number ABC1234, enter **ABC1234(100)**.
        
    
    When you enter a transfer order, you can enter the serial numbers for items you are transferring. However, you must enter a serial number for each item on the order. You cannot enter serial numbers for only some of the items. After you have entered serial numbers on a transfer order, the **Serial/Lot Numbers** field is disabled on the fulfillment form.
    
    If you do not enter serial numbers for serialized items when you enter the transfer order, note the following. NetSuite enables the **Serial/Lot Numbers** field on the fulfillment form, and you must enter serial numbers there.
    
6.  In the **Commit** column select one of the following:
    
    -   **Available Qty** - Items for this line item are committed as available. Available items are shipped, and items that are not available are placed on backorder.
        
    -   **Complete Qty** - This line item only ships when all items are committed.
        
    -   **Do Not Commit** - Items are not committed to this line item until this setting is changed.
        
7.  Set any options that apply to this item.
    
8.  Click **Add**.
    
9.  Repeat the steps above for each item you want to transfer between these locations.
    

#### Address subtab

1.  The **Ship To Address** of the transfer order defaults to the address of the destination location.
    
    To enter an address manually, select **Custom** in the **Ship To Select** field and enter the address.
    

#### Shipping subtab

1.  To calculate shipping for the transfer items:
    
    1.  In the **Ship Via** field, select a shipping method.
        
    2.  Click the **Calculate** button next to the **Shipping Cost** field.
        

-   If you require approval for transfer orders, approve the appropriate transfers at _Transactions > Inventory > Approve Transfer Orders._.
    
-   If you do not require approval for transfer orders, go to _Transactions > Sales > Fulfill Orders._.
    

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
