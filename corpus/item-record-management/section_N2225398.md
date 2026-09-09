---
id: "section_N2225398"
type: "section"
title: "Entering Serial and Lot Components on the Item Record for the Kit"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Kit/Package Items > Entering Serial and Lot Components on the Item Record for the Kit"
parent: "section_N2225190"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225398.html"
anchors: ["bridgehead_N2225555"]
sha256: "095cff353f98bd6b12a7ba2185ccf8539e19583b0c83a917f6f3f3a1e3f7bf05"
---

Kits can include components that are lot numbered or serial numbered. You can add lot and serial numbered components on the kit item record.

To use the serialized or lot items as a kit item member, enable the following features:

-   Advanced Shipping
    
-   Advanced Receiving
    
-   Advanced Bin/Numbered Inventory Management
    

You can include serial or lot numbered items as members for kit items on fulfillment and return transactions when you use the following features:

-   Serialized Inventory or Lot Tracking
    
-   Advanced Shipping
    
-   Advanced Bin Management
    
-   Advanced Receiving (to use this process for returns)
    

Note:

All components within the kit must be fulfilled or returned from a single location.

After you enable features, you can enter serial and lot components on the item record for the kit on fulfillment and return transactions.

#### To enter serial and lot components on the item record for the kit:

1.  Go to _Lists > Accounting > Items_.
    
2.  Beside the kit name, click **Edit**.
    
3.  Click the **Purchasing/Inventory** subtab.
    
4.  Add members on the **Components** subtab .
    
5.  Click **Save**.
    

Note:

When you process orders, kits with serial and lot members can be used to create a sales order or invoice. They can also be used to fulfill an item.

You can't use this feature on standalone cash sales or invoices. Invoices must be created from a sales order.

When fulfilling the item, use the **Inventory Detail** icon to open the popup window. Then, select a specific serial or lot number for that order. You can display this icon in the following two ways:

-   **Arrow** ![Inventory Detail Arrow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/InventoryDetailIconBlue.png) - The arrow icon indicates that the inventory detail is available for the item and needs to be configured. It appears only in edit mode for a transaction.
    
-   **Check Mark** ![Inventory Detail Check Mark](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/InventoryDetailIconGreen.png) - The check mark icon indicates that you have already configured the inventory detail for this item. It appears in view mode for transactions, and edit mode after you configure the inventory detail.
    

Note:

Permissions for the inventory detail icons are inherited from its parent transaction. For example, to edit the inventory detail from a sales order, you must have permission to edit the sales order. For more information, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

## Item Returns {#bridgehead_N2225555}

NetSuite supports serial and lot items within kits as part of the returns management process. Portions of kits with serial and lot members can be returned into inventory by creating a return authorization and then creating an item receipt.

Inventory details for serial and lot items within the kit can be updated on the receipt. When returning these kits, you can choose the serial or lot number, and also choose whether to restock the item.

The kit members that display are based on the item receipt type:

-   If the return is standalone, the kit members displayed are based on the item record definition.
    
-   If the return is linked to an existing transaction, the kit members displayed are based on the kit member definition on the original sales order.
    

### Related Topics

-   [Updating Kits with Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225728.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
