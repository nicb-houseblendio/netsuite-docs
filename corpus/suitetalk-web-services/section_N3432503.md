---
id: "section_N3432503"
type: "section"
title: "Subrecords"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Records in SOAP Web Services > Subrecords"
parent: "section_N3428663"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html"
anchors: []
sha256: "4fb5282605fc4194c1c3444d99ccd1bdaa36583036056f2cc4c092b408d3f0a0"
---

A subrecord is similar to a record. You can take many of the same actions with a subrecord as you can with a record. However, like a sublist, an instance of a subrecord is always contained within a parent record. The first subrecord, inventory detail, was exposed to SOAP web services in the 2011.2 endpoint.

Any add, get, update, delete, or search operation on a subrecord must be performed within the context of an operation on its parent record. For example, if you want to update inventory detail data for a purchase order transaction, you must update the purchase order record itself. You cannot do an independent update of the inventory detail object. This limitation applies to all operations on a subrecord.

When working with subrecords, the replaceAll attribute determines whether the subrecord will be added or updated during an update operation on its parent record. If this attribute is set to true, the subrecord is deleted and a new one is added. If replaceAll is set to false, the existing subrecord is updated.

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428928.html)
-   [Search Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3429060.html)
-   [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html)
-   [External IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3433806.html)
-   [Shared Internal and External IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
