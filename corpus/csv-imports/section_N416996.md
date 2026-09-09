---
id: "section_N416996"
type: "section"
title: "Supported Fields for Item Demand Plan Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Demand Plan Import > Supported Fields for Item Demand Plan Imports"
parent: "section_N414602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html"
anchors: []
sha256: "fbf7b653f5926634da834d131f3e94ef81c57948ba81f5939035730b2b8809e4"
---

Each CSV file used for an import should include data for only one type of time period, either monthly, weekly, or daily. Also, it's strongly encouraged that your CSV file use the preferred format for each type, because these preferred formats support automatic mapping of data in the Import Assistant. Other formats are also supported but are more difficult to use.

The following table lists standard fields available for item demand plan imports:

| Field | Mapping Required? | Notes |
| --- | --- | --- |
| **Body Fields** |
| External ID | No | \- |
| Internal ID | No | Available for updates only |
| Item | Yes | Item must have a value of Time Phased for the Replenishment Method field to be valid for this field. |
| Location | Yes, if Multi-Location Inventory enabled | \- |
| Memo | No | \- |
| Month | No | Redundant of Plan Start Date, Plan End Data fields |
| Plan End Date | Yes | Can set default on Import Assistant mapping page instead of setting value in CSV file |
| Plan Start Date | Yes | Can set default on Import Assistant mapping page instead of setting value in CSV file |
| Subsidiary | Yes, if OneWorld account | \- |
| Unit of Measure | No | Available when Multiple Units of Measure is enabled |
| View | Yes | Default value automatically set based on 'Monthly Quantity', 'Weekly Quantity', or 'Daily Quantity' keywords, when preferred format used If not inferred from keywords in preferred format, valid values are as follows (case-insensitive):
-   Monthly
-   Weekly
-   Daily

 |
| Year | No | Redundant of Plan Start Date, Plan End Data fields |
| **Sublist Fields** |
| Day of the Week | Yes, for Daily demand plans only | Day of the week Value automatically set, based on date provided in CSV file, when preferred format used If not inferred from date provided in preferred format, can be name of day, such as Sunday (case-insensitive) |
| Quantity | Yes | Represents either quantity per month, per week, or per day |
| Start Date | Yes | 

-   For monthly demand plans, first day of the month, based on date provided in CSV file
-   For weekly demand plans, first day of the week based on date provided in CSV file
-   For weekly demand plans, first day of the week based on date provided in CSV file

Default value automatically set when preferred format used |

Note:

You shouldn't enable the Overwrite Sublists option for item demand plan imports. Enabling this option may result in errors when imported sublist data overwrites existing sublist values driven by body field values such as View.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
-   [Demand Plan Body Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414956.html)
-   [Demand Plan Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html)
-   [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html)
-   [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html)
-   [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
