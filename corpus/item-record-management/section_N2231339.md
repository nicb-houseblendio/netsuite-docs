---
id: "section_N2231339"
type: "section"
title: "Track Serialized Inventory on Item Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Serial Numbered Items > Track Serialized Inventory on Item Records"
parent: "section_N2230290"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231339.html"
anchors: ["bridgehead_N2231363", "bridgehead_N2231426"]
sha256: "a37407d1aca7d09b0ee98b1c83431d72bb67d344d84d8e409142fac801589124"
---

You can track your purchase and sales of physical inventory items by assigning a serial number to each item. The item's serial number lets you choose a specific serial numbered item to fulfill or receive an order.

After a serialized item is entered, you can view the serial numbers for an item on the Serial Numbers subtab of the item record:

-   Select All in the Filter By field to view all numbers that have ever been associated with this item.
    
-   Select On Hand in the Filter By field to view only the serial numbers that are currently in stock.
    

If you enable the Multi-Location Inventory feature when viewing an item record, the following filters appear in the Location field on the Inventory Numbers subtab:

-   Select All to display information for active locations.
    
-   Select All (including Inactive) to display information from both active and inactive locations.
    

For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).

## Individual Serial Numbers {#bridgehead_N2231363}

Each serial number that contributes to the quantity on hand must be unique. However, note the following. If a serial number was previously sold but not currently on hand, the previously used serial number can be reused on new transactions. You can also purchase or adjust inventory to increase a serialized item's quantity on hand for the previously used serial number. However, that serial number must not contribute to the current quantity on hand for the item.

Note:

If you use Multi-Location Inventory, serial numbers must be unique across all locations.

For example, you purchase a Hi-Tech 9000 2Ghz Computer with a serial number of A1234. You can't buy this computer/serial number combination again until you do one of the following:

-   Sell this serial number
    
-   Use the Adjust Inventory page to remove this serial number from your on hand stock
    

Similarly, you might not receive a customer return for an item/serial number combination if that serial number is currently part of your on hand stock.

Although serial numbers must be unique within any individual serialized inventory item record, you can use the same serial number across **different** serialized items.

For example, you purchase a Hi-Tech 9000 2Ghz Computer with the serial number A1234. You can purchase a Tek-Know 100 3Ghz Computer that also uses the serial number A1234. Because they are two different item records, both can be part of your on hand stock and use the same serial number.

NetSuite warns you if you attempt to bring a serial number into inventory that is currently on hand. You are prompted to enter a new, different serial number. After you enter a new valid serial number, you can add the line item and save the transaction.

## Serialized Item Stock Status {#bridgehead_N2231426}

As you buy and sell serialized inventory, the accounts you specified when you set up your inventory items update. Profit on each serialized item is the difference between the values in the income account and Cost of Goods Sold (COGS) account. This is reflected on your income statement.

You can also view the following quantities for each item on the Items list:

-   **Quantity On Hand** - the number of units that have been received into your inventory that haven't yet been picked for orders.
    
-   **Quantity On Order** - the number of units that have been ordered from the vendor by purchase order.
    
-   **Quantity Committed** - the number of units of an item reserved by unfulfilled sales orders.
    
-   **Reorder Point** - the on-hand inventory level at which you should place an order to restock an item.
    

To view the quantity on hand, quantity on order, quantity committed and reorder point for items, go to _Lists > Accounting > Items_. Choose Stock in the View field.

If you use Inventory Level Warnings at Home > Set Preferences, a popup window notifies you when your inventory reaches the reorder point.

### Related Topics

-   [Enabling Serial Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230646.html)
-   [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html)
-   [Add New Serial Numbers to Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231739.html)
-   [Searching for Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508171622.html)
-   [Receiving a Purchase Order With a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233116.html)
-   [Serialized Items on Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233510.html)
-   [Fulfilling a Sales Order with a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233933.html)
-   [Memorizing Transactions with Serialized Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234305.html)
-   [Building a Serialized Assembly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234538.html)
-   [Adjusting Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235043.html)
-   [Removing Serial Numbers on Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235383.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
