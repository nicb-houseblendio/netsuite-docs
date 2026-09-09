---
id: "section_N2312176"
type: "section"
title: "Fulfilling Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Fulfilling Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html"
anchors: ["bridgehead_4661045572", "bridgehead_4661045834", "bridgehead_N2312338"]
sha256: "48876cf5d60454b873fa297517884e6774709ee01b8b3397bc3545e5248b6abf"
---

After a transfer order is entered, and approved if required, the order can be fulfilled. Fulfillment is the process of taking items out of inventory in one location and shipping the items to a second location.

For example, an approved transfer order for 50 widgets shows in the fulfillment queue for the warehouse at Location A. The transfer order shows that the widgets must be shipped to Location B. The warehouse supervisor pulls 50 widgets from inventory, packages them to be shipped and ships them out. Then, the manager marks the transfer order as fulfilled.

By default, item fulfillments show the same department and class entered on the transfer order.

If a transfer order includes a serialized or lot numbered item, the serial or lot numbers may not have been added when the transfer order was first entered. In this case, you must enter them in the **Serial/Lot Numbers** field for the item line on the fulfillment form.

Note:

If you tend to reallocate or partially fulfill orders, you should include lot or serial numbers in transfer orders to avoid quantity discrepancies. You can also enable settings or preferences depending on the features you use. For more information, see [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html).

After a transfer order is fulfilled, it has a status of Pending Receipt when the items are in transit between locations. This means the items have shipped out of the source location, but not yet been received into the receiving location.

When items are in transit, changes can no longer be made to the transfer order for values in the **Item**, **Quantity**, or **Location** fields.

You can fulfill a transfer order in the following ways:

-   Fulfill multiple transfer orders by going to _Transactions > Sales > Fulfill Orders_. In the **Transaction Type** field, select **Transfer Order**.
    
-   Fulfill a single transfer order by going to _Transactions > Inventory > Enter Transfer Orders > List_ and clicking **View** next to the order. On the transfer order page, click the **Fulfill** button.
    

For more details, read [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html).

## Transfer Order Fulfillment Quantities {#bridgehead_4661045572}

You cannot fulfill more than the quantity on the transfer order.

Lines on transfer orders cannot be partially fulfilled unless the **Use Item Cost as Transfer Cost** setting is enabled for that transfer order. For details about this setting or preference, read [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html) and [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

When you partially fulfill a transfer order quantity, you are required to match the fulfillment when it is received to process item costing accurately. For more information, see [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html).

## Transfer Order Fulfillment Status {#bridgehead_4661045834}

After you create a transfer order, the **Status** field is updated to show one of the following processing statuses:

-   **Pending Approval** - The transfer order is entered but not yet approved. Items on the order are not yet committed to be transferred.
    
-   **Pending Fulfillment** - The order is approved and ready to be fulfilled for transfer. Items on the order are now committed to be transferred.
    
-   **Pending Receipt** - Items are in transit between locations. They have shipped out of the source location, but not yet been received into the receiving location.
    
    Note:
    
    Items in this status are counted with the inventory of the source location.
    
-   **Received** - Items have been received into the destination location. These items are now counted with the on-hand inventory for the destination location.
    
-   **Rejected** - This transfer order has not been approved and is cancelled.
    

For more details on fulfilling orders, read [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html).

## Transfer Order Fulfillment and Commitment {#bridgehead_N2312338}

You can choose how to process transfer order fulfillments based on item commitment. On the preference Fulfill Based on Commitment, your selection determines how the fulfillment form works:

-   **Ignore Commitment** - The quantity field is disabled on the fulfillment.
    
-   **Allow Uncommitted** - The partially committed lines are displayed on the fulfillment form with the committed quantities. To fulfill the partially committed lines, you must manually adjust the quantity being fulfilled to be equal to the order line quantity.
    
-   **Limit to Committed** - The Fulfill button does not show on an order if it has no lines that are fully committed. When you click Fulfill on a transfer order, only fully committed lines show on the fulfillment form.
    

For details about setting preferences, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
