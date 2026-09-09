---
id: "section_N417879"
type: "section"
title: "Item Supply Plan Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Supply Plan Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N417879.html"
anchors: ["bridgehead_N417982"]
sha256: "7472343dd44c6e25f965b0e76338da781fa6b1414106da6b955ba63b5dcb5193"
---

An item supply plan lists the purchase orders or work orders required to ensure that item quantity meets expected demand. You can import item supply plan data from another system into NetSuite. You need to get the required data into a CSV file, then you can use the Import Assistant to create new supply plans and edit existing supply plans.

Importing item supply plan data is similar to creating a manual item supply plan in the NetSuite user interface. This item supply plan type isn't derived from any demand plan in the NetSuite system and can be based on data or projections from external sources.

Important:

Only one item supply plan per item is supported.

The item supply plan data that you can import generally matches the fields available at _Transactions > Demand Planning > Item Supply Plans > New_. If you're not familiar with this page, you should review it to get an understanding of the fields that you should include in your Item Supply Plan CSV files.

Each item supply plan includes two types of fields:

-   Body fields used to identify the record, such as ExternalId, Internal ID, Item, Location (when Multi-Location Inventory is enabled), Memo, Subsidiary (for NetSuite OneWorld), and Unit of Measure (when Multiple Units of Measure is enabled).
    
    You must provide ExternalId or Internal ID values to uniquely identify items, because the Item field may have non-unique values.
    
-   Orders sublist fields that define data for the orders needed to replenish the supply of items. These fields include:
    
    -   Order Date (required)
        
    -   Order Line - optionally can be used to identify orders
        
    -   Order Type - the type of order; always purchase order for inventory items, can be purchase order or work order for assembly/BOM items
        
        Although an Order Type value is required for each line item, it's not required to be mapped for imports, because its values may be determined by the selected item.
        
    -   Quantity (required)
        
    -   Receipt Date - (required) the date when the order is expected to be received from the vendor (for a purchase order) or the date when the assembly is expected to be completed (for a work order). This date can't be earlier than the Order Date.
        

## Prerequisites for Importing Item Supply Plans {#bridgehead_N417982}

-   Item supply plans are available for inventory items when the Demand Planning feature is enabled in your account.
    
-   Item supply plans are available for assembly/BOM items when both the Demand Planning and Work Orders feature are enabled.
    
-   Item supply plans can only be created for items that have a value of Time Phased for the Replenishment Method field.
    

Note:

For general information about demand planning in NetSuite, see [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html). For information about creating item supply plans in the NetSuite user interface, see [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html).

The following table shows how you might structure a file for importing item supply plans.

| External ID | Location | Item | Unit of Measure | Item Supply Plan Orders: Order Line | Item Supply Plan Orders: Order Date | Item Supply Plan Orders: Order Type | Item Supply Plan Orders: Receipt Date | Item Supply Plan Orders: Source Location | Item Supply Plan Orders: Quantity |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ISP-IMPNA02-01 | Boston | Scale | Case | 1 | 02/14/2014 | Work Order | 02/28/2014 | Chicago | 25 |
| ISP-IMPE02-02 | Prague | Blood Pressure Monitor | Case | 1 | 03/15/2014 | Purchase Order | 03/31/2014 | Brno | 30 |
| ISP-IMPE02-02 | Prague | Bandages | Case | 2 | 03/20/2014 | Purchase Order | 04/05/2014 | Brno | 15 |

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
-   [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
