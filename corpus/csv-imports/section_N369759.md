---
id: "section_N369759"
type: "section"
title: "Common Errors When Importing Custom Lists"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Customization Import Type > Custom List Import > Common Errors When Importing Custom Lists"
parent: "section_N363830"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N369759.html"
anchors: ["bridgehead_N369771", "bridgehead_N369792", "bridgehead_1541154812"]
sha256: "bdc1b9ab00d9ceb4e4ae35c341ac2eb6dc072171183084e563f4eaaca6081995"
---

The 'Results' file for a failed custom list import might include any of the following messages.

## 'Adding new line to sublist translations is not allowed' {#bridgehead_N369771}

This error might indicate that you tried to map data to the Custom List Translation sublist when the Multi-Language feature was not properly set up. For imports to this sublist to work, the Multi-Language feature must be enabled, and at least one language must be listed on the Languages subtab at _Setup > Company > Enable Features_. For more details, see [Custom List Translation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N364491.html#bridgehead_3705043200).

## 'Unable to find a matching line for sublist translations' {#bridgehead_N369792}

This error might indicate that you created a static mapping for the Language field (using the edit icon on the mapping page) when your CSV file included translations for more than one language. You can use the static mapping successfully only if the CSV file includes translations for **one** language and no others.

## 'One of the columns \[id, name\] must be mapped in the CUSTOMLIST import' {#bridgehead_1541154812}

This error might indicate that neither a name, nor an internal or external ID was mapped on the field mapping page of the Import Assistant. For the import to succeed, you must select a reference type, either a name or an ID, and map it to your CSV file content, using the edit icon on the mapping page. For more information about using reference types, see [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html).

### Additional Information

-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)

### Related Topics

-   [Custom List Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363830.html)
-   [Custom List Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html)
-   [Custom List Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N364491.html)
-   [Custom List CSV Multiple File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N365834.html)
-   [Custom List CSV Single File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157890910739.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
