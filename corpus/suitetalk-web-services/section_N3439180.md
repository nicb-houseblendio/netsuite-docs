---
id: "section_N3439180"
type: "section"
title: "Required Fields"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services > Required Fields"
parent: "section_N3436475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html"
anchors: []
sha256: "b1d83df72e35116caf83a94aa8838e198fb824229b19908e4a6efdf45c780682"
---

Required fields in the UI do not necessarily correspond to required fields in SOAP web services. This is because there can be standard defaults that are applied if the field is not populated. For example, in the CalendarEvent record type, the _eventAccess_ field is required in the UI. However, it is optional in SOAP web services because it has a default value of Public.

Important:

The **Required** column in the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html) lists T or F (for true or false) to specify if a field is required by the form in the user interface. Refer to the **Cardinality** column to see whether the XSD imposes a requirement for the field. For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

### Related Topics

-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Field Lengths](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438979.html)
-   [Fields and Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
