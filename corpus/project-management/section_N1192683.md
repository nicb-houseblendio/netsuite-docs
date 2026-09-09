---
id: "section_N1192683"
type: "section"
title: "Approving Time and Expenses for Projects"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Managing Time and Expenses for Project Resources > Approving Time and Expenses for Projects"
parent: "section_N1190979"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192683.html"
anchors: ["subsect_1519328676"]
sha256: "271ae3a4b7a04f136d67aaefc2c8c3da41b89d2d0baad3c266824060e9c6e9c1"
---

Approve resource time and expense transactions for a project to process payroll and bill customers for billable charges. With Project Management and Time Tracking, a project manager or time approver can approve time entries, and the employee's supervisor or expense approver can approve expenses.

Note:

Project time approvers can only approve time for projects in which they are assigned a role with project time approval permissions.

For example, if someone is the project manager but not the supervisor for any resources assigned to the project, they can approve time entries for the project but can't approve expense reports charged to the project.

Identify default approvers for employee time and expense reports on the Human Resources subtab of the employee record. If there's no designated approver, the employee's supervisor must approve expense reports. Project time approval depends on your approval preferences. See [Entering Human Resources Information for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N895403.html).

Project time approvals are dependent on project resource roles. On the project resource role record, the Project Time Approver preference determines if project resources with that role can approve time. The Own Time Approval setting means time entered with this role is automatically approved. The Project Manager resource role has both preferences enabled by default.

#### To add project time approval permissions to a project resource role:

1.  Go to _Setup > Accounting > Project Resource Roles_.
    
2.  Click **Edit** next to the role you want to update.
    
3.  Check the **Project Time Approver** box.
    
4.  Check the **Own Time Approval** box to automatically approve any time tracked on projects by employees with this role. If you clear this box, any time entered toward a project by a resource with this role will need to be approved by the resource's manager or a project level approver.
    
5.  Click **Save**.
    

Note:

When you add time approval permissions to a role, you don't need to update project assignments. Anyone with the edited role now has time approval permissions for the projects in which they're assigned that role.

After you've enabled project time approval for your roles, you can also select who has approval privileges for each project.

#### To set time approval preferences by project:

1.  Go to _Lists > Relationships > Projects_.
    
2.  Click **Edit** next to the project you want to update.
    
3.  Click **Preferences**.
    
4.  In the **Time Approval** field, select one of the following options:
    
    -   Approve time automatically - Project time is approved automatically when entered from the Employee Center or a time restricted role.
        
    -   Default Time Approver - Project time can be approved only by each employee's supervisor or time approver defined on the employee record.
        
    -   Project Time Approver - Project time can be approved only by project resources with project time approval permission defined on the project resource role.
        
    -   Project Time Approver or Default Time Approver - Both project time approvers and default time approvers can approve project time. This option is selected by default.
        
5.  When you're done, click **Save**.
    

Important:

The Time Approval setting doesn't override roles with full time permissions. Anyone with full time and unrestricted employee permissions can approve or reject time entries for any employee, no matter your selection in this field. Also, automatic approvals aren't available for full time permission roles. You'll need to update the Approval Status or submit a weekly timesheet. For more information about permissions, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html) and [Setting Employee Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637690919.html).

The default selection in the Time Approval field is Project Time Approver or Default Time Approver.

Since billable project time must be approved before you can bill customers, review the Time Approval page regularly. Time in Time Tracking is used to calculate actual time worked on tasks, whether it's approved or not

## Project Time Approval Permissions {#subsect_1519328676}

When you use project-based time approval, the way time is approved for each resource depends on how you set up your approval preferences on both your project resource roles and each project.

Any project resource role that doesn't have the Project Time Approver box checked can't approve any time transactions. See the table below for information about how approval permissions are affected based on your resource role and project preferences.

| Selected Project Time Approval Preference | Approve and Receive Notifications | Approver for Roles with Approval Privileges |
| --- | --- | --- |
|  |  | On | Off |
| Approve time automatically | N/A | Automatically Approved | Automatically Approved |
| Default Time Approver | No | Default Time Approver | Default Time Approver |
| Project Time Approver | Yes | Automatically Approved | Other Project Time Approver |
| Project Time Approver or Default Time Approver | Yes | Automatically Approved | Default or Other Project Time Approver |

#### To approve time related to a project:

1.  Go to _Transactions > Employees > Approve Time_.
    
2.  Select an employee or **All**.
    
3.  If you use Time Tracking, check the **Approve** box for time you want to approve. Click **Submit**.
    
    For more information about time approval with Time Tracking, see [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html).
    
    Note:
    
    If you use Time Tracking and enter time for your employees, then you can alternately check the **Supervisor Approval** box when entering time entries.
    

#### To approve employee expense for a project:

1.  Log into the Employee Center.
    
2.  Go to Expense Reports > Approve Expense Reports.
    
3.  Select the name of the employee who submitted the report.
    
4.  Check the box next to the expense report you want to approve.
    
5.  Click **Save**.
    
    For more information about approving expense reports, see [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html).
    

### Related Topics:

-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)
-   [Entering Time Against Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1191698.html)
-   [Entering Human Resources Information for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N895403.html)
-   [Creating a Project Resource Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html)
-   [Setting Up Project Record Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4585905289.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
