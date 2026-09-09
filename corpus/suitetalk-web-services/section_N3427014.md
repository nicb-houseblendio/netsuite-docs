---
id: "section_N3427014"
type: "section"
title: "Customer Center, Vendor Center, and Partner Center Roles"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Roles and Permissions in SOAP Web Services > Customer Center, Vendor Center, and Partner Center Roles"
parent: "chapter_N3424144"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427014.html"
anchors: ["procedure_N3427047"]
sha256: "ef511568c4809af9dd072dabb59b3bc80f821ad680d63e948a00f439e42dcde5"
---

The Customer, Vendor, and Partner Center roles have built-in SOAP web services permissions. This enables integration with external websites, allowing clients to perform tasks through SOAP web services. For example, the client could login and submit an order on the customer's behalf.

Note:

You shouldn't customize Customer Center, Partner Center, or Partner Center Roles to have only Web Services Only permissions. For information about the Web Services Only role, see [Setting a Web Services Only Role for a User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html).

You can remove SOAP web services permissions from the Customer, Vendor, and Partner Center roles if needed.

#### To remove SOAP web services permissions: {#procedure_N3427047}

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Locate the role you want to modify.
    
3.  Click **Edit** or **Customize**.
    
4.  Click the **Setup** subtab.
    
5.  In the **Permissions** list, click the **SOAP Web Services** line to make it editable.
    
6.  In the **Level** column, select the value **None** from the list.
    
7.  Click **OK** to stop editing the SOAP Web Services line.
    
8.  Click **Save**.
    

### Related Topics

-   [Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html)
-   [Role and Permission Considerations When Developing in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424344.html)
-   [Assigning the SOAP Web Services Permission to a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424476.html)
-   [Setting a Default Role for a SOAP Web Services User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424690.html)
-   [Setting a Web Services Only Role for a User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html)
-   [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
