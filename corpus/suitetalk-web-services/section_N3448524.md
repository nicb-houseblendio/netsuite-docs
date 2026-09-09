---
id: "section_N3448524"
type: "section"
title: "Custom Field Security"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Security > Custom Field Security"
parent: "chapter_N3445516"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448524.html"
anchors: []
sha256: "0de5c57a18b7fa5a66394bf05a60d9fc9c100ece379890bf9b9bf49ac4642408"
---

Custom field security can be applied on a per-field basis. If field security has been applied to a field in the UI, the custom field schema will include the field level security metadata. Consequently, users should be aware that the permissions they specify on custom fields will apply to any existing integration that is in place using endpoints 2008\_1 and older. Certain field permissions such as NONE and VIEW might break the integration in an unintended way.

Note:

See [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html) for details on this feature.

If the custom field security feature is turned on, SOAP web services will respect the access level set on each field. For example, if you have set a field permission to NONE, and you have code that references the field, you will not be able to read or write to that field in your code. NetSuite SOAP web services will essentially ignore that field when the SOAP request is sent. Similarly, if a field permission has been set to VIEW, you will be able to read the field's value, but you will be unable to set the field's value.

SOAP web services developers should keep custom field security in mind when designing their integrations. Before beginning a project, they should work with their company's NetSuite administrator to review which fields may have custom security applied.

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3445516.html)
-   [Authentication for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445710.html)
-   [Authorization for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447510.html)
-   [Session Management for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447680.html)
-   [Encryption for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448169.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
