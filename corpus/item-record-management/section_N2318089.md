---
id: "section_N2318089"
type: "section"
title: "Groups, Assemblies, and Kit/Packages"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Groups, Assemblies, and Kit/Packages"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html"
anchors: ["bridgehead_N2318108", "bridgehead_N2318216", "bridgehead_N2318417", "subsect_163301236648"]
sha256: "b88b5a2d848e3f388aecdabe5619cda2b4e41872ad9c615c2221392e6af6d4c5"
---

Groups, assemblies, and kit/packages are all item types that combine multiple items together to sell. The information below helps distinguish each of the item types so you understand the differences between them and the uses for each.

Note:

Depending on the NetSuite product you subscribe to, some item types might not be available for you to use. If you have questions about the availability of the item types, please contact your account representative.

## Item Groups {#bridgehead_N2318108}

An item group is sold as one unit, but has several member components from your inventory. Item groups can be inventory items, assemblies, kits, and service items.

When the retailer sells a quantity of the group, the stock level of each member item decreases by that quantity. You can track sales of the group and stock of the items it contains. For more information, see [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html).

The price of a group item **is dependent** on its members' prices. Each of the group's members has a price determined on its item record. The price of the members are totaled to calculate the price for the group.

Selling item groups can help streamline your inventory workflow because it saves time creating sales transactions. You can create groups for items that you frequently sell together, then you can enter them on sales as one unit.

## Assembly Items {#bridgehead_N2318216}

An assembly item is an inventory item made of several components, but identified as a single item. Assemblies are manufactured by combining raw materials you stock.

You create an assembly item record to define the members of an assembly. Then, NetSuite tracks stock separately for the assembly item and for each member component.

When you physically manufacture assemblies in a production run, you increase your stock of the assembled items. Record each production run and update stock levels by entering an assembly build.

For each assembly build you record:

-   the assembly item stock level increases
    
-   the member items' individual stock levels decrease
    

After an assembly item is built, it is processed like an individual inventory item for tracking inventory costs. The asset/costing value of each built assembly item can be the total value of the assembly's member items. It can also be another value that you assign on the item record. This value functions like the assembly item's purchase price for inventory costing calculations.

You can also unbuild assemblies to increase your inventory of raw materials.

For more information about assembly items, see [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html).

If you use the **Allow Purchase of Assembly Items** preference, you can add an assembly item to a purchase order. This is useful if you sometimes purchase the item already assembled. For more information about this preference, see the [Items/Transactions Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html) section of [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html).

## Kit/Package Items {#bridgehead_N2318417}

A kit/package is a unit composed of items from your inventory. A kit is sold as one unit, but has several member components. Kit components can be inventory items, assemblies, kits, and service items.

One difference between kits and groups is that the price of a kit **is not dependent** on its components' prices. It can also be assigned several price levels. Each time a kit is sold, inventory records are updated for the individual members of the kit.

To learn more, see [Handling Inventory Items with Alias SKU](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162563797748.html).

## Key Differences Between Kits, Groups, and Assemblies {#subsect_163301236648}

Although they are similar, there are key differences between kits, groups, and assemblies. The chart below explains these differences.

| Function | Assembly | Kit/Package | Item Group |
| --- | --- | --- | --- |
| Members can include: | Inventory items non-inventory items assemblies service items other charges | Inventory items non-inventory items assemblies kits service items | Inventory items non-inventory items assemblies kits service items |
| Pricing: | Item price is **independent** of its members' prices | Item price is **independent** of its members' prices | Item price is **dependent** on its members' prices |
| General Ledger Accounts: | Able to identify a Cost of Goods Sold (COGS), income, and asset account separate from its components' accounts | Able to identify a separate income account | No account designation available |
| Inventory Impact: | Building an assembly: Decreases the asset accounts of member items Increases asset account of the assembly | Fulfilling a kit: Decreases the asset account of member items | Fulfilling a group: Decreases the asset account of member items |

### Related Topics

-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)
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
