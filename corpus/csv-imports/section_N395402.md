---
id: "section_N395402"
type: "section"
title: "Prerequisite Records for Cost Template Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Cost Template Import > Prerequisite Records for Cost Template Import"
parent: "section_N395199"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395402.html"
anchors: ["bridgehead_N395461", "bridgehead_N395666", "bridgehead_N395975"]
sha256: "6fd45936f351d6fbae5c7bb1df4ac39af601b565eab746e5edc246959044cedc"
---

When you create a cost template record, you rely on certain prerequisite records that must already exist in NetSuite. Specifically, you need at least one record of each of the following types:

-   [Cost Categories](#bridgehead_N395666)
    
-   [Charge Items](#bridgehead_N395975)
    

Before creating these records, you should also be familiar with the concept of [Cost Types](#bridgehead_N395461), which are classifications predefined by NetSuite.

## Cost Types {#bridgehead_N395461}

A cost type is a classification that distinguishes between general types of expenses, such as the cost of paying an employee versus the cost of operating a machine. NetSuite defines the following cost types for use with the manufacturing routing feature:

| 
-   Labor Setup

 | 

-   Labor Setup Overhead

 |
| --- | --- |
| 

-   Labor Run

 | 

-   Labor Run Overhead

 |
| 

-   Machine Setup

 | 

-   Machine Setup Overhead

 |
| 

-   Machine Run

 | 

-   Machine Run Overhead

 |

These cost types become available when you enable the Manufacturing Routing and Work Center feature (at _Setup > Company > Enable Features_, on the Items & Inventory subtab). After the feature is enabled, you can view the routing cost types on the page where you create cost category records.

## Cost Categories {#bridgehead_N395666}

A cost category is a record you create in NetSuite. It is an expense classification that belongs to a particular cost type. For example, you might create cost categories labeled US Labor Run Standard and Europe Labor Run Standard, each of which belongs to the cost type Labor Run. You create cost categories at _Setup > Accounting > Accounting Lists_ > Cost Categories.

To be valid for use on a cost template, a cost category must belong to one of the manufacturing routing cost types (as opposed to one of the other cost types that may be available).

When you select cost categories to use in your cost template, note the following restriction: In some cases, if two cost categories belong to the same cost type, only **one** of the categories may be allowed on the template. Whether this restriction applies is determined by the cost type, as described in the following table.

| Cost Type | Notes on Using Cost Categories of this Type |
| --- | --- |
| Labor Setup | Only one cost category using this cost type can appear on any cost template. |
| Labor Run | Only one cost category using this cost type can appear on any cost template. |
| Machine Setup | Only one cost category using this cost type can appear on any cost template. |
| Machine Run | Only one cost category using this cost type can appear on any cost template. |
| Labor Setup Overhead | Cost categories using this cost type can occur multiple times on a cost template. |
| Labor Run Overhead | Cost categories using this cost type can occur multiple times on a cost template. |
| Machine Setup Overhead | Cost categories using this cost type can occur multiple times on a cost template. |
| Machine Run Overhead | Cost categories using this cost type can occur multiple times on a cost template. |

For more on cost types and cost categories, see [Defining Cost Categories for Manufacturing Routing and Work Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2342063.html).

## Charge Items {#bridgehead_N395975}

Before you can begin importing cost templates, you must create charge items that reference your cost categories. A charge item is an item record that has been flagged as a Manufacturing Charge Item on the Purchasing subtab of the item record. Charge items include an exact monetary rate, and they must be associated with a cost category valid for use on a cost template.

You can manually create charge item records, or you can import them. To manually create a charge item, go to _Lists > Accounting > Items > New_, then choose an appropriate item type, such as Other Charge for Purchase. (Note that only certain item types can be flagged for use as a Manufacturing Charge Item.) When creating your charge items, make sure you select the Manufacturing Charge Item box or, if importing, map the field to a value of Yes.

For more on manually creating item records, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html). For more on item record import, see [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html).

### Related Topics

-   [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html)
-   [Cost Template Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N396186.html)
-   [Cost Template CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N398462.html)
-   [Common Errors When Importing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399710.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
