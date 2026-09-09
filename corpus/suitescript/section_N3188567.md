---
id: "section_N3188567"
type: "section"
title: "Using Item Records in SuiteScript"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Items > Using Item Records in SuiteScript"
parent: "chapter_N3188218"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3188567.html"
anchors: ["bridgehead_N3188614", "bridgehead_N3188663", "bridgehead_158514045026", "bridgehead_4544338063"]
sha256: "102fe98bf78c09b18f46d14123504df1a33123d79549cc530d21ae0c3a93b799"
---

This section includes the following topics:

-   [Loading Item Types](#bridgehead_N3188614)
    
-   [Filtering Items by Type](#bridgehead_N3188663)
    
-   [Looking Up the Subsidiary Field](#bridgehead_158514045026)
    
-   [Advanced Revenue Management Scripting with Items](#bridgehead_4544338063)
    

For information about working with items in the UI, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html) and [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html).

## Loading Item Types {#bridgehead_N3188614}

When using [record.load(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258486.html), you can:

-   set the type parameter to record.Type.INVENTORY\_ITEM to load the following types of item records: inventoryitem, lotnumberedinventoryitem, serializedinventoryitem
    
-   set the type parameter to record.Type.ASSEMBLY\_ITEM to load the following types of item records: assemblyitem, lotnumberedassemblyitem, serializedassemblyitem
    

## Filtering Items by Type {#bridgehead_N3188663}

The following are valid search filter item type IDs. Note that the item filter IDs are case-sensitive.

| Item Type IDs |
| --- |
| Assembly Description Discount DwnLdItem EndGroup GiftCert Group InvtPart Kit | Markup NonInvtPart OthCharge Payment Service ShipItem Subtotal TaxGroup TaxItem |

To use these IDs:

1.  Create a script that will search for items of a specific type or types (for example, search for all non-inventory items).
    
2.  Next, see any of the valid SuiteScript item type IDs.
    

**Sample Code**

          `//Create a script that will search for all non-inventory part items function searchnoninventorypart() {     var searchType = search.Type.NON_INVENTORY_ITEM;     var mySearch = search.create({         type: searchType,         columns: [{             name: 'internalId'         }],         filters: [{             name: ' ',             operator: search.Operator.ANYOF,              values: 'NonInvtPart'         }]     }); }` 
        

## Looking Up the Subsidiary Field {#bridgehead_158514045026}

The [search.lookupFields(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345776651.html) method lets you retrieve the current value of a field on a record. Usually, single select fields are returned as an object with `value` and `text` properties. Multiselect fields are returned as an object with a set of `value`: `text` pairs.

The `subsidiary` field on an item record is a multiselect field. However, when you use [search.lookupFields(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345776651.html) to retrieve the value of this field, the field is returned as a single `value`: `text` pair instead of a set of pairs. The returned `value`: `text` pair represents the first subsidiary in the list.

## Advanced Revenue Management Scripting with Items {#bridgehead_4544338063}

The item record (internal ID `item`) contains several additional accounting fields associated with the Advanced Revenue Management (Essentials) and Advanced Revenue Management (Revenue Allocation) features. The following table lists these scriptable fields.

| **Field** | **Type** | **Internal ID** |
| --- | --- | --- |
| Create Revenue Plans On | List/Record | `createrevenueplanson` |
| Item Revenue Category | List/Record | `itemrevenuecategory` |
| Revenue Allocation Group | List/Record | `revenueallocationgroup` |
| Revenue Recognition Rule | List/Record | `revenuerecognitionrule` |

The **Item Revenue Category** and **Revenue Allocation Group** fields appear only when the Advanced Revenue Management (Revenue Allocation) feature is enabled.

Before you begin working with advanced revenue management programmatically, see [Setup for Advanced Revenue Management (Essentials)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4328435754.html) and [Setup for Advanced Revenue Management (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0627115526.html).

For help working with this record in the UI, see [Item Configuration for Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4340443927.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
