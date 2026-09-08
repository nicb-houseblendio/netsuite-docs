---
id: "section_N326630"
type: "section"
title: "Using the Global Permissions Feature"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Permissions Overview > Using the Global Permissions Feature"
parent: "section_N325094"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326630.html"
anchors: ["procedure_N326647", "procedure_N326670"]
sha256: "74cc99e8b0cb9f9e23582e9e2e9cee9c518190f457c100d43ab32efac984263f"
---

The Global Permissions feature allows users with the Administrator role to assign permissions that apply across all of assigned roles of employees. With global permissions, users with the Administrator role can make changes to each employee's permissions directly on the employee record. Please note that usage of the Global Permissions feature is not preferred.

Note:

Not all permissions that are supported for assignment to roles are available for assignment as global permissions.

#### To enable the Global Permissions feature: {#procedure_N326647}

1.  Go to _Setup > Company > Setup Tasks > Enable Features_, and on the Employees tab, check the Global Permissions box.
    

When this feature is enabled, each employee record includes the Global Permissions subtab on the Access subtab.

#### To assign global permissions to an employee: {#procedure_N326670}

1.  After the Global Permissions feature has been enabled, open an employee record.
    
2.  Click the **Access** subtab, and the **Global Permissions** subtab.
    
3.  Select a permission from the **Permission** dropdown list, select an access level for that permission (**View**, **Create**, **Edit**, **Full**, **None**) from the **Level** dropdown list, and click **Add**.
    
    Note:
    
    For more information about the permission access levels, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).
    
4.  Repeat step 3 until you have added all desired permissions.
    
5.  Click **Save**.
    

You still need to assign one or more role to each employee on the Access subtab's Roles subtab. When an employee logs in, the applicable permission set is a combination of the employee's global permissions and the currently used role's permissions. Where conflicts between an employee's role-based permissions and global permissions occur, global permissions take precedence, even if global permissions are at a lower level.

The global permissions are not taken into account for the Administrator role. It is not possible to downgrade access for the Administrator role by using the global permissions.

### Related Topics

-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)
-   [Permissions and Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3781107123.html)
-   [Reviewing Permissions Assigned to Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326209.html)
-   [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html)
-   [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html)
-   [Core Administration Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540845284.html)
-   [Feature Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html)
-   [Giving Access to the Transactions Subtab on Entity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326821.html)
-   [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html)
-   [Hiding Employee Information on Financial Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4667963542.html)
-   [Setting Permissions for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327307.html)
-   [Permissions for Inbound Single Sign-on Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158206555854.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
