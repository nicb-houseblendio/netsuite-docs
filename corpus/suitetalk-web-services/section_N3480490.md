---
id: "section_N3480490"
type: "section"
title: "SOAP Web Services List Operations"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > SOAP Web Services List Operations"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html"
anchors: []
sha256: "845cc7f7d5251c1eb015383e5063bd1b191a85bd5b6da0ff9f89bca99f2d5933"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Within a single SOAP request, only one operation can be performed. For example, one add, one addList or one delete. However, a single **list** operation (addList, updateList, upsertList, deleteList, getList, and initializeList) lets you work with multiple record types. For example, with a single addList operation you can add 3 customers, 4 opportunities, and 1 contact.

Note:

List operations process records in the order in which the records are submitted. For example, an addList operation will add all records in the order they appear in the list.

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)
-   [SOAP Web Services Governance Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
