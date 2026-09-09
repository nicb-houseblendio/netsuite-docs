---
id: "section_N3424690"
type: "section"
title: "Setting a Default Role for a SOAP Web Services User"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Roles and Permissions in SOAP Web Services > Setting a Default Role for a SOAP Web Services User"
parent: "chapter_N3424144"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424690.html"
anchors: ["procedure_N3424751"]
sha256: "338a8251a73de2adf491620aef5e18cbf5ed43e60b1a945c7dd5b3d800c5a9d0"
---

A default role can be set for users making SOAP web services requests. Default role permissions are determined by the following rules:

-   If no role is specified in the request, the default SOAP web services role from the user's Web Services Preference page is used.
    
    Each user can have only one default SOAP web services role, which must include the SOAP web services permission. The assigned role may differ from the one in the user's employee record. This means SOAP web services permissions can be different from UI permissions.
    
-   If no role is specified in the request or as a default, a role is selected based on the following order:
    
    -   A non-Customer Center role in the account, indicated as the default role.
        
    -   A non-Customer Center role in the account, selected based on the last login date.
        
    -   A Customer Center role in the account, indicated as the default role.
        
    -   A Customer Center role in the account, selected based on the last login date.
        

Note:

All standard roles have the SOAP web services permission by default when the SOAP web services feature is enabled. Custom roles, however, must be explicitly set to have SOAP web services permissions. For information about creating custom roles, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)

#### To set a specific default role for a SOAP web services user: {#procedure_N3424751}

1.  Go to _Setup > Integration > Integration Management > SOAP Web Services Preferences_.
    
2.  Select the user from the **Name** list.
    
3.  Select the default role to use for SOAP web services requests for this user.
    
    The internal ID for the selected role automatically populates the **ID** field.
    
4.  Click **OK**.
    
5.  Click **Save**.
    

### Related Topics

-   [Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html)
-   [Role and Permission Considerations When Developing in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424344.html)
-   [Assigning the SOAP Web Services Permission to a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424476.html)
-   [Setting a Web Services Only Role for a User](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3424894.html)
-   [Customer Center, Vendor Center, and Partner Center Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427014.html)
-   [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
