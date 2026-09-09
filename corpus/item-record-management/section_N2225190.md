---
id: "section_N2225190"
type: "section"
title: "Kit/Package Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Kit/Package Items"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html"
anchors: []
sha256: "ba3de7087df7785cce9728a193680b891720be8970767efc63a03ea617f12791"
---

Kits or packages let you create individually-sold items that are collected from other items.

-   Add description, inventory, non-inventory, other charge, service, kit, gift certificates, and assembly items to your kits or packages.
    
-   The price of a kit isn't dependent on its components' prices and can be assigned several price levels.
    
-   Assign multiple price levels to your kits and make them available in your website.
    
-   Partially fulfilled Kit/Package items display a quantity of zero (0) on printed invoices.
    

For example, the electronics retailer creates the kit Creativo 2400 Graphics Bundle. They want to give customers an incentive to buy the entire kit, rather than some of the components. The price based on the component prices is $2783.99. Because a kit does not have to be based on the component prices, the retailer can set the price of the kit at $2730.00.

Important:

When member items use bins, serial, or lot numbers, NetSuite displays the member items and quantity when the sales order is saved on shipment. When the sales order fulfillment is saved, NetSuite retrieves the current kit member item definition and then uses that value for the fulfillment. If any bin, serial, or lot number items have been added or removed from the kit, NetSuite presents a mismatch error. You must edit and save the sales order. You can also use the special mass update to force the new kit member definition quantity into the open sales order. If you use Advanced Bins, NetSuite validates that the new kit member definition quantities match what displays in the user interface. If the quantities don't match, NetSuite presents the mismatch error.

Note:

If a Kit/Package item includes a member that uses bins, you can't create a standalone invoice or cash sale for it. For these kits, first enter a sales order for the kit and then fulfill the order. After the sales order is fulfilled, you can create an invoice or cash sale from the sales order or fulfillment.

A kit sale posts revenue for the kit only, it doesn't post revenue for each component. Therefore, sales revenue appears on inventory reports for the kit, not the components. Kit sales revenue can be evaluated using the Inventory Activity Detail report or the Sales by Item Summary or Detail reports. For more information about kit items and revenue recognition, see [Auto-Expansion of Kit Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4677544043.html).

Important:

Kit/Package item inventory isn't tracked by the kit, it is tracked by individual component members. The Kit/Package item record can't display an available quantity for these items.

Kits and their components cannot be set to Do Not Commit. For more information, see [Committing Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3765928460.html).

Tip:

To edit a kit, go to _Lists > Accounting > Items_. Click **Edit** next to the kit name.

To show member items pages, on the **Purchasing/Inventory** subtab, check the **Display Components on Transactions** box.

### Related Topics

-   [Entering Serial and Lot Components on the Item Record for the Kit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225398.html)
-   [Updating Kits with Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225728.html)
-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
-   [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)
-   [Special Order Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html)
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
