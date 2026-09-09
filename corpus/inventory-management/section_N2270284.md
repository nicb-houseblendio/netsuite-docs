---
id: "section_N2270284"
type: "section"
title: "Bin Management"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management"
parent: "chapter_N2250682"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html"
anchors: ["bridgehead_N2270434", "bridgehead_N2270486", "bridgehead_N2271127", "bridgehead_N2271186", "bridgehead_N2271260", "bridgehead_N2271276", "bridgehead_0419100225", "bridgehead_N2271313"]
sha256: "eaa78793e43fdf7771501dadf7db9d42d848e8e9689f15d80613aae9ae54d792"
---

Bin Management enables you to identify areas and places in a location where you store inventory items. Bins help you organize and track on-hand quantities of items within a warehouse or location.

Tracking items by bins can help organize item receiving and simplify item picking to fulfill orders, among other inventory processes. When you receive a purchase order, you can choose the bins in which to put the items. Bin Management enables you to track the stock levels of items that you put away in bins. When you enter an item on a sale, you can specify the bin to pull the item from based on available quantities. By specifying bins on orders, warehouse operators know where to go to pick the quantity of items when fulfilling an order. They also know exactly what items need to be put away, or stocked, and where, after they are received from vendors.

NetSuite provides the following features for bins:

-   **Bin Management** - A basic means of tracking inventory in bins. This feature requires that you associate bins with items before you can use bins on transactions. This feature does not allow using bins with serialized and lot numbered items or on a per-location basis.
    
    To learn more and set up, see [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html).
    
-   **Advanced Bin / Numbered Inventory Management** - An enhanced version of tracking bins, including serial numbered and lot numbered items and on a per-location basis. Using this feature, you are not required to pre-associate bins with items to use bins on transactions. Also, you can associate bins with serialized and lot numbered items or use bins on a per-location basis.
    
    To learn more and set up, [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html).
    

The information in the following sections apply to both basic and advanced Bin Management, unless stated otherwise:

## Put Away Items in Bins {#bridgehead_N2270434}

Use Bin Put-Away Worksheets as you process items that use bins to store received items, restock them, or assign quantities of an item per bin. Print a basic Bin Put-Away Worksheet that contains the list of received items and their associated bins within a location. Worksheets also show the current on-hand quantity in each bin for reference.

Items that you already associate with bins on an item receipt or inventory adjustment do not appear in a Bin Put-Away Worksheet. If you set the **Use Preferred Bin on Item Receipts** preference, all received items are placed in the preferred bin for that location by default. To put away an item later using a worksheet, set the quantity for the preferred bin to zero on the item receipt.

## Receive with Bins {#bridgehead_N2270486}

When you receive items for a purchase order or customer return, the following related transactions include the bin numbers:

-   Cash Refunds
    
-   Credit Card purchases
    
-   Checks
    
-   Vendor Bills
    
-   Inventory Adjustments
    
-   Inventory Transfers
    

## Bins on Sales and Transfers {#bridgehead_N2271127}

When customers submit sales orders or when you create transfer orders, the following related transactions that apply to the order include the bin numbers:

-   Picking tickets
    
-   Item fulfillments
    
-   Invoices
    

Note:

Use of the Multi-Location Inventory feature differs whether you use basic or advanced Bin Management. For more information, see [Bin Management by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4713998969.html).

## Bins on Picking Tickets {#bridgehead_N2271186}

Your employees can print the picking tickets to automatically find the bins for the items needed to fill the order. Bins are included on a picking ticket using the following logic:

-   If the preferred bin has sufficient quantity to pick item, only the preferred bin is printed on the picking ticket.
    
-   If you need multiple bins to meet the item quantity, each bin is listed on the picking ticket, with the preferred bin listed first.
    
-   If the preferred bin has zero quantity, and no other bin has quantity to pick all items, bins appear in order of descending quantity.
    
-   Only bins with quantity greater than or equal to the quantity ordered are printed on the picking ticket.
    
-   A Bin Number column is only included on a picking ticket if the ticket includes items with associated bin numbers.
    

A picker can pull a quantity from a bin different from what is listed on the picking ticket. However, the picker should edit the quantity taken from each bin on the item fulfillment page.

## Data Tracked Per Bin {#bridgehead_N2271260}

Using either bins feature, item costing is not calculated per bin. Only on-hand quantity is tracked per bin. Available, committed, backordered, and ordered quantities are also not tracked per bin.

## Specify Bins on Transactions {#bridgehead_N2271276}

Bins are required on all cash sales, invoices, and negative inventory adjustments with bin items. This is true with any state of the **Require Bins on All Transactions Except Item Receipts** preference.

For example, you enter a cash sale with a bin item that specifies a location. The item is required to have at least one bin in that location. Also, when you enter an inventory adjustment, any line that deducts a quantity of an item that uses bins will require a bin.

When you edit an existing sale transaction that has a bin item but no bin specified, bins must be specified on the transaction.

If you do not specify a bin, you see the notice: 'The number of bins entered (0) is not equal to the item quantity (x)'.

Note:

NetSuite does not require bins on positive adjustments or purchases because you can use a Bin Putaway Worksheet later. This is true unless the **Require Bins on All Transactions Except Item Receipts** preference is enabled.

## Preferred Bins for Items {#bridgehead_0419100225}

You can assign preferred bins to items that use bins. When you include the item on a transaction, its preferred bin is used as follows:

-   If the preferred bin quantity can cover the transaction, the preferred bin is used.
    
-   If the preferred bin quantity cannot cover the transaction but another single bin can cover the transaction, that bin is used.
    
    Otherwise, you must distribute the quantities among bins that contain the item to cover the total quantity. For advanced Bin Management, you must configure the Inventory Detail record to process the transaction.
    
-   When you issue work orders and an item's preferred bin contains insufficient quantity, you can manually select another bin. Otherwise, you may encounter an error. For more information about work order issues, see [Entering Work Order Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2338862.html).
    

These conditions apply only to non-serial numbered and non-lot numbered items.

## Bins and Assembly Items {#bridgehead_N2271313}

If you use the Assembly Items feature, you must designate a bin for any component item in a build which uses bins. If a parent assembly item uses bins, you must designate a bin for that item to unbuild it.

You are not required to designate a bin for a member item in an unbuild or for an assembly item in a build. This is true unless the **Require Bins on All Transactions Except Item Receipts** preference is enabled.

### Related Topics

-   [Enabling Features for Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161963741628.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html)
-   [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html)
-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html)
-   [Printing Bin Putaway Worksheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2275156.html)
-   [Updating Bin Putaway Worksheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2277819.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)
-   [Disabling Use Bins Settings and Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0512092419.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
