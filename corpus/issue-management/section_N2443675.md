---
id: "section_N2443675"
type: "section"
title: "Creating Issue Role Types"
branch: "issue-management"
category: "support-management"
breadcrumb: "Support Management > Issue Management > Creating Issue Role Types"
parent: "chapter_N2438260"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2443675.html"
anchors: ["procedure_N2444102"]
sha256: "3721e2aafb8272082b94fd50f561a29d47f3bda7a0489c230164a9fc64d1d5b9"
---

You can create issue role types to set defaults for groups or employees who use issue records regularly. An issue role type defines what settings an employee can place on an issue record. For example, whether they can mark issues as Fixed or be selected in the Reviewer field.

When you create a new issue role type, user with the Administrator role must associate the issue role with a user role. They can do this at _Setup > User/Roles > User Management > Manage Roles_.

The following default user roles are already associated with issue role types:

-   Engineer
    
-   Engineering Manager
    
-   QA Engineer
    
-   QA Manager
    
-   Product Manager
    
-   PM Manager
    
-   Support Person
    
-   Support Manager
    
-   Issue Administrator
    

To give employees access to issues, you can choose to assign a default role to the employees on the employee record. You can also assign an issue role type to the employee's user role at _Setup > Users/Roles > User Management > Manage Roles_.

To edit or customize a role to give access to issue records, select the issue role with the access you need.

| Issue Role Type (assigned on role) | User Role (assigned on employee record) | Issue Permissions of User Roles |
| --- | --- | --- |
| Development | Engineer Engineering Manager | Issue Reports Edit/Create Issue Records Mark Issues as Showstoppers |
| Quality Assurance | QA Engineer QA Manager | Issue Reports Edit Issue Records Mark Issues as Showstoppers |
| Product Management | Product Manager PM Manager | Issue Reports Edit/Create Issue Records Mark Issues as Showstoppers |
| Support | Support Person Support Manager | Edit/Create Issue Records |
| Administrator | Issue Administrator | Issue Reports Edit/Create Issue Records Mark Issues As Showstopper Issue Setup (statuses, issue roles, etc.) |

You can issue role types to determine how each type of employee can edit issues using the Manage Status Transitions page. For more information, see [Managing Issue Status Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444542.html).

#### To create an issue role type: {#procedure_N2444102}

1.  Go to _Setup > Issues > Issue Roles > New_.
    
2.  In the **Issue Role** field, select the name of this issue role type.
    
    You can select this role in Issue Role fields when you create or edit user roles, employee groups, and status transitions. You'll also be able to select this role type in the **Assigned To** column when you create or edit issue statuses.
    
3.  In the **Description** field, enter a brief description defining the purpose of this issue role.
    
4.  Check the **Administrator** box if employees with this role type should have access the following pages used for setting up the Issue Management feature:
    
    -   Set Up Issues
        
    -   Issue Statuses
        
    -   Issue External Statuses
        
    -   Issue Severities
        
    -   Issue Priorities
        
    -   Issue Types
        
    -   Issue Sources
        
    -   Issue Reproducibility
        
    -   Issue Tags
        
    -   Products
        
    -   Issue Roles
        
    -   Manage Status Transitions
        
5.  Check the **Reviewer** box if employees using this role type should be available for selection in the Reviewer field on issue records.
    
6.  Check the **Can Fix Issues** box to let employees with this role to set issue statuses to a base status of Resolved.
    
7.  Check the **Restrict Assignees** box to let only employees with this role type to assign issues to other employees with this role type.
    
    Note:
    
    To assign an issue to another role type, note the following: Employees using role types with this preference must change the status to an issue status linked to another role type.
    
8.  In the following fields, you can set the default selections for this role type for the respective fields on issue records:
    
    -   **Severity** - Create and edit selections for this list at _Issues > Setup > Issue Severities_.
        
    -   **Priority** - Create and edit selections for this list at _Issues > Setup > Issue Priorities_.
        
    -   **Type** - Create and edit selections for this list at _Issues > Setup > Issue Types_.
        
    -   **Source** - Create and edit selections for this list at _Issues > Setup > Issue Sources_.
        
    -   **Reproduced** - Create and edit selections for this list at _Issues > Setup > Issue Reproducibility_.
        
    -   **Product** - Create and edit products at _Issues > Setup > Products_.
        
    -   **Module** - Create and edit modules for products at _Issues > Setup > Products_.
        
    -   **Broken In** , **Target**, and **Fixed In Version and Build** - Create and edit product versions. You do this on the **Versions** subtab of product records at _Issues > Setup > Products_.
        
9.  Click **Save**.
    

### Related Topics

-   [Issue Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2439679.html)
-   [Issue Management Setup Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2439844.html)
-   [Getting Started With Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2440450.html)
-   [Setting Issue Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441221.html)
-   [Setting Up Issue Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441539.html)
-   [Creating an Issue External Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442071.html)
-   [Setting Up Issue Severities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442248.html)
-   [Setting Up Issue Priorities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442386.html)
-   [Setting Up Issue Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442528.html)
-   [Setting Up Issue Sources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442704.html)
-   [Setting Up Issue Reproducibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442842.html)
-   [Setting Up Issue Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442980.html)
-   [Working with Products and Modules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2443140.html)
-   [Managing Issue Status Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444542.html)
-   [Creating Employee Groups for Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444787.html)
-   [Customizing Issue Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445049.html)
-   [Logging Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445262.html)
-   [Linking Issues with Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445726.html)
-   [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html)
-   [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
