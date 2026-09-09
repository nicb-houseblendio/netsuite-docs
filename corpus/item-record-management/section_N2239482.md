---
id: "section_N2239482"
type: "section"
title: "Setting Up Drop Shipping"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Drop Ship Items > Setting Up Drop Shipping"
parent: "section_N2239232"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239482.html"
anchors: ["subsect_163404780417", "subsect_163404802462", "procedure_N2239618"]
sha256: "018dfa2a5c87d1b8a0638cffc9236d099d87bd0adeff1af6fca361951ca09be1"
---

When you drop ship an item, the item is sent directly from your vendor to your customer. The item isn't processed in your inventory.

To set up the drop ship feature, do the following:

-   [Enabling the Drop Shipments and Special Orders Feature](#subsect_163404780417)
    
-   [Setting up Your Drop Ship Preferences](#subsect_163404802462)
    

## Enabling the Drop Shipments and Special Orders Feature {#subsect_163404780417}

Use the following procedure to enable the Drop Shipments and Special Orders feature.

#### To enable the Drop Shipments and Special Orders feature:

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Items and Inventory** subtab.
    
3.  Check the **Drop Shipments & Special Orders** box.
    
4.  Click **Save**.
    

Note:

Drop Shipments are a function of the Drop Shipments and Special Orders feature. After you enable the feature, an item can be either a drop ship or special order, but not both.

The table below explains the differences between special order and drop ship items:

| Function | Drop Shipment | Special Order |
| --- | --- | --- |
| Sales revenue tracked in NetSuite | YES | YES |
| Purchase order form | Drop Ship PO form | Preferred PO form |
| P.O. links to sale | YES | YES |
| Vendor ships to | your customer's address | your company's address |
| Inventory impact | None-when it is not received into inventory | Impacts Asset and Cost of Goods Sold (COGS) accounts upon receipt and fulfillment |
| Item commitment | **Drop shipments do not commit.** | A special order item always commits upon receipt of the linked PO-it **is not** committed from stock on hand. |
| Can be used for inventory items and non-inventory for resale items | YES | YES |
| Item record can default to this method | YES | YES |
| Item Fulfillment | Can be marked as fulfilled before or after the linked purchase order has been received. | Can be fulfilled only after the linked purchase order has been received. |

## Setting up Your Drop Ship Preferences {#subsect_163404802462}

Use the following procedure to set up your drop ship preferences.

#### To set up your drop ship preferences: {#procedure_N2239618}

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **Order Management** subtab.
    
3.  In the **Drop Ship P.O. Form** list, select the default form to use for drop ship purchase orders.
    
4.  Check the **Automatically Email Drop Ship P.O.s** box to automatically email your drop ship item purchase orders to the preferred vendor.
    
    To use this preference, enter the preferred vendor's email address on that vendor record.
    
    Note:
    
    The drop ship email is generated only if you update the purchase order directly. It is not generated if the purchase order is updated based on a sales order change.
    
5.  Check the **Queue Drop Ship P.O.s for Printing** box to automatically queue drop ship purchase orders for printing.
    
    To print these purchase orders, go to _Transactions > Management > Print Checks and Forms > Purchase Orders_, and then click Purchase Orders.
    
6.  Check the **Automatically Fax Drop Ship P.O.s** box to automatically fax drop ship item purchase orders to the preferred vendor.
    
    To use this preference, enter a preferred vendor on the item record and a vendor fax number on the vendor record.
    
    The **Limit Vendor List on Items** preference filters available vendors on sales orders and the order items page. If enabled, only vendors associated with an item appear in the **Vendor** list. If disabled, the list displays all vendors.
    
7.  To drop ship or special order an inventory item where part of the ordered quantity is unavailable, choose a setting to **Include Committed Quantities**. The quantity ordered from the vendor depends on your setting for this preference:
    
    -   When **Disabled**, click the **Drop Ship/Special Order** link to create a purchase order for only the backordered quantity.
        
    -   When **Enabled**, click the **Drop Ship/Special Order** link to create a purchase order for the entire quantity ordered, not the backordered quantity.
        
8.  To skip the sales order approval process by default, in the **Default Sales Order Status** list, select **Pending Fulfillment**. You can still change the status on each sales order you create.
    
    If **Pending Fulfillment** is the default sales order status, the status field on sales orders is unavailable and sales orders can no longer be edited.
    
    1.  To edit the status of a sales order in pending fulfillment status, open the sales order and then click the **History** subtab.
        
    2.  On the **Fulfillments & Invoices** subtab, click the **Date** column link to open the transaction for editing.
        
9.  Choose a setting for the following preferences:
    
    -   **Update Drop Ship Order Quantities Automatically Prior to Shipment**
        
    -   **Drop Ship Fulfillment Quantity Validation**
        
    -   **Allow Both Mark Shipped Fulfillments and Receipts on a Drop Shipment Line**
        
    
    For more information, see [Drop Shipping Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163412960428.html).
    
10.  Click **Save**.
     

After drop ship features are enabled and preferences set, you can drop ship inventory items or non-inventory for resale items.

To drop ship an item, mark the item record as a drop ship item. When the item is entered on a sales order it defaults to drop ship. For more information, see [Marking an Item for Drop Shipment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239986.html).

After an order with an item marked for drop shipment is approved, the purchase order is automatically created.

### Related Topics

-   [Viewing a Drop Ship Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2241194.html)
-   [Selling a Drop Ship Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2241390.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
