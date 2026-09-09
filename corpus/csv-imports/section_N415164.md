---
id: "section_N415164"
type: "section"
title: "Demand Plan Sublist Data"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Demand Plan Import > Demand Plan Sublist Data"
parent: "section_N414602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html"
anchors: []
sha256: "9981fc033812649b37e5d867a30e8493f4b834f81a6fd959635bbb4199e0523c"
---

Demand plan sublist fields vary according to the plan type: monthly, weekly, or daily. A demand plan usually includes multiple start dates and end dates. Each start date-end date pairing represents a time period within the demand plan. Quantity sublist field values store the projected quantity needed for each time period.

-   For monthly demand plans, each start date-end date pairing represents a month, for which one quantity can be stored.
    
-   For weekly demand plans, each start date-end date pairing represents a week, for which one quantity can be stored.
    
-   For daily demand plans, each start date-end date pairing represents a week, for which up to seven quantities can be stored. Each quantity is tied to a day of the week.
    

The Import Assistant Field Mapping page displays Item Demand Plan sublist fields in the Item Demand Plan Demand Planning folder:

![Item Demand Plan sublist fields.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/demandplansublistfields.png)

To import sublist data for multiple days, weeks, or months, add all your sublist data into one demand plan sublist file. Then map your daily, weekly, or monthly data to separate instances of the Item Demand Plan DemandPlanning sublist, as shown in the previous screenshot. Do not use separate files for the data for each day, week, or month.

Each sublist instance represents a time period within the demand plan, like each row on the Item Demand Plan page in the user interface. For monthly and weekly plans, each sublist instance includes two fields: **Start Date** and **Quantity**. For daily plans, each sublist instance also includes the **Day of the Week** field. Note that the **End Date** sublist field isn't required for CSV imports.

There's a separate instance of this sublist, represented by a numbered subfolder, for each quantity column included in the CSV file. If your file includes a quantity for each month in a year, there are 12 instances of the sublist. If your file includes a quantity for each week in a year, there are 52 instances of the sublist. it's best to use the preferred file format and rely on automatic mapping of the data, so you don't have to manually map fields for a large number of sublist instances. For details about preferred formats, see [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html), [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html), and [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html).

See [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html) for more details on specific fields.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
-   [Demand Plan Body Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414956.html)
-   [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html)
-   [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html)
-   [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html)
-   [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
