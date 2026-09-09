---
id: "section_N2841053"
type: "section"
title: "Restricting Access to Custom Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Restricting Access to Custom Fields"
parent: "section_N2829580"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html"
anchors: []
sha256: "f7c929b34f6276e5e8673942439d199ce5de07d1f93762dc4c487d69375e9430"
---

You can control who can access the information in custom fields, enabling you to maintain the security of your business information. The access you define determines how the field can be accessed both on the record as well as through search results and reports.

You can control access to custom field data based on roles, departments, and subsidiaries. For details about how to set up these access restrictions, details about tracking access changes, or guidance for bundling custom fields with access restrictions, see the following topics:

-   [Setting Role, Department, or Subsidiary Access Restrictions for a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1106091633.html)
    
-   [Access Level History for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2842230.html)
    
-   [Bundling Fields with Access Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2842249.html)
    

Note:

When the Advanced Employee Permissions feature is enabled, use the **Employee Access** subtab to assign custom fields to custom advanced employee permissions. For more information, see [Restricting Access to Employee Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1514478336.html).

Access to a field can be based on role, department, or subsidiary. The following custom access levels can be assigned to each department and subsidiary.

-   **Edit** - The field and its contents can be viewed and changed.
    
-   **View** - The field can be seen, but its contents can't be changed. (The permission level affects how the form is accessed on records.)
    
-   **Run** - The field can be seen through reports and search results, but its contents can't be changed. (The permission is applicable only to reports and search.)
    
-   **None** - The field can't be seen, and its contents can't be changed.
    

For cases when various access levels are defined for a user's role, department, or subsidiary, the highest level of access is granted. For example, an employee is assigned to a department that has Edit access to a custom field, and the employee's role has been granted View access. The employee has the higher level of access - in the preceding example, Edit access.

In addition to search and reporting, the access level granted to a custom field includes instances where it's referenced by online forms, mail merge operations, and when it's sourced by other custom fields, or referred to by formula fields.

Note:

If you remove the administrator role's access to a custom field, the field won't be accessible to scripts that are run by an administrator. To access the field through scripting, you must edit and restore administrator access to the field.

You can set the level of access you want to grant by default to custom fields. The default access level applies to the roles, departments, and subsidiaries, that you don't define on the Role, Department, and Subsidiary subtabs.

To set default access, edit the custom field record, and click the Access subtab. In the Default Access Level, set the level of access you want to give by default. In the Default Level for Search/Reporting field, select the level of access you want to give through search and reporting.

The access you define on the Role, Department, and Subsidiary subtabs overrides the default access levels.

### Related Topics

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Setting Role, Department, or Subsidiary Access Restrictions for a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1106091633.html)
-   [Access Level History for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2842230.html)
-   [Bundling Fields with Access Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2842249.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
