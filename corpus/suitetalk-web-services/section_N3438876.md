---
id: "section_N3438876"
type: "section"
title: "Enumerated Lists"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services > Enumerated Lists"
parent: "section_N3436475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438876.html"
anchors: []
sha256: "b7205a8f74e9a8c103162d0dc980ed9f59f908b0696857b1feecbec1aab8a140"
---

If values being returned for WSEnum and Enum fields in a get or search operation do NOT match the values enumerated in the schema, the following warning is returned:

          `Code = Invalid_data     Message = 'Error in record number <id>: Invalid field value <field>.     Please refer to the XSD for enumerated list of valid field values.'` 
        

In these cases, the existing data is corrupted and must be corrected before it can be retrieved using SOAP web services.

### Related Topics

-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Required Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html)
-   [Fields and Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
