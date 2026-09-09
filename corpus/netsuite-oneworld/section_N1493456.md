---
id: "section_N1493456"
type: "section"
title: "Intercompany Inventory Drop Ship"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Managing Intercompany Inventory Transfers - Arm's Length > Intercompany Inventory Drop Ship"
parent: "section_N1492766"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html"
anchors: ["svg_1", "svg_1Node", "svg_1Node_1_", "svg_1Bendy_Thin", "svg_1Bendy_Thin_1_", "svg_1Node_2_"]
sha256: "5c972b29042a29bf31cca806066dbc5d1766c2229561af81de7cf411cf96c86c"
---

You can use Automated Intercompany Management to manage intercompany inventory drop ship orders. With the intercompany inventory drop ship order, one subsidiary sells an inventory item to an external customer and a different subsidiary fulfills the order. See [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html).

Important:

If you use the Intercompany Cross-Subsidiary Fulfillment feature, the system uses the Intercompany Cost of Goods Sold account when you fulfill an external item. You must manually set the account to the regular COGS account. For information about the Intercompany Cross-Subsidiary Fulfillment feature, see [Intercompany Cross-Subsidiary Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515621767.html).

To manage intercompany drop ship orders, you must enable Automated Intercompany Drop Ship. Go to _Setup > Company > Enable Features_. Click the Accounting subtab. The following features are also required to use the Intercompany Drop Ship feature:

-   Automated Intercompany Management
    
-   Drop Shipments & Special Orders
    
-   Advanced Shipping
    
-   Advanced Receiving
    

When you enable the Automated Intercompany Drop Ship feature, NetSuite automatically sets the following accounting preferences. Go to _Setup > Accounting > Preferences > Accounting Preferences_. These preferences are on the Order Management subtab, under Drop Shipments. The intercompany drop ship workflow must have these preferences to properly function. You can't change these preferences.

-   **Update Drop Ship Order Quantities Automatically Prior to Shipment** - The quantities, prices, and amounts on linked transactions for intercompany drop ship orders must match.
    
-   **Drop Ship Fulfillment Quantity Validation** - set to **Do not allow unequal quantities**. This preference enforces matching quantities for intercompany drop ship transactions.
    
-   **Allow Both Mark Shipped Fulfillments and Receipts on a Drop Shipment Line** - set to **Do not allow**. For intercompany drop ship orders, you must mark the order the sales subsidiary as shipped (dummy fulfillment).
    

The workflow for intercompany drop ship orders follows these steps:

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               

1.  Sales subsidiary creates a sales order for an external customer, and specifies an intercompany vendor that represents the warehouse subsidiary.
    
2.  Sales subsidiary creates an intercompany purchase order for the sale with an intercompany vendor that represents the warehouse subsidiary.
    
3.  Warehouse subsidiary generates an intercompany sales order through the Manage Intercompany Sales Orders page. Go to _Transactions > Sales > Manage Intercompany Sales Orders_.
    
4.  Warehouse subsidiary fulfills the order and sends the item to the external customer.
    
5.  Warehouse subsidiary creates an intercompany sales invoice, and bills the Sales subsidiary. This intercompany sales invoice debits Intercompany A/R and credits Intercompany Revenue.
    
6.  Sales subsidiary marks the external sales order as shipped, and creates a dummy item fulfillment, completing the order.
    
7.  Sales subsidiary bills the intercompany purchase order. This intercompany vendor bill debits Intercompany Dropship Expense and credits Intercompany A/P.
    
8.  Sales subsidiary invoices the external customer for the item shipped.
    

For information about the general ledger impact for the posting transactions involved in intercompany drop ship orders, see [Intercompany Drop Ship Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html#bridgehead_N1497553).

Note:

NetSuite doesn't support returns for intercompany drop-ship orders. You must complete the following:

\* Create a standalone return authorization between the external customer and the purchasing subsidiary.

\* Create an intercompany transfer order between the purchasing subsidiary and the selling subsidiary. See [Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493092.html).

### Related Topics:

-   [Intercompany Inventory Returns - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493277.html)
-   [Intercompany Inventory Transfer Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html)
-   [Intercompany Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498276.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
