---
id: "section_N414602"
type: "section"
title: "Item Demand Plan Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Demand Plan Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html"
anchors: ["bridgehead_N414690", "bridgehead_N414735"]
sha256: "5c31d5381b3712d7d979f14cee7cdb1e1e12ac41b0c47049f5b92d4dd53c1867"
---

An item demand plan transaction stores the quantity expected to be needed, during specified time periods, for an item. You can import item demand plan data from another system into NetSuite. You need to get the required data into a CSV file, then you can use the Import Assistant to create new demand plans and edit existing demand plans.

The item demand plan data that you can import generally matches the fields available at _Transactions > Demand Planning > Item Demand Plans > New_. If you're not familiar with this page, you should review it to get an understanding of the fields that you should include in your Item Demand Plan CSV files. Each plan includes two types of fields:

-   Body fields used to uniquely identify the record, such as Item, Plan Start Date, Plan End Date, Location (when Multi-Location Inventory is enabled), and Subsidiary (for NetSuite OneWorld). A View body field indicates the time period used in the demand plan: monthly, weekly, or daily. For more information, see [Demand Plan Body Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414956.html).
    
-   Sublist data that varies according to the demand plan type, as represented by the monthly, weekly, and daily views. The Import Assistant maps one sublist instance per row. For a monthly plan, each row/sublist instance represents a month and can store one monthly quantity. For a weekly plan, each row/sublist instance represents a week and can store one weekly quantity. For a daily plan, each row/sublist instance represents a week and can store up to seven daily quantities. For more information, see [Demand Plan Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html).
    

You're encouraged to set up your CSV files in accordance with the preferred format for each demand plan type. When a CSV file follows the preferred format, the Import Assistant automatically maps CSV file fields to NetSuite fields, simplifying the import process. For body fields other than the View field, the preferred format is to include a column with a header matching the NetSuite field name. For sublist fields, the preferred format varies per plan type. For more information, see: [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html), [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html), and [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html).

Each CSV file used for an import should include data for only one type of time period: either monthly, weekly, or daily. Also, it is strongly encouraged that your CSV file use the preferred format for each type, because these preferred formats support automatic mapping of data in the Import Assistant. For more information, see [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html).

## Prerequisites for Importing Item Demand Plans {#bridgehead_N414690}

-   Item demand plans are available for inventory items when the Demand Planning feature is enabled in your account.
    
-   Item demand plans are available for assembly/BOM items when both the Demand Planning and Work Orders feature are enabled.
    
-   Demand plans can only be created for items that have a value of Time Phased for the Replenishment Method field.
    

If the above requirements are met, you can also import data for item record fields related to demand planning. See [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html).

## Item Demand Plan Import Errors {#bridgehead_N414735}

An import that attempts to add an item demand plan returns an 'Invalid item reference Key' error when any of the following occur:

-   The item doesn't exist in NetSuite.
    
-   The demand plan already exists. (Only one demand plan can be created per item and location combination.)
    
-   The Replenishment Method field for the item isn't set to Time Phased.
    

Note:

For information about using demand planning and creating item demand plans in the NetSuite user interface, see [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
