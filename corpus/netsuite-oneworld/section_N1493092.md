---
id: "section_N1493092"
type: "section"
title: "Intercompany Inventory Transfers - Arm's Length"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Managing Intercompany Inventory Transfers - Arm's Length > Intercompany Inventory Transfers - Arm's Length"
parent: "section_N1492766"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493092.html"
anchors: ["svg_1", "svg_1Node", "svg_1Node_1_", "svg_1Bendy_Thin"]
sha256: "3513844b92e7a624dc5a26e6a8ab8d3dc62620238b2ceabeffc21c06bfbd5315"
---

Intercompany inventory transfers begin with the creation of an intercompany purchase order. Subsidiaries are the trading entities for the inventory transfer. You must create intercompany customers and vendors to represent the subsidiaries involved in the transaction. See [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html).

The purchasing subsidiary is the destination for the transfer. The selling subsidiary is the source for the transfer. All intercompany transactions related to the inventory transfer must be in the base currency of the purchasing subsidiary (destination). Inventory items must be accessible by both subsidiaries involved with the transfer.

The workflow for intercompany inventory transfers involves the following steps.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       

1.  Destination subsidiary creates an intercompany purchase order.
    
2.  Source subsidiary generates an intercompany sales order through the Manage Intercompany Sales Orders page. Go to _Transactions > Sales > Manage Intercompany Sales Orders_.
    
3.  Source subsidiary fulfills the order and creates an item fulfillment.
    
4.  Destination subsidiary receives the order and creates an item receipt. The quantity received can't be greater than the quantity shipped.
    
5.  After the order is fulfilled and received, subsidiaries can generate the vendor bills and invoices.
    
6.  At period end, run the intercompany elimination process to automatically revalue inventory and inventory costing balances.
    

Important:

For arm's length intercompany inventory transfer, do **not** mark the COGS account as Elimination.

For information about the general ledger impact for the posting transactions involved in arm's length intercompany inventory transfers, see [Arm's Length Intercompany Inventory Transfer Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html#bridgehead_N1493770).

### Related Topics:

-   [Intercompany Inventory Returns - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493277.html)
-   [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html)
-   [Intercompany Inventory Transfer Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html)
-   [Intercompany Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498276.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
