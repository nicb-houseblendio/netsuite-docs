---
id: "section_N1224254"
type: "section"
title: "Fulfill a Single Order Using Advanced Shipping"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Advanced Shipping > Fulfill a Single Order Using Advanced Shipping"
parent: "section_N1224089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224254.html"
anchors: ["procedure_N1224279", "bridgehead_N1225860"]
sha256: "bc80f038bb71ff4f953b461a4ab4f1855cbaad4a2a6ac21252a3789260942deb"
---

Use this process to fulfill one order at a time.

For details about enabling the Advanced Shipping feature, read [Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224089.html).

#### To fulfill a single order: {#procedure_N1224279}

1.  Go to _Shipping > Shipping > Fulfill Orders_.
    
2.  Select a customer to show only orders for that customer.
    
3.  In the **Transaction Type** field, select to filter the list for sales orders or transfer orders.
    
4.  In the **Filter By** field, choose one of the following to filter the orders shown:
    
    -   **Some Items Committed** - the list shows orders that have one or more items committed to be fulfilled.
        
    -   **All Items Committed** - the list shows orders that have all items committed to be fulfilled.
        
    -   **Respect Ship Complete** - the list shows only the orders that are committed according to their ship complete setting. This includes all orders that are not restricted to ship complete.
        
    -   **Ignore Item Availability** - the list shows all open orders regardless of the availability of items on the orders.
        
    
    Note:
    
    You cannot fulfill or bill sales orders with the status Pending Approval. You also cannot close lines on a sales order with this status. If you need to make changes to an order that is pending approval, you can remove line items.
    
5.  In the **Process** column, click **Fulfill** next to the order you want to fulfill.
    
6.  On the Item Fulfillment page, verify or enter information in the following fields:
    
    -   **Customer or Project** - the customer or project the order is for
        
    -   **Address** - the customer's address where the order will be shipped
        
    -   **Order #** - the number of the order you are fulfilling
        
    -   **Date** - the date on which the order was fulfilled.
        
    -   **Ref. No.** - a number you can later use to reference this item fulfillment
        
    -   **Ship Via** - the shipping method being used for this order
        
    -   **Shipping Cost** - the total cost of shipping for this order
        
    -   **Tracking Numbers** - any numbers used to track this shipment
        
7.  At the bottom of the page, in the **Quantity** column, enter the amount of each item you are fulfilling.
    
    If you want to fulfill the entire order, make sure the amount in the Quantity column equals the amount in the Remaining column for each item.
    
8.  In the **Serial/Lot Number** field, enter the serial or lot number of the item.
    
    -   Separate each serial number with a space, comma or by pressing **Enter** after each one.
        
        You must enter a serial number for each serialized item. For example, if you enter a quantity of 2, then you must enter two serial numbers.
        
    -   Lot numbers must be entered in this format: **LOT#(Quantity)**
        
        For example, to enter a quantity of 100 items as Lot number ABC1234, enter **ABC1234(100)**.
        
9.  In the **Bin Numbers** column, the preferred bin for that item displays. After this item is picked, you can edit this field if items were pulled from other bins associated with the item.
    
    To edit bins, click the **Bins** icon, change the quantity pulled from each bin associated with the item, and click **Done**.
    
10.  When you have finished, choose one of these options:
     
     -   Click **Save & Bill** to convert the order to an invoice.
         
     -   Click **Save**.
         
         If you save without billing, later you will need to go to _Transactions > Sales > Bill Sales Orders_ to bill the order.
         

Note:

If you fulfill items across periods, additional fields show on this form. For details, read [Fulfilling Orders Across Multiple Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3997655525.html).

Your inventory is updated for the items that you fulfilled. To see what has been fulfilled and invoiced for an order, go to the **History** subtab on the order and click **Fulfillments & Invoices**.

You can also print a label for your shipment. To do this, go to _Transactions > Management > Print Checks and Forms_, and then click the Shipping Labels item. For more information about printing shipping labels, read [Printing Shipping Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262680.html).

For information on how to process multiple orders at once, read [Fulfill Multiple Orders Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1225980.html).

## Fulfilling Overages {#bridgehead_N1225860}

Sometimes when you are fulfilling an order, the amount you are processing is more than the quantity shown on the receipt. This additional amount is called an overage, and NetSuite enables you to process overages using the Allow Overage on Item Fulfillments preference.

If the Advanced Shipping feature is enabled, there is a setting to allow the fulfillment of more items than the original quantity entered on purchase orders.

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  Click the Order Management subtab.
    
3.  Under Fulfillment, check the Allow Overage on Item Fulfillments box.
    
4.  Click Save.
    

With the preference enabled, you can enter a quantity larger than the quantity remaining for an item when processing an item fulfillment.

### Related Topics:

-   [Fulfill Multiple Orders Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1225980.html)
-   [Fulfilling Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
