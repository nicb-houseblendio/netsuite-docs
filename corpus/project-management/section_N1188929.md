---
id: "section_N1188929"
type: "section"
title: "Creating a Project Resource Role"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Working with Resources in Project Management > Creating a Project Resource Role"
parent: "section_N1187445"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html"
anchors: []
sha256: "495caaff1c0d1ea3ad49b970ac9921295ae3b48fd5b441d773a6ce0912909e67"
---

When you identify an employee or vendor as a resource on a project, you can identify their role for that project.

For example, create a project resource role called **Assistant Manager.** Then, you can assign the Assistant Manager role to one of the resources for a project.

Note:

When assigning resources to a project, you can select multiple project roles for a single resource using a multi-select field.

Multi-select for the Role field isn't available when using SuiteScript or SOAP web services for project tasks. Multiple roles are accessible using SuiteScript or SOAP web services with each resource listed one time for each assigned role.

To select project resource roles on projects, you must first create resource role records.

#### To create a project resource role record:

1.  Go to Setup > Accounting > Project Resource Roles > New.
    
2.  Select **Project Resource Role**.
    
3.  Enter a name for the role. This is the name that appears in the Role dropdown on projects.
    
    For example, enter Assistant Manager.
    
4.  Enter a description for the role.
    
5.  Check the **Allow Replacing Task Assignments in Bulk** box to enable employees with this role to reassign project tasks in bulk.
    
6.  If you also use Resource Allocations and Time-Off Management, check the **Send E-mail Notification if Time-off Collides with Project Resource Allocation** box to send notifications to employees assigned this role when resource allocations for projects conflict with approved time off.
    
7.  Check the **Project Time Approve** box to enable employees with this role to approve project time for the projects in which they are assigned this role.
    
8.  Check the **Own Time Approval** box to automatically approve any time tracked by employees with this role. If you clear this box, any time entered toward a project by a resource with this role will need to be approved by the resource's manager or a project level approver.
    
9.  Click **Save**.
    

Now you can assign this project resource role to resources on your projects.

### Related Topics:

-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Identifying an Employee as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188347.html)
-   [Identifying a Vendor as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188644.html)
-   [Assigning Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html)
-   [Project Resource Work Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189731.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
