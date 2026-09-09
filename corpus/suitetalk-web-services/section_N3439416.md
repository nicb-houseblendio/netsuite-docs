---
id: "section_N3439416"
type: "section"
title: "Default Field Values"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services > Default Field Values"
parent: "section_N3436475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439416.html"
anchors: ["bridgehead_N3439516"]
sha256: "82ae538c2084a9cc023924283768cede5a01c19d6a8590ae34cc61b23a00f3fc"
---

The system provides default values only for fields that are not required. When applying a default value, the system first tries to use a specified value. If none is given, the system uses the default. If no default is given, the system enters null.

User-defined defaults through the UI do not apply to SOAP web services.

Note:

For information about setting default values to custom fields, see [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html).

## Hidden Fields {#bridgehead_N3439516}

The SOAP web services API includes fields that are not visible in the NetSuite UI. In some cases, these fields have been hidden through point-and-click customization. In other cases, hidden fields are hidden by NetSuite. These types of hidden fields are used primarily for storing system-generated information such as dates.

For example, every SOAP-supported record contains either a _dateCreated_ or _createdDate_ field. These fields are not writeable. By default, these fields are populated with a system-generated timestamp. Note that system-generated dates and times are preserved for audit trail purposes.

Note:

The Use Defaults Web service preference does not affect the behavior of hidden fields. Even if the Use Defaults preference is not enabled, hidden fields are populated when a value is not supplied in the request. Also, for audit purposes, the true system date is always recorded for each record and cannot be overridden.

Important:

Calls to get or search (when the full record is returned) return the record in **edit** mode.

### Related Topics

-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Required Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html)
-   [Fields and Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
