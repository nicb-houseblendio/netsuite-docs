---
id: "section_N1230473"
type: "section"
title: "Fulfilling Orders Using Pick, Pack, and Ship"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Pick, Pack, and Ship > Fulfilling Orders Using Pick, Pack, and Ship"
parent: "section_N1229691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230473.html"
anchors: ["procedure_N1230525", "bridgehead_1525085414"]
sha256: "6f11158f0da9e160f091275fd7692e754e416e2984f030d18f0747f1659ee509"
---

The Pick, Pack, and Ship feature gives your warehouse and shipping departments separate processes for each step to fulfill orders. To use Pick, Pack and Ship, you must enable the feature and set preferences. For more information, see [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html).

Warehouse employees pick the items needed to fulfill the order from inventory and then physically package them for shipping. Then, the shipping department marks an order shipped when the order is on the way to its destination.

You can track orders through each step of the fulfillment process. Possible statuses for a fulfillment are Picked, Packed, or Shipped.

To view a list of item fulfillments and their statuses, go to _Shipping > Shipping > Fulfill Orders > List_. In the **Status** field of the Filters, select a status to filter the list of item fulfillments. Select All, Picked, Packed, or Shipped.

The Fulfill Orders page lists all orders that have not yet had all items picked from inventory.

Note the following guidelines when fulfilling orders using the Pick, Pack, and Ship feature:

-   You can enable a preference to send a confirmation email showing the total quantity shipped upon fulfillment of orders. For more information, read [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html).
    
-   When you use the Pick, Pack and Ship feature, you can fulfill in one accounting period and ship in another. For details, read [Fulfilling Orders Across Multiple Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3997655525.html).
    
-   You cannot disable the Pick, Pack, and Ship feature when you have existing fulfillments in Picked or Packed status.
    

#### To fulfill (pick) an order using Pick, Pack, and Ship: {#procedure_N1230525}

1.  To pick the orders, go to _Shipping > Shipping > Fulfill Orders_.
    
2.  To filter the list of orders by customer, select a customer in the **Customer** field.
    
3.  In the **Process** column, click **Fulfill** next to the order you want to fulfill.
    
4.  On the Item Fulfillment page, verify or enter information in the following fields:
    
    -   **Customer** or **Project** - the customer or project for the sales order
        
    -   **Ref. No.** - the reference number to identify the fulfillment
        
    -   **Status** - the status assigned to the fulfillment when you save the record.
        
        The status defaults based on your setting for the Default Item Fulfillment Stage preference. Set this preference at _Setup > Accounting > Setup Tasks > Shipping_.
        
    -   **Date** - the date of the fulfillment.
        
5.  Click the **Items** subtab.
    
6.  Verify that items checked in the Fulfill column are the items you are actually picking.
    
7.  Verify or enter the quantities to pick for each item.
    
    If you want to pick the entire order, make sure the amount in the Quantity column equals the amount in the Remaining column for each item.
    
8.  Click the **Shipping** subtab.
    
9.  Verify or enter information under Shipping Address to show the customer address the order will be shipped to.
    
    Note:
    
    When picking an order, you cannot enter information on the Shipping or Packages subtabs unless you change the Status to Packed or Shipped.
    
10.  Click **Save**.
     

Now, the items you included in this fulfillment are marked Picked.

## Unpicking Items Already Picked {#bridgehead_1525085414}

If you have picked items to fulfill an order, but then need to 'unpick' or cancel the picking of the items, you must edit the item fulfillment record. To edit an item fulfillment, go to _Transactions > Sales > Fulfill Orders > Lists_, click **Edit** next the record you want to edit, and then do one of the following:

-   To unpick one or more items - but not all items - clear the **Fulfill** box next to each item, and then click **Save** to confirm the changes. The unpicked items are removed from the item fulfillment. You can continue to fulfill the other picked items.
    
-   To unpick all items, select **Delete** from the Actions menu. The item fulfillment record is deleted from the system.
    

### Related Topics:

-   [Pick, Pack, and Ship Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229796.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html)
-   [Commitment Settings for Reallocation of Picked or Packed Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0525105436.html)
-   [Marking an Order Packed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230849.html)
-   [Marking an Order Shipped](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231176.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
