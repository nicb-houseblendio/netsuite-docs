---
id: "section_N414956"
type: "section"
title: "Demand Plan Body Data"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Demand Plan Import > Demand Plan Body Data"
parent: "section_N414602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414956.html"
anchors: []
sha256: "475915d5901cfe7497b4d864332cedbd4a7d0e974075d64488ba032b9f35c27e"
---

Most body fields are used to uniquely identify the demand plan, such as **Item, Plan Start Date**, **Plan End Date, Location** (when Multi-Location Inventory is enabled), and **Subsidiary** (for NetSuite OneWorld). Data for each of these body fields should be stored in its own column in the CSV file.

Generally, demand plans are unique per item. In NetSuite OneWorld accounts, demand plans are unique per item/subsidiary combination. When Multi-Location Inventory is enabled, demand plans are unique per item/location combination or per item/subsidiary/location combination.

A **View** body field indicates the time period used in the demand plan: monthly, weekly, or daily. In the preferred format, this field doesn't need its own CSV file column; its value is inferred from the heading of quantity columns. See [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html), [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html), and [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html).

![Item Demand Plan body fields.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/demandplanbodyfields.png)

The demand plan body fields that can be imported remain consistent for all types of plans. If you use column headings that match NetSuite field names, these fields are automatically mapped in the Import Assistant.

See [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html) for more details on specific fields.

### Related Topics

-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
-   [Demand Plan Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html)
-   [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html)
-   [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html)
-   [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html)
-   [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
