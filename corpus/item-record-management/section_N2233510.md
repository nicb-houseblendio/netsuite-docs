---
id: "section_N2233510"
type: "section"
title: "Serialized Items on Sales Transactions"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Serial Numbered Items > Serialized Items on Sales Transactions"
parent: "section_N2230290"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233510.html"
anchors: []
sha256: "f687a85f3ff34401e7b5483382b4055b7d034e6f02c23cac84d2595179532d31"
---

When selling serialized items on sales transactions, you should consider the following:

-   In the Item field on sales transactions, you can choose a serialized item from the inventory list. Select a serialized item by entering the item name, UPC, or serial number. When you enter a serial number, the item name or UPC autofills in the Item field.
    
-   Serialized items added to sales transactions must include a serial number for each item when the transaction posts.
    
    -   If a serialized inventory item is selected on a non-posting sales transaction, you enter a serial number when the order is fulfilled.
        
        Non-posting sales transactions include the following:
        
        -   Prepare Estimates
            
        -   Enter Sales Orders
            
        
        If a serial number is entered on a non-posting sales transaction, that serial number **is not on hold** and is available for sale on transactions.
        
    -   If a serialized inventory item is selected on a posting sales transaction, enter a serial number on that transaction.
        
        Posting sales transactions include the following:
        
        -   Create Invoice
            
        -   Enter Cash Sale
            
        -   Fulfill Sales Orders
            
            In the Serial Numbers field on a posting sales transaction, enter or select the serial number of the item you are selling. The quantity of serial numbers entered must match the quantity of serialized items on each transaction line.
            
            For example, if you're fulfilling three serialized items, the fulfillment must show three serial numbers.
            
-   To add a new serialized inventory item, go to _Lists > Accounting > Items > New_. Then, under Inventory Item, click Serialized.
    
-   To choose multiple serial numbered items on sales transactions, click the Select Multiple link next to the Serial/Lot Numbers field. A popup window lists available serial numbers for the item. Click each item in the left pane to add it in the list right pane and then, click Done. All the items in the right pane of the popup window are added to the transaction.
    
-   When you view a sales order, invoice, or cash sale that has more than 10 serial numbers entered, **More...** displays below the serial numbers. If you point your cursor at **More...**, a tooltip window opens that lists all the serial numbers. You can click a serial number in this tooltip window to open the serial number record.
    
-   After an order is fulfilled and billed, the serial number on the cash sale or invoice appears for information only. Changes made to the serial number no longer affect inventory.
    
-   If you change a serial number on a transaction, the serial number is not updated automatically on any existing linked transactions. You must update the serial number manually on the linked transactions to match the new serial number. For example, you change the serial number on a sales order when an item fulfillment record has already been created and linked to the order. You must also update the serial number on the item fulfillment.
    

Note:

When you view a saved sales transaction that includes a serialized item. If you click the serialized number to view or edit values in the Memo field or a custom field on the inventory number record. For more information, see [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html).

For information about selling serialized inventory using Multiple Units of Measure, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

For information about best practices for committing numbered inventory, see [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html).

### Related Topics

-   [Enabling Serial Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230646.html)
-   [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html)
-   [Track Serialized Inventory on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231339.html)
-   [Add New Serial Numbers to Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231739.html)
-   [Searching for Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508171622.html)
-   [Receiving a Purchase Order With a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233116.html)
-   [Fulfilling a Sales Order with a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233933.html)
-   [Memorizing Transactions with Serialized Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234305.html)
-   [Building a Serialized Assembly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234538.html)
-   [Adjusting Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235043.html)
-   [Removing Serial Numbers on Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235383.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
