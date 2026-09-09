---
id: "section_N2310933"
type: "section"
title: "Entering a Transfer Order"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Entering a Transfer Order"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html"
anchors: ["procedure_N2310988"]
sha256: "498a3869aead7eb4c2e6a448a44573a60c280a57d5a871684e807f863036a910"
---

Enter a transfer order to schedule items to be shipped out of one location and received into another location's inventory. Transfer orders enable you to track items in transit between two locations.

Note:

If you are restricted to access only one location, you can create a transfer order, but it will require approval because the source location list shows only one location. The source location will need to be entered to approve the order.

#### To enter a transfer order: {#procedure_N2310988}

1.  Go to _Transactions > Inventory > Enter Transfer Orders_.
    
2.  Complete the fields in each section as indicated below.
    
3.  Click **Save**.
    

#### Primary Information

1.  The **Order #** field shows the correct number if autonumbering is activated. Otherwise, enter the order number in this field.
    
2.  On the Transfer Order form, the **Date** defaults to the current date. You can select or enter another date if necessary.
    
3.  For NetSuite OneWorld accounts, select a **Subsidiary**.
    
    Note:
    
    After selecting a subsidiary on a transfer order, the order must use the base currency designated for that subsidiary.
    
4.  In the **From Location** field, select the originating location for the transfer. Items are taken out of this location and the inventory count for the item is decreased at the location when the order is fulfilled.
    
    You are not required to enter a source location to enter a transfer order, but you must choose a source location to approve and fulfill the transfer order.
    
5.  Optionally choose an **Employee** to associate with this transfer order.
    
6.  In the **To Location** field, select the receiving location for the transfer. The inventory count and asset value for the item is increased at this location when the items are received.
    
    You are required to enter a destination location to enter or approve a transfer order.
    
    The **Ship To Address** of the transfer order defaults to the address of the destination location.
    
7.  The **Status** field shows the current status of the transfer. The default status shown may be pending Approval or Pending Fulfillment, depending on the preference setting. For details on setting this default, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).
    
8.  When the **Firmed** box is checked, the line items are no longer eligible for reallocation to another order. The items must remain committed to the firmed order. Firmed transfer orders are not available to be rescheduled or cancelled.
    
9.  In the **Memo** field, optionally enter information to identify this transaction in a list of other transactions. When you use the Search Transactions feature, you can search for specific words and phrases in the Memo field.
    
10.  Choose a setting for the **Use Item Cost as Transfer Cost** preference to apply to this transaction. This field defaults to use the setting chosen under Accounting Preferences.
     
     If you use approval routing, this setting can be changed on a transfer order if the transfer order is not yet approved. After the transfer order is approved, this setting cannot be changed.
     
     Note:
     
     This preference can be applied to items that use the **Standard** costing method. When this preference is set, NetSuite uses the standard cost at the source location as the transfer cost for those items on the transfer order.
     
     For details about this preference, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).
     
11.  Use **Incoterms** to define when the transfer of ownership occurs for items being transferred between locations:
     
     -   **Ex Work (EXW)** - inventory ownership is transferred at the shipping point
         
     -   **Delivered at Place (DAP)** - inventory ownership is transferred at the destination point
         
     
     Be aware that the incoterm you select impacts accounting and inventory information.
     
12.  To remove the transaction from the most current planning repository version, check the **Exclude from Supply Planning** box.
     
     After selecting this option, you do not need to refresh the repository to get rid of errors. The transaction will be automatically removed from supply planning when the engine is run.
     

#### Classification

1.  If you track **Departments** or **Classes**, select them.
    

#### Items

1.  In the **Item** field, select the item you want to transfer. Only inventory and assembly items can be added to a transfer order. You can also click the **Add Multiple** button to enter more than one item at a time
    
    The description of this item shows in the **Description** field.
    
    Only available stock can be committed to transfer orders.
    
2.  In the **Quantity** field, enter the quantity of items you want to transfer to another location.
    
    Note:
    
    You should not enter an item quantity that exceeds the item's quantity on hand at the location you are pulling items from inventory. Please review the quantity on hand at that location before entering a value in this field.
    
3.  The **Transfer Price** field defaults to show the value in the Transfer Price field on the item record. You can accept the default value or enter a new one for this order.
    
    The use of the value entered in the **Transfer Price** field depends on your setting for the **Use Item Cost as Transfer Cost** preference. This field defaults to show a value of zero if the field is blank or shows zero on the item record.
    
    -   When the Use Item Cost as Transfer Cost preference is enabled, the transfer price is not considered for posting cost accounting of line items. In the Transfer Price field, enter a declared value for the item to be used for shipping purposes only.
        
    -   When the Use Item Cost as Transfer Cost preference is disabled, the transfer price is considered during the posting of cost accounting lines. Items that do not have a transfer price set on the transfer order use a zero value for cost accounting calculations when the item is received.
        
4.  The unit of measure for the item is displayed in the **Units** field. You can select another unit of necessary.
    
5.  If the item you are transferring is a serial or lot numbered item, enter the serial or lot numbers.
    
    Note:
    
    By entering a specific serial or lot number, you are designating a specific item and NetSuite attempts to allocate the specific item for this order. If you do not enter a specific serial or lot number, NetSuite allocates only the specified quantity of this item to the order. Then, you can designate the specific serial or lot number for the item later.
    
    Tip:
    
    To enter these details in the Inventory Detail popup window, see [Entering Inventory Details on Transactions or Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0326021504.html).
    
    -   Separate each serial number with a space, comma or by pressing Enter after each one.
        
        You must enter a serial number for each serialized item. For example, if you enter a quantity of 2, then you must enter two serial numbers.
        
    -   Lot numbers must be entered in this format: **LOT#(Quantity)**
        
        For example, to enter a quantity of 100 items as Lot number ABC1234, enter **ABC1234(100)**.
        
    
    When you enter a transfer order, you can enter the serial numbers for items you are transferring, but you must enter a serial number for each item on the order. You cannot enter serial numbers for only some of the items. After you have entered serial numbers on a transfer order, the **Serial/Lot Numbers** field is disabled on the fulfillment form.
    
    If you do not enter serial numbers for serialized items when you enter the transfer order, then the **Serial/Lot Numbers** field is enabled on the fulfillment form and you must enter serial numbers there.
    
6.  In the **Expected Ship Date** field, enter the date you expect this item to be shipped from the vendor. This defaults to show the transaction date.
    
7.  In the **Expected Receipt Date** field, enter the date you expect this item to arrive in your warehouse. This defaults to show the transaction date.
    
8.  In the **Commit** column select one of the following:
    
    -   **Available Qty** - Items for this line item are committed as available. Available items are shipped, and items that are not available are placed on backorder.
        
    -   **Complete Qty** - This line item only ships when all items are committed.
        
    -   **Do Not Commit** - Items are not committed to this line item until this setting is changed.
        
9.  Set any options that apply to this item.
    
10.  Click **Add**.
     
11.  Repeat the steps above for each item you want to transfer between these locations.
     

#### Shipping

1.  The **Ship Date** field defaults to show the current date. You can type or pick another shipping date for this order.
    
2.  The **Shipping Carrier** field displays the carrier associated with the customer, if available, or your default shipping carrier. You can select a different carrier.
    
3.  In the **Shipping Method** field, select a shipping method for this order.
    
    Select a shipping method for this order.
    
    If you automatically charge for shipping, the shipping amount is entered in the shipping costs field. To automatically charge for shipping, go to _Setup > Accounting > Shipping_ and check the **Charge for Shipping** box, then click **Submit**. You must also set up the charge details of your shipping items.
    
    To add or edit shipping items, go to _Lists > Accounting > Shipping Items_.
    
4.  The **Shipping Cost** calculates automatically depending on the shipping method you select above. To change the cost of a shipping method, go to _Lists > Accounting > Shipping Items_ and select the shipping method you want to change. If you use UPS Real-Time rates and a package is over 150 lbs, the package is charged as multiple packages equal to or less than 150lbs.
    
    To calculate shipping for the transfer items, click the **Calculate** button.
    
5.  In the **Handling Cost** field, enter the price you want to charge for this item's handling.
    
6.  The **Ship To Address** of the transfer order defaults to the address of the destination location.
    
    To enter an address manually, select **Custom** in the **Ship To Select** field and enter the address.
    

#### Communication

1.  Click the **Communication** subtab to associate activities, notes or files with this transaction.
    
    -   Use the **Events**, **Tasks**, and **Phone Calls** subtabs to attach activities to this transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
        
    -   On the **Files** subtab, you can select and attach files from the File Cabinet related to this transaction. Select **New** to upload a new file to File Cabinet.
        
    -   On the **User Notes** subtab, you can enter a title and note for any comments you want to add to this transaction. Click **Add** after each note.
        

Now, this transfer order can be processed.

-   If you require approval for transfer orders, approve the appropriate transfers at _Transactions > Inventory > Approve Transfer Orders._.
    
-   If you do not require approval for transfer orders, go to _Transactions > Sales > Fulfill Orders._.
    

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
