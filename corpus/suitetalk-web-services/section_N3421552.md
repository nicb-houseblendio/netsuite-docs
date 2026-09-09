---
id: "section_N3421552"
type: "section"
title: "NetSuite Features in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Setup > SOAP Web Services Development Considerations > NetSuite Features in SOAP Web Services"
parent: "section_N3421363"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421552.html"
anchors: []
sha256: "ca34ee4ef3f6017d590e7ec31af9b8ab30f230faa124eceebf6c650a0faa9877"
---

The NetSuite UI lets you enable or disable certain features. When designing your SOAP web services, it is important to know which features must be enabled for the service to run properly. If a disabled feature is called, a SOAP **InsufficientPermissionFault** occurs causing the entire service to fail. For example, in the NetSuite UI you can enable or disable the Opportunities feature for CRM. If disabled, a web service call to add an OpportunityItem will fail.

SOAP web services is itself a feature that **must** be enabled prior to submitting SOAP web services requests. To enable the feature, see [Enabling the SOAP Web Services Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419926.html).

### Related Topics

-   [Development Considerations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421458.html)
-   [SOAP Web Services Reliability Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540364662.html)
-   [Effects of Account Configuration in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421585.html)
-   [Enumerations, Special Characters, and Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421860.html)
-   [Image References in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421872.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
