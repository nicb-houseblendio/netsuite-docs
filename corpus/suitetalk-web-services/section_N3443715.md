---
id: "section_N3443715"
type: "section"
title: "Sublist Line Numbers"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Sublists in SOAP Web Services > Sublist Line Numbers"
parent: "section_N3439908"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443715.html"
anchors: []
sha256: "bebc93b9a0790c38480c92ec9c493ceff189338c414a5fb3d19162668c4b2fd9"
---

The index number for each sublist line is assigned by the system. SOAP web services developers cannot change these values. When lines are added or removed from a sublist (using either the UI or SOAP web services), the system does not re-index the line numbers. Therefore, it is best practice to perform a get operation on the sublist data before trying to update individual lines, otherwise you may be updating the wrong line in the sublist.

For example, if you perform a get operation on an Items sublist on a transaction record, the index values for the first three line items might be:

<ns3:line>1</ns3:line>

<ns3:line>8</ns3:line>

<ns3:line>9</ns3:line>

### Related Topics

-   [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html)
-   [Updating Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3441570.html)
-   [Deleting All Lines on a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443838.html)
-   [Searching a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443977.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
