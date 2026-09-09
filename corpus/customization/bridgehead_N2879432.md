---
id: "bridgehead_N2879432"
type: "bridgehead"
title: "Define the Permission Model for a Custom Record Type"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Specifying Permission and UI Settings > Setting Permissions for a Custom Record Type > Define the Permission Model for a Custom Record Type"
parent: "section_N2879388"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2879432.html"
anchors: []
sha256: "a0717569957b2889fe1394a92c0cd9f26144107a35b236b506cd6d9c2a63e3cd"
---

This topic explains the available models for controlling access to custom record types in NetSuite. Learn how to assign permissions based on roles, customize permission lists, and provide public access where needed.

You can use the **Access Type** list on a custom record type page to define a permissions model for a custom record type. You can base your permission model on any of the following:

-   Custom record entries permissions defined on role records
    
-   Permissions defined on the **Permissions** subtab of a custom record type
    
-   No permissions required for internal roles
    
    -   Permission level defined for external users, such as customers, vendors, and partners.
        
    -   Permission level defined for unauthenticated users (meaning users (for example, anonymous shoppers - online form users) who did not log in to NetSuite).
        

Note:

The No Permission Required access type has changed to No Permission Required for Internal Roles. For more information, see [Changes to 'No Permission Required' Access on Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0816050536.html).

The **Access Type** list includes the following options:

-   **Require Custom Record Entries Permission**
    
    -   This option is the default.
        
    -   Custom record types created prior to 2012.1 that did not have the **Use Permissions** box checked have this option set.
        
    -   This option indicates that only users logging in with a role with permission granted to the custom record type can access it. This permission can be set on the **Lists** subtab of the **Permissions** subtab on each Role page. For more information, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).
        
        Note that this limitation doesn't apply to the owner of the custom record type. The owner always has full permission to access the custom record type in any role.
        
-   **Use Permission List**
    
    -   Custom record types created prior to 2012.1 that had the **Use Permissions** box checked have this option set.
        
    -   This option indicates the users logging in with a role with permissions defined on the **Permissions** subtab of the custom record type can access it. This permission can also be set on the **Custom Records** subtab of the **Permissions** subtab on each Role page.
        
        Note that the owner of the custom record type isn't affected by this limitation. The owner always has full permission to access the custom record type in any role.
        
    -   For details about creating a permission list, see [Setting Up a Permissions List for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879931.html).
        
-   **No Permission Required for Internal Roles**
    
    -   Use this option for non-sensitive custom record types when you want to give all employees create, read, update, and delete access. This option denies external users or unauthenticated users from accessing the custom record type.
        
    -   New roles have immediate access to relevant custom record types without having to explicitly grant access.
        
    -   You can add custom access controls using SuiteFlow or SuiteScript.
        
    -   For more information, see [Changes to 'No Permission Required' Access on Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0816050536.html).
        
-   **External Roles Access**
    
    -   This option is available only if you selected No Permission Required for Internal Roles as the access type. It permits public access to users such as customers, vendors, and partners. The default access is None.
        
    -   **None** - User doesn't have access any instance of the custom record type. The user can't create new, view existing, edit existing, or delete existing instances.
        
    -   **View** - User has access to view existing instances of the custom record only. The user can't create new, edit existing, or delete existing instances.
        
    -   **Create** - User can create new and view existing instances of the custom record type. The user can't edit or delete existing instances.
        
    -   **Edit** - User has access to create new, view existing, and edit existing instances of the custom record type. The user can't delete existing instances.
        
    -   **Full** - User has access to create new files, and view, edit, and delete existing instances of the custom record type.
        
-   **Unauthenticated Users Access**
    
    -   This option is available only if you selected No Permission Required for Internal Roles as the access type. It permits public access to users (such as shoppers - online form users) who haven't logged in to NetSuite. The default access is None.
        
    -   **None** - User doesn't have access any instance of the custom record type. The user can't create new, view existing, edit existing, or delete existing instances.
        
    -   **View** - User has access to view existing instances of the custom record only. The user can't create new, edit existing, or delete existing instances.
        
    -   **Create** - User can create new and view existing instances of the custom record type. The user can't edit or delete existing instances.
        
    -   **Edit** - User has access to create new, view existing, and edit existing instances of the custom record type. The user can't delete existing instances.
        
    -   **Full** - User has access to create new files, and view, edit, and delete existing instances of the custom record type.
        

### Related Topics

-   [Setting Permissions for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879388.html)
-   [Changes to 'No Permission Required' Access on Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0816050536.html)
-   [Prevent Access to a Custom Record Type through the User Interface](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2879618.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
