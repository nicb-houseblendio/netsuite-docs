---
id: "section_N396186"
type: "section"
title: "Cost Template Body and Sublist Fields"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Cost Template Import > Cost Template Body and Sublist Fields"
parent: "section_N395199"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N396186.html"
anchors: ["bridgehead_N396198", "bridgehead_N398146"]
sha256: "02061235ee8923de6f95a60e4b5d16d7ca178cd48c00eea63a802d397ab458f0"
---

When you import a cost template, you specify several body values, plus at least one record in the template's sublist.

## Body Fields {#bridgehead_N396198}

The following body fields are supported for import.

| Field | Notes | Required? |
| --- | --- | --- |
| ExternalId | Can be used as a unique identifier for the record. | No |
| Inactive | If set to Yes, the cost template is hidden in lists on records and forms. | No, but if you don't include a mapping for this field, the system uses the default value, which is No. |
| Memo | Can be used to add a description about the record. | No |
| Name | Used as a label for the template. This value must be unique. | Yes |
| Subsidiary (OneWorld only) | The subsidiary in which this template is available. | Yes, for OneWorld accounts |

## Sublist Fields {#bridgehead_N398146}

At least one row is required in this record's sublist. In the Import Assistant, this sublist is referred to as Manufacturing Cost Template Cost Detail. (In the UI, the sublist is labeled simply Costs - to see this, choose _Lists > Supply Chain > Manufacturing Cost Templates > New_).

Each record in the sublist must consist of a pair of values, as follows. Note that this sublist is not keyed.

| Field | Notes | Required? |
| --- | --- | --- |
| Cost Category | Must name a cost category record, created in NetSuite, that uses one of the manufacturing cost types. For more details on this entry, including restrictions on duplicate cost type references, see [Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395402.html#bridgehead_N395666). | Yes |
| Item | Must refer to a charge item, created in NetSuite, that uses the cost category named for this particular sublist record. If you choose an Item that uses a different cost category, the import fails. For more details on charge item records, refer to [Charge Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395402.html#bridgehead_N395975). | Yes |

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html)
-   [Prerequisite Records for Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395402.html)
-   [Cost Template CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N398462.html)
-   [Common Errors When Importing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399710.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
