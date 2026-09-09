---
id: "section_N1201405"
type: "section"
title: "Including CRM Tasks in Project Totals"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Tasks > Including CRM Tasks in Project Totals"
parent: "section_N1192913"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html"
anchors: ["bridgehead_N1201527"]
sha256: "8c0e5657889bae58d55961efcfeb971f48aa03170a55e3fe1f4649fc982cb084"
---

CRM tasks are "to do" activities that need to be completed. Each CRM task has its own record to track what needs to be done and who's responsible. You can assign CRM tasks to an employee, partner, or vendor.

CRM tasks can be associated with a project, but aren't considered part of the project's cost and time data unless they're explicitly included by checking the Include CRM Tasks in Project Totals box. CRM tasks associated with a project don't show up in the project schedule.

The Include CRM Tasks in Project Totals box on project records allows CRM tasks to contribute to the costs, work, and actual work for a project. This box helps accommodate existing, open projects which depend on CRM task records created prior to the 2008.2 release.

Important:

When you enable the Include CRM Tasks in Project Totals preference on a project, remember that task hierarchies only work within one task type. A CRM task can only be a parent or child of another CRM task. Project tasks and CRM tasks can't be parents or children of each other.

Note:

After the 2008.2 release, it is best to use project task records for costs, work, and actual work.

You must customize project forms to show the Include CRM Tasks in Project Totals box.

#### To customize a project form to use CRM tasks:

1.  Go to Lists > Relationships > Projects and click **Edit** next to the project.
    
2.  On the project form, click **Customize**.
    
3.  Enter a name for the form.
    
4.  Click the **Fields** subtab.
    
5.  Click the **Info** subtab.
    
6.  Check the **Show** box next to **Include CRM Tasks in Job Totals**.
    
7.  Complete other fields on the form as needed.
    
8.  Click **Save**.
    

Be sure to use this form for all projects that need to include CRM tasks. When you use the customized form to create a project record, you can check the Include CRM Tasks in Project Totals box.

Important:

If you have enabled the Gross Profit feature and Include CRM Tasks in Job Totals is also enabled, then the gross profit values will be inaccurate on the Financial subtab of the project record and on the sales order. This is because CRM tasks don't have prices associated with them. Only cost and time data is sourced from CRM tasks so the gross profit shown will be less than the real amount.

## Using Saved Searches for Project Tasks and CRM Tasks {#bridgehead_N1201527}

You can create saved searches to review combined data from project tasks and CRM tasks. Select the Project Task and CRM Task search type when defining the search parameters.

Other search types available for project information are Project, Project Task, and Task. For information about how to create a saved search, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).

You can create saved searches to provide project information to help you manage your projects and resources. If you want to view project data by employee across projects or project tasks, create a saved search that joins project task records to project task assignment records and select the fields to filter out the data you are looking for.

Additional data for project task assignment records aren't exposed in the application at the resource level but are available for search. This includes Actual Work and Estimated Work Baseline. These fields provide useful information for creating advanced searches for resource exposure and profitability by resource.

For example, you can create saved searches for:

-   Actual hours worked per resource for a specific task
    
-   Estimated work, estimated work baseline, and actual work performed by resource
    
-   Unit cost, unit price, estimated revenue, and gross profit by project or by resource
    

For a list of the project related record types available for creating advanced searches that join fields from different records, see [Related Records Fields Available for Advanced Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N651952.html).

### Related Topics

-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
-   [Project Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1192945)
-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Project Task Attributes Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1195767.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Scheduling Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199494.html)
-   [Importing Project Tasks from Microsoft Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200868.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
