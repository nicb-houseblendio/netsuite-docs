---
id: "section_N3195081"
type: "section"
title: "Item Demand Plan"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Item Demand Plan"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3195081.html"
anchors: ["bridgehead_1492725375", "bridgehead_1492725131", "bridgehead_N3195122"]
sha256: "6aa60f09d2b1cee375d7435bf8022c5840f5d71a1eb642bddb19a1fb0160679f"
---

The item demand plan record is available for inventory items when the Demand Planning feature is enabled, and for assembly/BOM items when both the Demand Planning and Work Orders features are enabled. Item demand plans can be added for items where the supplyReplenishMethod field is set to Time Phased.

An item demand plan transaction stores the quantity expected to be needed, during specified time periods, for an item. NetSuite supports three types of demand plans: monthly, weekly, and daily.

For help working with this record in the UI, see [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html).

The internal ID for this record is `itemdemandplan`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/itemdemandplan.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492725375}

The item demand plan record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492725131}

The invoice record is partially scriptable - it can be created, updated, deleted, and searched using SuiteScript. It cannot be copied or transformed.

## Usage Notes {#bridgehead_N3195122}

A demand plan records the expected future demand for an item based on previous or projected demand. When the Demand Planning feature is enabled, demand plans can be created for inventory items. When the Work Orders feature is also enabled, demand plans also can be created for assembly/BOM items. Demand plans can only be created for items that have a value of 'Time Phased' for the **supplyreplenishmethod** field.

Each demand plan record includes:

-   A set of body fields used to uniquely identify the demand plan, define the time period it covers, and indicate the time period it uses (monthly, weekly, or daily).
    
    Body fields must be defined before matrix field values can be edited.
    
-   A matrix of projected quantities per time period, similar to the matrix used for item pricing.
    
    -   In a monthly demand plan, this matrix includes a row for each month in the time period, and one column with the projected quantity demand for each month.
        
    -   In a weekly demand plan, this matrix includes a row for each week in the time period, and one column with the projected quantity demand for each week.
        
    -   In a daily demand plan, this matrix includes a row for each week in the time period and seven columns with the projected quantity demand for each day of each week.
        
-   Review the following table for details about Item Demand Plan body and matrix sublist fields. For more details and code samples, see [Demand Plan Detail Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3212114.html).
    

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| subsidiary | Subsidiary | Required in OneWorld accounts. |
| location | Location | Required when the Multi-Location Inventory feature enabled. |
| item | Item | 
Required.

Can only use items with supplyreplenishment method set to Time Phased.



 |
| units | Unit of Measure | 

Optional.

Available when the Multiple Units of Measure feature is enabled.



 |
| memo | Memo | Optional. |
| startdate | Start Date | 

Optional.

Defaults to the first day of the current year, for example for 2011, defaults to 1/1/2011.



 |
| enddate | End Date | 

Optional.

Defaults to the last day of the current year, for example for 2011, defaults to 12/31/2011.



 |
| demandplancalendartype | View | 

Required.

Valid values are MONTHLY, WEEKLY, or DAILY. (Must use all capital letters.)



 |
| **Matrix Fields** |
| quantity | Quantity | 

-   For monthly and weekly demand plans, each row has one quantity column.
-   For daily demand plans, each row has seven quantity columns.

 |
| startdate | Start Date | System-calculated, read-only values.

-   For monthly plans, the date of the first day of the month that the row represents.
-   For weekly and daily plans, the date of the first day of the week that the row represents, based on the preference set for First Day of Week at _Setup > Company > General Preferences_.

 |
| enddate | End Date | System-calculated, read-only values.

-   For monthly plans, the date of the last day of the month that the row represents.
-   For weekly and daily plans, the date of the last (seventh) day of the week that the row represents, based on the preference set for First Day of Week at _Setup > Company > General Preferences_.

 |

Note:

You should work with the Item Demand Plan record in dynamic mode. See [SuiteScript 2.x Standard and Dynamic Modes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1524156901.html).

### Related Topics

-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
