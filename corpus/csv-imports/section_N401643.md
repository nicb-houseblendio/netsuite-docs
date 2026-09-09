---
id: "section_N401643"
type: "section"
title: "Routing CSV File Examples"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Routing Import > Routing CSV File Examples"
parent: "section_N399906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N401643.html"
anchors: ["bridgehead_N401655", "bridgehead_N402333"]
sha256: "2a3244edeb6c73ddb1f217e01418a7c9c4623602e02a33a3d19a4b17aa06a853"
---

You can import routing records using multiple files or a single file.

## Multiple Files Import {#bridgehead_N401655}

With a multiple-file import, you create a main file for body fields and a secondary file for the Routing Steps sublist. The following example shows how your main file might look when importing one routing record.

| ExternalId | Item | Location | Name |
| --- | --- | --- | --- |
| 101 | Cedar Chest | East Coast | Cedar Chest - Standard Routing |

The second file should include details of the operations required by the assembly process. Each operation belongs on its own row and must include a unique identifier that links it to an entry in the main file, as follows.

| ExternalId | Operation Sequence | Operation Name | Manufacturing Work Center | Manufacturing Cost Template | Setup Time (Min) | Run Rate (Min/Unit) |
| --- | --- | --- | --- | --- | --- | --- |
| 101 | 10 | Retrieve materials | Warehouse Employees | Warehouse Rates | 5 | 20 |
| 101 | 20 | Sand boards | Woodworkers | Woodworking Rates | 15 | 40 |
| 101 | 30 | Assemble chest | Woodworkers | Woodworking Rates | 15 | 180 |
| 101 | 40 | Clean up work space | Shop Workers | Shop-Working Rates | 5 | 25 |
| 101 | 50 | Move chest to stock room | Warehouse Employees | Warehouse Rates | 5 | 25 |

With a multiple-file import, you should have a file for the body fields of the record and a file for the routing steps sublist. The fields of each file should be mapped to the corresponding NetSuite fields. If you name your columns as shown in this example, the mapping should happen automatically.

## Single File Import {#bridgehead_N402333}

With a single-file import, all data for a single routing record must exist on the same row. For this reason, if the sublist for any routing record must describe more than one operation, you must create a discrete group of columns for mapping **each** operation. Each group should include all six required sublist fields (Manufacturing Cost Template, Manufacturing Work Center, and so on).

For example, the following table shows an excerpt from a file you could use to create two new manufacturing routing records. For each routing record, two operations are defined for the Routing Steps sublist. (The entire data snippet is not shown; for the import to be successful, both rows would include additional columns representing second instances of the Work Center, Cost Template, Setup Time, and Run Rate fields.)

| Name | Manufact-uring Routing Routing Steps 1: Operation Sequence | Manufact-uring Routing Routing Steps 1: Operation Name | Manufact-uring Routing Routing Steps 1: Manufact-uring Work Center | Manufact-uring Routing Routing Steps 1: Manufact-uring Cost Template | Manufact-uring Routing Routing Steps 1: Setup Time (Min) | Manufact-uring Routing Routing Steps 1: Run Rate (Min/Unit) | Manufact-uring Routing Routing Steps 2: Operation Sequence | Manufact-uring Routing Routing Steps 2: Operation Name |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Cedar chest routing | 10 | Retrieve materials | Warehouse Labor Run | Warehouse Employee Rates | 5 | 60 | 20 | Build chest |
| Clock routing | 10 | Retrieve materials | Warehouse Labor Run | Warehouse Employee Rates | 5 | 30 | 20 | Build clock |

On the mapping page, ensure that the fields are mapped to the correct sublist under the NetSuite Fields panel. Note that, in the column at the right, two instances of the sublist fields must be used. Two instances are used because the CSV file includes two sets of columns for the routing steps sublist.

If you name your columns as shown in this example, the mapping should happen automatically. If in your CSV file you choose column headings that don't match what the system expects, you must map the fields manually.

In these cases, if your import requires multiple instances of the sublist fields, you must manually create the additional fields in the right-hand mapping column under 'NetSuite Fields.' You can create an extra instance by clicking the plus sign to the right of the Manufacturing Routing Routing Steps label.

### Related Topics

-   [Manufacturing Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399906.html)
-   [Prerequisite Records for Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400118.html)
-   [Routing Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400811.html)
-   [Common Errors When Importing Routing Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404433.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
