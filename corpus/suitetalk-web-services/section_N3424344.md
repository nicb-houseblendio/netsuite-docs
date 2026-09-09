---
id: "section_N3424344"
type: "section"
title: "Role and Permission Considerations When Developing in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Roles and Permissions in SOAP Web Services > Role and Permission Considerations When Developing in SOAP Web Services"
parent: "chapter_N3424144"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424344.html"
anchors: []
sha256: "b181cc1c740648e72bf6e6d4195d606c0836a6a997a8ef18b8096d176eb4c4d1"
---

Due to SOAP web services' being reliant on the NetSuite role-based permissions, SOAP web services developers should consider this during the design phase for smooth deployments.

Developers often use the administrator role during development for full permissions and access to all records and operations. However, the target users may have limited roles, restricting access to required data

Some roles' custom forms may lack access to fields or sublists needed by the SOAP application. This can cause permission errors when the application tries to access those fields.

Define a custom role and custom forms for the SOAP application to solve these problems. The custom role should have the correct access permissions and operations permissions that the SOAP web services application needs. The custom forms should give access to fields and sublists that are relevant to the SOAP application. All SOAP web services supported records have a `customForm` field for the application to reference specific custom forms.

Note:

In 2016.2, a permission has been added to the Role page on the Permissions > Setup subtab. If the Control SuiteScript and Workflow Triggers in Web Services Request permission is selected, users cannot change the setting for scripts and workflow triggers on individual SOAP web services requests. For users who don't have permission to disable scripts, the global setting for the account applies for all of their requests.

Important:

When testing SOAP web services applications, you should do so using the role(s) of your intended users(s), in addition to the administrator role, to catch permission-related defects.

### Related Topics

-   [Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html)
-   [Assigning the SOAP Web Services Permission to a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424476.html)
-   [Setting a Default Role for a SOAP Web Services User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424690.html)
-   [Setting a Web Services Only Role for a User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html)
-   [Customer Center, Vendor Center, and Partner Center Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427014.html)
-   [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
