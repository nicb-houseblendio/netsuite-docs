---
id: "section_N2312623"
type: "section"
title: "Pick, Pack, and Ship with Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Pick, Pack, and Ship with Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html"
anchors: ["bridgehead_4661069107"]
sha256: "2a72ffd828f4316efc559b476677e169248e8b0b1eeba75c2e9b2226a67845fd"
---

You can also use the Pick, Pack, and Ship feature to assist with processing transfer orders.

The Pick, Pack, and Ship feature gives your warehouse and shipping departments separate processes for each step to fulfill orders. This enables greater flexibility in processing and tracking the status of orders through the fulfillment and shipment processes.

For example, a warehouse manager uses individual steps to process each fulfillment. One employee picks the items off the shelves and another employee boxes them up and ships them. To know which orders are at which stage, he needs to mark each order for each step in the process.

The Pick, Pack, and Ship feature enables him to show each step separately for each order. The first employee pulls the items and marks them as fulfilled (picked). The second employee boxes the items and marks them as packed. He then ships the package and marks the order as shipped.

You use separate transactions for each step:

-   to pick the items from inventory (Fulfill Orders)
    
-   to pack the items to prepare them to be shipped (Mark Orders Packed)
    
-   to ship the items to the receiver (Mark Orders Shipped)
    

For more information about enabling and using this feature, read [Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229691.html).

Note:

Lines on transfer orders cannot be partially picked, packed or shipped. The entire line must be processed at one time. Also, you cannot pick, pack or ship more than the quantity on the transfer order.

## Transfer Order Pick, Pack or Ship Quantities {#bridgehead_4661069107}

You cannot pick, pack or ship more than the quantity on the transfer order.

Lines on transfer orders cannot be partially picked, packed or shipped unless the Use Item Cost as Transfer Cost preference is enabled for that transfer order. For details about this preference, read [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html) and [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

When you partially pick, pack or ship a transfer order quantity, you are required to match the fulfillment when it is received to process item costing accurately.

### Related Topics

-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
