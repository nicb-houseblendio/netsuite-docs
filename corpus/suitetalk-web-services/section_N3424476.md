---
id: "section_N3424476"
type: "section"
title: "Assigning the SOAP Web Services Permission to a Role"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Roles and Permissions in SOAP Web Services > Assigning the SOAP Web Services Permission to a Role"
parent: "chapter_N3424144"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424476.html"
anchors: ["procedure_N3424492"]
sha256: "a521394113e2ce4e6384128e4c23399f1e3acd2d207d856832985b90d4262f93"
---

Most standard NetSuite roles have SOAP web services permissions by default. For security reasons, you should restrict permissions level to the minimum required for a specific set of operations. For more details, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

For non-standard or custom roles, use these steps to assign the SOAP web services permission to the role.

#### To assign the SOAP Web Services permission to a role: {#procedure_N3424492}

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Locate the role you want to modify. Click **Edit** or **Customize**.
    
3.  Click the **Setup** subtab.
    
4.  In the **Permissions** dropdown list, select **SOAP Web Services**.
    
5.  In the Level dropdown list, select **Full**.
    
    Note:
    
    Users with a SOAP Web Services permission level other than Full (View, Create, Edit) can't log in to SOAP web services. The Full level is required. Also note that the SOAP Web Services permission doesn't provide access to the SOAP Web Services Usage Log or to integration records; only administrators can access these pages. For details on the SOAP Web Services Usage Log, see [Using the SOAP Web Services Usage Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444819.html). For details on working with integration records, see [SOAP Web Services Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3445516.html).
    
6.  Click **Add**.
    
7.  Click **Save**.
    

Note also:

-   When building an integrated application, create a new role or customize an existing one with minimal necessary permissions. Avoid assigning administrator privileges for SOAP web services use.
    
-   With permission to view credit card data in the UI, you can also retrieve it through SOAP web services calls. This benefits integrated applications using external credit card processing profiles. Based on your role, you may be able to retrieve the credit card on file for your customers.
    
-   To use getDeleted, a role needs both Deleted Records and SOAP Web Services permissions. Users with Deleted Records permission can access deleted record results, regardless of their permission to create or modify that record type. They can also use the Deleted Record search type, unless the Web Services Only option is selected
    

### Related Topics

-   [Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html)
-   [Role and Permission Considerations When Developing in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424344.html)
-   [Setting a Default Role for a SOAP Web Services User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424690.html)
-   [Setting a Web Services Only Role for a User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html)
-   [Customer Center, Vendor Center, and Partner Center Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427014.html)
-   [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
