---
id: "section_N1493277"
type: "section"
title: "Intercompany Inventory Returns - Arm's Length"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Managing Intercompany Inventory Transfers - Arm's Length > Intercompany Inventory Returns - Arm's Length"
parent: "section_N1492766"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493277.html"
anchors: ["svg_1", "svg_1Background", "svg_1Node", "svg_1Node_1_", "svg_1Bendy_Thin"]
sha256: "f40aa5b5c26f0c7696d58eff6be9f667f32ab41b32b89740915bd46e79b71de7"
---

The return process for an intercompany inventory transfer reverses the original transfer transaction. It originates when the subsidiary that purchased the item (the original destination subsidiary) creates a vendor return authorization for the original purchase order. The original source subsidiary (the subsidiary that sold the item) can't create a credit memo to initiate the return of an intercompany inventory transfer. Instead, the source subsidiary automatically generates a return authorization for the vendor return authorization. Then, each subsidiary completes their part of the return process. **NetSuite doesn't process changes made to any line item.**

The transaction currency for the return is the base currency of the vendor return authorization. The currency for the return authorization matches the currency for the vendor return authorization. It is the same currency used for the paired intercompany sales order and purchase order for the original inventory transfer.

You can't manually create a vendor return for an intercompany inventory transfer order.

The workflow for arm's length inventory returns involves the following steps. In this diagram, the Destination Subsidiary is the subsidiary that originally ordered the item. The Source Subsidiary is the subsidiary that originally shipped the item.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           

1.  Destination subsidiary, the subsidiary that initially purchased the item, creates an intercompany vendor return authorization to return an item.
    
2.  Source subsidiary generates an intercompany return authorization through the Manage Intercompany Return Authorizations page. Go to _Transactions > Customers > Manage Intercompany Return Authorizations_.
    
3.  Destination subsidiary fulfills the vendor return and creates an item fulfillment.
    
4.  Source subsidiary receives the order and creates an item receipt. The quantity received can't be greater than the quantity shipped.
    
5.  After the return is fulfilled and received, the subsidiaries can generate the credit memo and vendor credit.
    
6.  At period end, run the intercompany elimination process to automatically revalue inventory and inventory costing balances.
    

For information about the general ledger impact for the posting transactions involved in an intercompany inventory return, see [Arm's Length Intercompany Inventory Return Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html#bridgehead_N1496683).

Note:

NetSuite doesn't support returns for intercompany drop-ship orders. You must complete the following:

\* Create a standalone return authorization between the external customer and the purchasing subsidiary.

\* Create an intercompany transfer order between the purchasing subsidiary and the selling subsidiary. See [Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493092.html).

### Related Topics:

-   [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html)
-   [Intercompany Inventory Transfer Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html)
-   [Intercompany Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498276.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
