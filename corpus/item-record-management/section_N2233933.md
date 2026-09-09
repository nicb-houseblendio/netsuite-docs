---
id: "section_N2233933"
type: "section"
title: "Fulfilling a Sales Order with a Serialized Item"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Serial Numbered Items > Fulfilling a Sales Order with a Serialized Item"
parent: "section_N2230290"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233933.html"
anchors: ["procedure_N2233961", "bridgehead_N2234087"]
sha256: "c73f242dad6340277521970a43aeff5597cdf9a06341711fa3cc39b2423b082f"
---

If a serialized inventory item is selected on a sales transaction, you must enter a serial number to fulfill the items from inventory.

For example, you create a sales order that includes a serialized item, but you don't enter the serial number for that item. Later, when you fulfill that sales order, you are required to enter the serial number for the serialized item.

#### To fulfill a sales order that contains a serialized item: {#procedure_N2233961}

1.  Go to _Transactions > Sales > Fulfill Orders_.
    
2.  On the Fulfill Orders page, in the **Customer** field, select a single customer or **All**.
    
3.  Beside the sales order you want to fulfill, check the **Fulfill** box.
    
    To select all orders, click **Mark All**.
    
4.  On the Item Fulfillment page, click the line that shows the serialized item.
    
5.  In the **Serial Number** field, enter the serial number of the item.
    
    The quantity of serial numbers entered must match the quantity of serialized items on each transaction line. For example, if you're fulfilling three serialized items, you must enter three serial numbers.
    
    1.  To choose multiple serial numbered items on transactions, beside the **Serial/Lot Numbers** field, click the **Select Multiple**.
        
    2.  In the popup list, click items from the left pane to add to the right pane list.
        
    3.  Click **Done**.
        
        All items in the right pane of the popup window are added to the transaction.
        
    
    Note:
    
    You can enter a maximum of 4000 characters in this field.
    
6.  Click **Save**.
    
    The items are fulfilled from your inventory.
    

For information about fulfilling serialized inventory using Multiple Units of Measure, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

For information about fulfilling kit items that include serialized inventory, see [Entering Serial and Lot Components on the Item Record for the Kit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225398.html).

## Bulk Fulfillment {#bridgehead_N2234087}

To bulk fulfill a batch of sales orders, sales orders with serialized items must include the corresponding serial numbers. If a serialized item on a sales order doesn't have a serial number, you can't bulk fulfill. You must fulfill the sales order individually to enter the serial number.

### Related Topics

-   [Enabling Serial Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230646.html)
-   [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html)
-   [Track Serialized Inventory on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231339.html)
-   [Add New Serial Numbers to Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231739.html)
-   [Searching for Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508171622.html)
-   [Receiving a Purchase Order With a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233116.html)
-   [Serialized Items on Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233510.html)
-   [Memorizing Transactions with Serialized Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234305.html)
-   [Building a Serialized Assembly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234538.html)
-   [Adjusting Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235043.html)
-   [Removing Serial Numbers on Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235383.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
