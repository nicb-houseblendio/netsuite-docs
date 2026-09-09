---
id: "section_N2316558"
type: "section"
title: "Closing Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Closing Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html"
anchors: ["bridgehead_N2316619", "bridgehead_N2316700"]
sha256: "56aafc249f2c9a7abbf81831d02e43525707460dcfb8b841d437f0e9f2a183b1"
---

On transfer orders, you are able to close line items manually when you do not intend to transfer open items on the order.

For example, you enter a transfer order for ten widgets and have already transferred five of them. The warehouse manager informs you that the remaining five cannot be located to be transferred. If you close the line manually instead of changing the quantity, you retain a record of how many you originally planned to transfer.

Note:

A line on a transfer order can be closed only if the in-transit quantity is zero.

Transfer order lines can be closed in two ways:

-   [To close individual lines on an order:](#bridgehead_N2316619)
    
-   [To close all lines on an order at one time:](#bridgehead_N2316700)
    

#### To close individual lines on an order: {#bridgehead_N2316619}

1.  Go to _Transactions > Inventory > Enter Transfer Orders > List_.
    
2.  Click **Edit** next to the order.
    
3.  On the **Items** subtab, each item line shows a box in the **Closed** column. Check the **Closed** box to close that line without transferring the item.
    
4.  Click **Save**.
    

#### To close all lines on an order at one time: {#bridgehead_N2316700}

1.  Go to _Transactions > Inventory > Enter Transfer Orders > List_.
    
2.  Click **View** next to the order.
    
3.  Click **Close Order**.
    
    This button shows only if the in-transit quantity is zero for all lines.
    

The order now shows the quantities that have been closed and has a transaction status of Closed.

After a line on a transfer order is closed, you cannot do the following:

-   change the item receipt quantity
    
-   create a new item receipt that links to the transfer order
    
-   delete an existing item receipt that links to the transfer order
    

### Related Topics

-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
