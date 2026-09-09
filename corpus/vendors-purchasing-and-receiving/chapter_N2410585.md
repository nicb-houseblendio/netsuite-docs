---
id: "chapter_N2410585"
type: "chapter"
title: "Receiving Orders"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Receiving Orders"
parent: "book_N2393897"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html"
anchors: ["bridgehead_N2410744", "bridgehead_N2410867", "bridgehead_N2410895", "bridgehead_N2410961"]
sha256: "a704ed47de1578ea62b27521a24018261e2e816254725f490010cae564d4f824"
---

-   [Receipt Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411122.html)
    
-   [Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411320.html)
    
-   [Partially Receiving a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411754.html)
    
-   [Receiving a Purchase Order Before Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415076.html)
    
-   [Receiving a Purchase Orders With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2412119.html)
    
-   [Creating a Bill From an Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162020541497.html)
    
-   [Bulk Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2414814.html)
    
-   [Closing Line Items on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415338.html)
    
-   [Deleting an Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163705803638.html)
    
-   [Exchange Rates on Item Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415572.html)
    
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162626600304.html)
    

Items can arrive at your warehouse for several reasons:

-   Vendors send items you have ordered.
    
-   Customers send items you have authorized to be returned.
    
-   Other company locations send items to transfer to your location.
    

Purchase order items are received from vendors and suppliers. Transfer order items are received from your company's various locations. Return authorization items are received as returns from customers.

As these items arrive at your business, you need to match the items against open purchase orders. transfer orders, or return authorizations. This process is called receiving.

When you receive items at your location, those items need to be recorded in your inventory. It is important to track the items you receive because it affects your stock levels, accounting records and item commitment.

When you receive an order, NetSuite does the following:

-   Updates item stock levels and tracks how much is still on order
    
-   Updates the total asset value of your inventory
    
-   Allocates items to existing sales commitments and backorders.
    

When a shipment arrives, you receive items against an open order to specify that some or all items on the order are received. If you enter an item receipt to specify exactly what you received, you can track items that arrived and the items not yet arrived.

How you receive items depends on whether you use the Advanced Receiving feature.

-   If you do not use Advanced Receiving, the receiving and billing processes are combined. When you receive an item, you create a vendor bill for it simultaneously.
    
-   If you prefer to have separate processes to receive items and create vendor bills, you can use the Advanced Receiving feature.
    
    With Advanced Receiving, you can use separate processes to receive items separately from billing items. Then, you can receive parts of an order before creating a bill for the whole order.
    
-   If you use return authorizations, you can also receive authorized returns in parts using Advanced Receiving and the Item Receipt page.
    

## Receiving Purchase Orders {#bridgehead_N2410744}

When receiving purchase orders, you need to receive the items and create a bill for them.

-   **Receiving** a purchase order indicates you have received items you ordered from a vendor and added them to your inventory.
    
-   **Billing** a purchase order creates a vendor bill for the amount you owe for the products received.
    

The steps to receive and bill orders depend on whether you use the Advanced Receiving feature.

-   If you do not use Advanced Receiving, you receive and bill purchase orders in one step, at the same time.
    
-   If you use Advanced Receiving, you can receive and bill purchase orders as separate transactions. This enables you to receive entire orders or parts of an order, even if you do not bill the order when you receive it.
    
    To enable Advanced Receiving, go to _Setup > Company > Enable Features_. On the Purchase Transactions subtab, check the Advanced Receiving box and then click Save.
    

If you want to include expenses in addition to items on your purchase orders, go to _Setup > Accounting > Preferences > Accounting Preferences_. Check Allow Expenses on Purchase Orders and then click Save.

For more information, see [Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411320.html) or [Receiving a Purchase Orders With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2412119.html).

When you use Advanced Receiving, purchase order items can be matched to the corresponding vendor bill to check for variances in quantities and rates. For more information, see [Posting Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2372745.html).

## Receiving Transfer Orders {#bridgehead_N2410867}

When items being transferred between locations are received by a warehouse, the transfer order must be marked as received by entering an item receipt. Receiving a transfer order into inventory adds the quantities received to the Quantity on Hand count at the receiving location.

If a transfer order has been partially fulfilled, you must match items to a fullfillment when you receive them.

For more information, see [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html).

## Receiving Customer Returns {#bridgehead_N2410895}

When a shipment from a customer arrives at your business, process the return by matching the shipment to the corresponding return authorization number. Then, enter an item receipt for any items in that shipment against the open authorized return.

When you use the Advanced Receiving feature, you can mark authorized returned items as received when they arrive.

By entering a receipt against the RMA, the following information is updated:

-   Items on return authorizations are recorded as received.
    
-   Inventory records are updated for the new stock levels.
    
-   Inventory asset accounts are updated with the values of returned items.
    
-   Status of the return is updated.
    

For more information, see [Receiving a Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html).

## Exchange Rates on Returns {#bridgehead_N2410961}

You can set a preference for how currency exchange rates are handled on returns you process. This helps if exchange rates change between the time an order is entered and when it is received. For more information, see [Exchange Rates on Item Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415572.html).

Related Topics

-   [Requisitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3875569040.html)
    
-   [Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2393987.html)
    
-   [Request for Quote](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4189559896.html)
    
-   [Purchase Contracts and Blanket Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4077153711.html)
    
-   [Purchasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2399286.html)
    
-   [Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2415855.html)
    
-   [Procurement Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4370304623.html)
    
-   [Purchases Workbooks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156439261857.html)
    
-   [Purchasing and Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2393897.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
