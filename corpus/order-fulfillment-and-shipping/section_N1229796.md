---
id: "section_N1229796"
type: "section"
title: "Pick, Pack, and Ship Overview"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Pick, Pack, and Ship > Pick, Pack, and Ship Overview"
parent: "section_N1229691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229796.html"
anchors: []
sha256: "4c19c8eae893181ea4fdb787119be7768dac2b11b67e9ee69e1ae63535ec286d"
---

The Pick, Pack, and Ship feature allows greater flexibility to process and track the status of orders through the fulfillment and shipment processes. You use separate transactions to pick the items from inventory, pack the items to prepare them to be shipped, and then ship the items to their destination.

Using Pick, Pack and Ship, you can send items to your customers or to your other locations, if you use the Multi-Location Inventory feature. For details, read [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html).

When the Pick, Pack, and Ship feature is activated, orders are fulfilled in three stages: Fulfill Orders (Pick), Mark Orders Packed and Mark Orders Shipped.

When you fulfill an order, you pick the items from inventory in the warehouse that you need to fill the order. Mark the order packed when you physically package them to be ready to ship. Finally, you mark orders shipped when the order is on the way to its destination.

You can track orders through each step of the fulfillment process. Possible statuses for a fulfillment are:

-   **Picked** - The items on the order have been picked from inventory and are waiting to be packed and shipped.
    
    This is a non-posting transaction.
    
-   **Packed** - The items on the order have been packed and are waiting to be shipped.
    
    This is a non-posting transaction.
    
-   **Shipped** - The items have been shipped out, and the order is completely fulfilled.
    
    This is a posting transaction.
    

To view a list of item fulfillments and their statuses, go to _Shipping > Shipping > Fulfill Orders > List_. In the Status field of the footer, filter the list by type of status for fulfillments you want to see. Select All, Picked, Packed or Shipped.

Select a Default Item Fulfillment Stage at _Setup > Accounting > Setup Tasks > Shipping_. The default status populates the Status field on new item fulfillments, as well as in the Set Shipment Status To field on the Bulk Fulfill Orders page.

For other related preferences or settings, see [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html) or [Commitment Settings for Reallocation of Picked or Packed Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0525105436.html).

It is possible for one order to be partially picked, partially packed and partially shipped, so an order may have several fulfillments, each with a different status.

For example, an order with six items is picked in two fulfillments:

-   First fulfillment - items #1 - 3 are picked and awaiting packing.
    
-   Second fulfillment - items #4 - 6 are picked, packed, and shipped out.
    
    The first fulfillment has a status of Picked.
    
    The second fulfillment has a status of Shipped.
    

### Related Topics:

-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html)
-   [Fulfilling Orders Using Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230473.html)
-   [Marking an Order Packed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230849.html)
-   [Marking an Order Shipped](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231176.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
