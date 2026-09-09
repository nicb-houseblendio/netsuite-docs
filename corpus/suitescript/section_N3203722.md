---
id: "section_N3203722"
type: "section"
title: "Custom List"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Customization > Custom List"
parent: "chapter_N3203672"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3203722.html"
anchors: ["bridgehead_1490212871", "bridgehead_N3203794", "bridgehead_N3204012"]
sha256: "af3b335ce811ff4c7aca4982f5b18273ed8623b67c1ef8ff7bde1865096f9c1a"
---

A custom list is a list of values that you can use in custom fields on your forms and records. Custom lists enable you to set up predefined choices for your employees and customers to select when entering transactions and records. Custom lists can be searched using search filters and search columns.

For help working with this record in the UI, see [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html).

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with custom lists, see the following help topics:

-   [SuiteScript 2.1 Custom List Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518456414.html)
    
-   [Custom List IDs](#bridgehead_1490212871)
    
-   [Search Filters](#bridgehead_N3203794)
    
-   [Search Columns](#bridgehead_N3204012)
    

## Custom List IDs {#bridgehead_1490212871}

Each custom list has a unique ID. This value shown in the ID field on the custom list record. When creating or interacting with an instance of a custom record type, you must use this ID.

Every custom list ID is prefaced by `customlist`. If the ID was entirely system generated, it ends with a number (for example, `customlist100`). If the ID was customized when the record was created, the ID may be more descriptive. To view a list of all these IDs, go to _Customization > Lists, Records, & Fields > Lists_. These values are shown in the ID column.

## Search Filters {#bridgehead_N3203794}

| Field Internal ID | Field UI Label | Field Type |
| --- | --- | --- |
| internalid | Internal ID | select |
| internalidnumber | Internal ID (Number) | integer |
| isinactive | Inactive | checkbox |
| name | Name | text |

## Search Columns {#bridgehead_N3204012}

| Field Internal ID | Field UI Label | Field Type |
| --- | --- | --- |
| internalid | Internal ID | select |
| isinactive | Inactive | checkbox |
| name | Name | text |

### Related Topics

-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3203672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
