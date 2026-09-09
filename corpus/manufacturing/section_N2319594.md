---
id: "section_N2319594"
type: "section"
title: "Assembly Item Records"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Items > Assembly Item Records"
parent: "chapter_N2319010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319594.html"
anchors: ["bridgehead_N2319618", "bridgehead_N2319920", "bridgehead_N2319942"]
sha256: "973e858878ad8d8a7bf6d518c30150578915af0251b226f2be72836e066a4553"
---

You can create an assembly item record to track each assembly and its component items. The assembly record details member items and the quantity of each member required for each assembly. For more information, see [Building Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321340.html).

Important:

With the release of NetSuite 2023.1 Bills of Materials, where components are embedded to an Assembly Item, will no longer be supported. Only business critical issues will be fixed. To continue working with this functionality you should transition to the [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html) feature, which is free of charge. After you enable this feature, NetSuite will automatically migrate all of your Bill of Materials to the new structure.

## Available Member Items {#bridgehead_N2319618}

The following table displays the available member item types:

| Regular Inventory Assembly | Serial or Lot Numbered Inventory |
| --- | --- |
| Inventory | Inventory |
| Non-Inventory | Serialized Inventory |
| Other Charge | Lot Numbered Inventory |
| Service | Non-Inventory |
| Regular Assemblies | Other Charge |
| Kit Items | Service |
|  | Regular Assemblies |
|  | Serialized Assemblies |
|  | Lot Numbered Assemblies |

## Assembly Items in Item Lists {#bridgehead_N2319920}

To make an inventory item available in your assembly build but not for sale, don't choose an income account on the item record.

By not setting an income account on an inventory item's record, the item doesn't appear in the sales transaction's items list. The item is sold as part of the finished goods assembly the item belongs to, which has its own income account.

If you don't set an expense account on a non-inventory item for resale, the item doesn't appear in the purchase transaction's item list.

## Assemblies and Serial/Lot Numbered Members {#bridgehead_N2319942}

Serialized and lot numbered items cannot be included as member items in a regular assembly item.

-   A non-serialized assembly cannot include a serialized or lot numbered member item.
    
-   A non-lot numbered assembly cannot include a serialized or lot numbered member item.
    

Serialized or lot numbered inventory items can be members of an assembly only if the assembly is serialized or lot numbered.

-   A serialized assembly can include a serialized or lot numbered member item.
    
-   A lot numbered assembly can include a serialized or lot numbered member item.
    

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Enabling Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319428.html)
-   [Assemblies on Purchase Transactions, Web Sites, and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161487042976.html)
-   [Matrix Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4249789892.html)
-   [Phantom Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4714298883.html)
-   [Assemblies and Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2320172.html)
-   [Building Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321340.html)
-   [Unbuilding Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321882.html)
-   [Marking Work Orders Built](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2322811.html)
-   [Printing an Item Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323540.html)
-   [Bill of Materials Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324073.html)
-   [Costed Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160730538.html)
-   [Printing Assembly Item Materials on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324339.html)
-   [Printing Assembly Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324547.html)
-   [Running the Component Where Used Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511882961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
