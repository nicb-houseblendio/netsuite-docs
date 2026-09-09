---
id: "section_N400811"
type: "section"
title: "Routing Body and Sublist Fields"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Routing Import > Routing Body and Sublist Fields"
parent: "section_N399906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400811.html"
anchors: ["bridgehead_N400823", "bridgehead_N401212"]
sha256: "ae02a628ad69374a499596e7f109fb2dca8d3505d981b0a143bf0b25d707a4ee"
---

When you import a routing record, you specify several body values, plus at least one entry in the record's sublist.

## Body Fields {#bridgehead_N400823}

The following body fields are supported for import.

| Field | Notes | Required? |
| --- | --- | --- |
| Default | If mapped to a value of Yes, this routing is used as the default for the assembly item specified in the Item field. | No, but if you don't include a mapping for this field, the system uses the default value, which is No. |
| ExternalId | Can be used as a unique identifier for the record. | No |
| Inactive | If mapped to a value of Yes, this routing is hidden in lists on records and forms. | No, but if you don't include a mapping for this field, the system uses the default value, which is No. |
| Item | The assembly item to which this routing can be applied. | Yes |
| Location | The locations with which this routing is associated. When entering multiple locations, separate each value with either the pipe symbol ( | ) or your custom multi-select value delimiter (which can be specified on either the CSV Import Preferences page or under Advanced Options on the second page of the Import Assistant). | Yes |
| Memo | Can be used to add a description about the record. | No |
| Name | A name for this particular routing. This value must be unique. | Yes |
| Subsidiary (OneWorld only) | The subsidiary with which this routing is associated. | Yes, for OneWorld accounts |

## Sublist {#bridgehead_N401212}

For each routing record, you must include at least one record in the Manufacturing Routing Routing Steps sublist. Each record in the sublist must include values for the fields listed in the following table.

Note that this sublist is keyed - the key field is Operation Sequence.

| Field | Notes | Required? |
| --- | --- | --- |
| Operation Sequence | A numeric value that determines the sequence of this operation relative to others. This field is the key for the sublist. | Yes |
| Operation Name | A name that describes the task to be completed. | Yes |
| Manufacturing Work Center | The group responsible for completing the operation. | Yes |
| Manufacturing Cost Template | The rates associated with this work. | Yes |
| Setup Time (Min) | The number of minutes of setup time required to complete the task. | Yes |
| Run Rate (Min/Unit) | The number of minutes per unit required to complete this task. | Yes |

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Manufacturing Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399906.html)
-   [Prerequisite Records for Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400118.html)
-   [Routing CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N401643.html)
-   [Common Errors When Importing Routing Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404433.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
