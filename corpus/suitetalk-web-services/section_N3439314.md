---
id: "section_N3439314"
type: "section"
title: "Fields and Operations"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services > Fields and Operations"
parent: "section_N3436475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html"
anchors: []
sha256: "3931dc04c252e18cd26c6b1ef0e3d175501281c413e6daef97cd0b895fa414f9"
---

For simplicity, the SOAP WSDL is designed with all available fields listed for each record in each corresponding XSD. There is no differentiation as to what field is available for each operation. For example, add operations take a separate set of field values than the corresponding update operation for some records. If your SOAP web services request includes a field value for a field that is unavailable, an error is thrown for that submission.

If you are using SOAP web services for data migration where there may be fields that need to be populated that are unavailable during an add operation, you should perform two consecutive requests. Submit an initial add or addList request, with values for all fields available for an add operation, followed by an update or updateList request, with values for the fields available only during an update operation.

### Related Topics

-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Required Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html)
-   [Field Lengths](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
