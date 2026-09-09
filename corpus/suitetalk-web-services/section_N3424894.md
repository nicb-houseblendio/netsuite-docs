---
id: "section_N3424894"
type: "section"
title: "Setting a Web Services Only Role for a User"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Roles and Permissions in SOAP Web Services > Setting a Web Services Only Role for a User"
parent: "chapter_N3424144"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html"
anchors: ["procedure_N3424937", "bridgehead_N3424974"]
sha256: "66812b5d74680be4a5f37f8404dd8f30be49871aaac1aaf4904a92f01fff64bf"
---

In NetSuite you can designate a user's role as **Web Services Only**. For Web Services Only roles, login validation checks that access is through SOAP web services, not the UI.

Note:

Your account must have the SOAP web services feature enabled for the Web Services Only box to appear. See [Enabling the SOAP Web Services Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419926.html) for steps on enabling this feature.

The Web Services Only role increases the security by prohibiting a UI user from accessing the system with permissions and privileges created for a web services applications. For example, a web services application may require employees to have write access to certain records. However, you want to prevent them from editing these records directly in the NetSuite UI. If you assign the Web Services Only role to employees, the employees can log in to NetSuite and access the application through web services, however, the employees can¨t switch to their other roles and write, edit, or delete these data-sensitive records.

Important:

The Web Services Only role doesn't appear in the Change Role list. Users can't switch from their original UI role to a Web Services Only role within the UI.

#### To designate a role as Web Services Only: {#procedure_N3424937}

Note:

A **Web Services Only** role prevents UI access to NetSuite which enhances integration security. However, checking the **Web Services Only** box doesn't exclude access to NetSuite by other non-UI methods. Be aware that a **Web Services Only** role could combine with other access permissions. For example, Web Services Only role with SuiteAnalytics Connect permissions allows ODBC access.

1.  Click _Setup > Users/Roles > Manage Roles_.
    
2.  On the Manage Roles list page, locate the role you want to set as Web Services Only.
    
3.  Click **Edit** or **Customize**.
    
4.  Check the **Web Services Only Role** box.
    
5.  Click **Save**.
    

## When to Set the Web Services Only Role {#bridgehead_N3424974}

Delay designating a role as **Web Services Only** until the integrated application is complete. This delay allows developers to test permissions during design and development. When development is complete, set Web Services Only to TRUE to restrict UI access for the specified role.

Note:

External roles such as Customer Center, Partner Center, Advanced Partner Center, Vendor Center, and Employee Center shouldn't be customized to have Web Services Only permissions.

### Related Topics

-   [Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html)
-   [Role and Permission Considerations When Developing in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424344.html)
-   [Assigning the SOAP Web Services Permission to a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424476.html)
-   [Setting a Default Role for a SOAP Web Services User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424690.html)
-   [Customer Center, Vendor Center, and Partner Center Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427014.html)
-   [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
