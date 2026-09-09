---
id: "chapter_N3424144"
type: "chapter"
title: "Roles and Permissions in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Roles and Permissions in SOAP Web Services"
parent: "book_156388532579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html"
anchors: []
sha256: "d1254ae8c714e77bd6fb54c97548a8b6e31d4071a2073d72e8643f605653b109"
---

NetSuite provides many standard roles with predefined permissions. A role is a set of permissions that allows customers, vendors, partners and employees access to specific aspects of your data. Each role grants access at a certain level for each permission.

You can provide a **role id** with your **credentials** when logging in with SOAP web services. The provided role ID must have SOAP web services permissions to avoid an **INSUFFICIENT\_PERMISSION** error. If no role ID is provided, the user's default role is used. Without SOAP web services permissions in the default role, a **ROLE\_REQUIRED** fault is returned.

The following topics are provided in this section. They don't need to be read in order. If you're new to NetSuite SOAP web services, reading each topic will help you understand how roles and permissions work.

-   [Role and Permission Considerations When Developing in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424344.html)
    
-   [Assigning the SOAP Web Services Permission to a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424476.html)
    
-   [Setting a Default Role for a SOAP Web Services User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424690.html)
    
-   [Setting a Web Services Only Role for a User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html)
    
-   [Customer Center, Vendor Center, and Partner Center Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427014.html)
    
-   [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html)
    

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
