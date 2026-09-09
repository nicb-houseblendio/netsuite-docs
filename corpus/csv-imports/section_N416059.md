---
id: "section_N416059"
type: "section"
title: "Daily Item Demand Plan Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Item Demand Plan Import > Daily Item Demand Plan Import"
parent: "section_N414602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416059.html"
anchors: []
sha256: "bf581e2e1898e43d0e690836fd9201a4aeda2b7ec085b1c0ea28d2de21cdd6d4"
---

The following screenshot shows a daily item demand plan in the NetSuite user interface, with sublist fields outlined in red. Each week included in the plan is represented by a row in this screenshot. Each row includes seven columns, one for each day of the week.

![Sublist fields on the Daily Item Demand Plan.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/demandplandaily_2014_2.png)

The preferred format in your CSV file for this sublist data is to include one column for each day, with a heading of **Daily Quantity:<date>** and the quantity value. For example, columns like the following should be included for the first week of a daily item demand plan:

| Daily Quantity: 1/2/2012 | Daily Quantity: 1/3/2012 | Daily Quantity: 1/4/2012 | Daily Quantity: 1/5/2012 | Daily Quantity: 1/6/2012 |
| --- | --- | --- | --- | --- |
| 50 | 200 | 100 | 100 | 100 |

Each quantity column corresponds to one day, meaning one sublist instance, for a daily plan.

The following screenshot illustrates how the above columns are automatically mapped in the Import Assistant:

![Daily Item Demand Plan mapping.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/demandplandailymap.png)

-   The View body field is automatically mapped to a value of Daily based on the **Daily Quantity** keywords in the quantity column headings.
    
-   A Start Date field for each sublist instance is automatically mapped to the date of the first day of the week based on the date in each quantity column heading.
    
    -   Each sublist Start Date must correspond to the date of the first day of the week based on the company preference set at _Setup > Company > General Preferences_. The default is Sunday.
        
    -   Up to seven columns may have the same Start Date, and belong to the same sublist instance. In the example above, if a first day of week preference of Sunday is assumed, each quantity has a Start Date value of 1/1/2012.
        
    -   A sublist Start Date may precede the Plan Start Date, if the Plan Start Date is not the first day of the week. For example, if the Plan Start Date is 2/1/2012, which is a Wednesday, and the preference for first day of the week is Sunday, the sublist Start Date would be 1/29/2012.
        
-   A Day of the Week field for each sublist instance is automatically mapped to a day of the week, based on the date in each quantity column heading.
    
    For example, the quantity column with a date of 1/2/2012 is mapped to Monday, 1/3/2012 is mapped to Tuesday, 1/4/2012 is mapped to Wednesday, 1/5/2012 is mapped to Thursday, and 1/6/2012 is mapped to Friday.
    
-   A Quantity field for each sublist instance is automatically mapped to a Daily Quantity.
    
-   Sublist End Date fields don't need to be included in CSV files or Import Assistant mappings.
    

### Related Topics

-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
-   [Demand Plan Body Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414956.html)
-   [Demand Plan Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html)
-   [Monthly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415398.html)
-   [Weekly Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415713.html)
-   [Supported Fields for Item Demand Plan Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N416996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
