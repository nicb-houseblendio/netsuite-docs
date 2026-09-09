---
id: "section_N3429060"
type: "section"
title: "Search Records"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Records in SOAP Web Services > Search Records"
parent: "section_N3428663"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3429060.html"
anchors: []
sha256: "0b90438a7038410964809bb77b19459a5cec5f0e9ee0b7358a968bed36ab9cba"
---

Search record types encapsulate the available search criteria for a specific NetSuite record type. A NetSuite search record is defined as a top-level record that is used in the request portion of a search operation. Any field defined within a search record must be of one of the following logical types.

| Type | Description |
| --- | --- |
| String | Corresponds to the [SearchStringField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3461474) type |
| Int | Corresponds to the [SearchTextNumberField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3462885) type |
| Double | Corresponds to the [SearchDoubleField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3461822) type |
| Boolean | Corresponds to the [SearchBooleanField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3461684) type |
| Datetime | Corresponds to the [SearchDateField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3463126) type |
| MultiSelectRef | Corresponds to the [SearchMultiSelectField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3463443) type |
| MultiSelectEnum | Corresponds to the [SearchEnumMultiSelectField](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3463650) type |

For details on using the search operation, see [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html). Also see the following topics, which describe all search types that can be used when constructing SOAP web services searches.

-   [SOAP Objects Used in a Basic Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html#bridgehead_N3514890)
    
-   [SOAP Objects Used in a Joined Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html#bridgehead_N3516482)
    
-   [SOAP Objects used in Advanced Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html#bridgehead_N3517407)
    

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428928.html)
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
-   [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html)
-   [External IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3433806.html)
-   [Shared Internal and External IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
