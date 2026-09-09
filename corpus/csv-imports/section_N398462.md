---
id: "section_N398462"
type: "section"
title: "Cost Template CSV File Examples"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Cost Template Import > Cost Template CSV File Examples"
parent: "section_N395199"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N398462.html"
anchors: ["bridgehead_N398474", "bridgehead_N399180"]
sha256: "266012ffb3d1b0afb6b64e67e76ee12b10154b770d1cb8a1812bc36477753371"
---

You can import cost template records using multiple files or a single file.

## Multiple Files Import {#bridgehead_N398474}

With a multiple-file import, you use one file for the cost template body fields and another file for the Cost Detail sublist.

The file holding the body data must include, at a minimum, the name of the template. An External ID is also preferred. For example:

| ExternalId | Name |
| --- | --- |
| 101 | Metalworking Rates |
| 102 | Mailroom Rates |
| 103 | Warehouse Rates |

For full details on body fields supported for import, see [Custom List Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html).

Each row in the second file must include a cost category and an item that are a matching pair. For example, suppose the charge item value is Metalworker Labor Run and the cost category value is Skilled-Labor Run. If you open the item record for Metalworker Labor Run and review the record's Purchasing subtab, you should see the cost category for the item. If that category is not Skilled-Labor Run, the import fails.

Further, each row in the file must include a unique identifier to pair the row with the appropriate entry from the main file.

For example, the following data would create one sublist record for each of the three cost templates identified in the sample main file above.

| ExternalId | Cost Category | Item |
| --- | --- | --- |
| 101 | Skilled-Labor Run | Metalworker Labor Run |
| 102 | Labor Run | Mailroom Labor Run |
| 103 | Labor Run | Warehouse Labor Run |

If you want to create more than one sublist record for any of your cost template records, add multiple rows for that item to the secondary file. Again, make sure that each row includes a unique identifier to match the sublist data to the appropriate cost template record.

| ExternalId | Cost Category | Item |
| --- | --- | --- |
| 101 | Skilled-Labor Run | Metalworker Labor Run |
| 101 | Skilled-Labor Setup | Metalworker Labor Setup |
| 101 | Skilled-Labor Machine Run | Forge Press Machine Run |
| 102 | Labor Run | Mailroom Labor Run |
| 102 | Labor Setup | Mailroom Setup Rates |
| 103 | Labor Run | Warehouse Labor Run |
| 103 | Labor Setup | Warehouse Setup Rates |

With a multiple-file import, you should have a file for the Cost Detail sublist. The fields of this file should be mapped to the corresponding NetSuite fields, which you can see when you expand the sublist. If you have named your columns as shown in the tables above, the mapping should happen automatically.

## Single File Import {#bridgehead_N399180}

With a single-file import, all data for a single cost template record must exist on a single row. For this reason, if the sublist data for any cost template must include more than one record, you must create a discrete set of columns for mapping **each** cost category and item pair.

For example, the following sample would create three new cost template records. For each cost template record, the Cost Detail sublist would include two records.

| External ID | Name | Manufacturing Cost Template Cost Detail 1: Cost Category | Manufacturing Cost Template Cost Detail 1: Item | Manufacturing Cost Template Cost Detail 2: Cost Category | Manufacturing Cost Template Cost Detail 2: Item |
| --- | --- | --- | --- | --- | --- |
| 104 | Woodworking rates | Skilled-Labor Run | Woodworker Labor Run | Skilled-Labor Overhead | Woodworker-Lab Costs |
| 105 | Project management rates | Skilled-Labor Run | Project-Manager Labor Run | Skilled-Labor Overhead | Conference- Room Use |
| 106 | Assembly line rates | Labor Run | Assembly-Worker Labor Run | Machine Run | Assembly-Line Machine Cost |

On the mapping page, the main fields should be mapped to the NetSuite fields under Manufacturing Cost Template, and the Cost Detail sublist columns must be mapped to the corresponding Cost Detail sublist fields. In this example, two instances of the sublist fields must be used, because the CSV file includes two sets of cost-category/item pairings.

If you name your columns as shown in this example, the mapping should happen automatically. If you choose column headings that don't match what the system expects, you must map the fields manually.

In these cases, if your import requires multiple instances of the sublist fields, you must manually create the additional fields in the right-hand mapping column under 'NetSuite Fields.' You can create an extra instance by clicking the plus sign to the right of the Cost Template Cost Detail label.

### Related Topics

-   [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html)
-   [Prerequisite Records for Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395402.html)
-   [Cost Template Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N396186.html)
-   [Common Errors When Importing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399710.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
