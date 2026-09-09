---
id: "section_N415713"
type: "section"
title: "Weekly Item Demand Plan Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Demand Plan Import > Weekly Item Demand Plan Import"
parent: "section_N414602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html"
anchors: []
sha256: "49f5173b581c948db20ea2b279f9b8363759242732e060c5d147c3866bee0e72"
---

The following screenshot shows a weekly item demand plan in the NetSuite user interface, with sublist fields outlined in red. Each week included in the plan is represented by a row in the screenshot.

![Sublist fields on the Weekly Item Demand Plan.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/demandplanweekly_2014_2.png)

The preferred format in your CSV file for this sublist data is to include one column for each week, with a heading of **Weekly Quantity:<date of first day of week>** and the quantity value. For example, columns like the following should be included for the first 3 weeks of a weekly item demand plan:

| Weekly Quantity:1/1/2012 | Weekly Quantity:1/8/2012 | Weekly Quantity:1/15/2012 |
| --- | --- | --- |
| 100 | 200 | 200 |

Each quantity column corresponds to one week, meaning one sublist instance, for a weekly plan.

The following screenshot illustrates how the above columns are mapped in the Import Assistant:

![Weekly Item Demand Plan mapping.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/demandplanweeklymap.png)

-   The View body field is automatically mapped to a value of Weekly based on the **Weekly Quantity** keywords in the quantity column headings.
    
-   A Start Date field for each sublist instance is mapped to the date of the first day of the week based on the date in each quantity column heading.
    
    -   Each sublist Start Date must correspond to the date of the first day of the week based on the company preference set at _Setup > Company > General Preferences_. The default is Sunday.
        
    -   If the date in a CSV file quantity column doesn't correspond to the first day of the week, the Import Assistant maps the date of the first day of the week, instead of the date in the CSV file, as Start Date. For example, for a heading of **Weekly Quantity:1/9/2011** where the first day of the week is Sunday, the mapped Start Date value is 1/8/2011, because that's the date of the Sunday of that week.
        
    -   A sublist Start Date may precede the Plan Start Date, if the Plan Start Date is not the first day of the week. For example, if the Plan Start Date is 2/1/2012, which is a Wednesday, and the preference for first day of the week is Sunday, the sublist Start Date is 1/29/2012.
        
    -   The date in the CSV file quantity column must be entered without leading zeros. For example, for January 1, 2017 to be used as the Start Date, enter this date in the CSV file as 1/1/2017, not 01/01/2017.
        
-   A Quantity field for each sublist instance is mapped to a Weekly Quantity.
    
-   Sublist End Date fields don't need to be included in CSV files or Import Assistant mappings.
    

You can also move your sublist data to a separate import file, and upload multiple files. In this case, make sure that your primary file only includes body field data, and all the sublist data for the Demand Planning sublist is moved to the linked file.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
-   [Demand Plan Body Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414956.html)
-   [Demand Plan Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html)
-   [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html)
-   [Daily Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html)
-   [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
