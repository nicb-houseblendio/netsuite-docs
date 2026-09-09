---
id: "section_N2242662"
type: "section"
title: "Special Order Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Special Order Items"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html"
anchors: ["bridgehead_4563461751"]
sha256: "6a95e75bb8b1687a5854f843da9144b68f5ac241bb314a8b334c1f2e98570a6c"
---

You can use special orders to purchase and track items that might not follow regular inventory processing. For example, just-in-time orders or orders for customized items.

Important:

If you change the base price on a special item record, the sales order and linked purchase order will be automatically updated. This may result in incorrect prices appearing on customer invoices.

If you sell items that are customized by your vendor, you can track custom item orders as special order items. Then, the sales order is not fulfilled with regular stock. It is fulfilled only when the linked order for the special item is received from the vendor. For example, an office supply retailer sells custom engraved signs. A customer places an order for a sign engraved with **Bob's Widget Service**. The retailer places the order with the sign vendor for the custom sign. The sales order cannot be fulfilled with regular stock. It is fulfilled only when the **Bob's Widget Service** sign is received from the vendor.

Using special orders to process just-in-time orders also lets you sell expensive items without having to maintain expensive stock. For example, you offer your customers a high-end item that you order from your vendor only when you need to fill a sales order. This process helps you reduce your overhead.

You can special order any inventory items and non-inventory for resale items. Items can be tagged as special orders in two ways:

-   Marking the item when you create the sales order
    
-   Tagging the item record
    

Note:

You must identify a preferred vendor and a purchase price on an item record for that item to be selected as a special order.

For example, you tag an item as a special order on the item record. When you save or approve a sales transaction that contains the item, a purchase order is created that is linked to the sale. The form used for special orders is your preferred purchase order form. Purchase orders for special orders contain a **Created From** link that opens the original sales order.

A special order inventory item can be fulfilled only when the linked purchase order is received. When the linked purchase order is received, the item is committed and the sales order appears in the picking ticket queue. Then, the item can be fulfilled.

This fulfillment workflow applies only to inventory items. Non-inventory items are not committed and can be fulfilled without receiving a purchase order.

Special Orders are a function of the Drop Shipments and Special Orders feature. After you enable the feature, an item can be either a drop ship or special order, but not both.

Note:

Unlike drop shipments, special orders **are** received into your inventory and **do** impact assets and inventory costing. Receiving a special order item increases the value of the item's asset account. Selling it increases the value in its Cost of Goods Sold (COGS) account.

The following table explains the differences between special order and drop ship items:

| Function | Drop Shipment | Special Order |
| --- | --- | --- |
| Sales revenue tracked in NetSuite | YES | YES |
| Purchase order form | Drop Ship PO form | Preferred PO form |
| P.O. links to sale | YES | YES |
| Vendor ships to | your customer's address | your company's address |
| Inventory impact | None-when it is not received into inventory | Impacts Asset and Cost of Goods Sold (COGS) accounts upon receipt and fulfillment |
| Item commitment | **Drop shipments do not commit.** Drop ship items don't show as a committed quantity in the linked Sales Order transaction. The item can commit only through steps in the process of manually receiving it instead of clicking the Mark Shipped button on the order. Then, after you receive the item, it is no longer considered a drop shipment and the item is treated as inventory. | A special order item always commits upon receipt of the linked PO-it **is not** committed from stock on hand. Lines marked as special order commit only from the linked purchase order. To commit non-special order stock items to an order, those items must be entered on a separate line and not marked as a special order. |
| Can be used for inventory items and non-inventory for resale items | YES | YES |
| Item record can default to this method | YES | YES |
| Item Fulfillment | Can be marked as fulfilled before or after the linked purchase order has been received. | Can be fulfilled only after the linked purchase order has been received. |

## Special Order Items and Assemblies {#bridgehead_4563461751}

You enter a sales order and an assembly component is identified as a special order item on its item record. NetSuite generates a special order for the item, unless the assembly item is being special ordered as a Special Order Work Order Item.

Note:

This workflow is specific to you special ordering a component, and then building the assembly after the special ordered component has been received. For more information, see [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html).

### Related Topics

-   [Enabling Drop Shipments and Special Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244482.html)
-   [Identifying Special Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244641.html)
-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
-   [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)
-   [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html)
-   [Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2247990.html)
-   [Service Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248153.html)
-   [Download Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248348.html)
-   [Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html)
-   [Subtotal Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248793.html)
-   [Description Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248894.html)
-   [Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248975.html)
-   [Expense Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4042372470.html)
-   [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html)
-   [Other Charge Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249208.html)
-   [Payment Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249363.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
