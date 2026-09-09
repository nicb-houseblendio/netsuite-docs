---
id: "section_N1199176"
type: "section"
title: "Identifying Parent Tasks"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Tasks > Identifying Parent Tasks"
parent: "section_N1192913"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html"
anchors: []
sha256: "df44b2495aef5eb76b0a0ab75ffe8305e3ef97546e0368fdcca415bd2264a63f"
---

Organize project tasks in a hierarchy of parent tasks and subordinate tasks to structure the component parts of a project.

Tasks can be one of the following:

-   Work task - A task record that tracks actual project activity, such as time worked.
    
-   Parent task - A task record that only tracks cumulative information about subordinate tasks that are required to complete a project.
    

For example, if you need to manage an installation project that is composed of 3 individual tasks, you can set up task records as follows:

-   First, create a task record for the installation. This task will become a parent task record after you identify it as the parent of other tasks.
    
-   Next, enter a work task for each of the three individual tasks. Identify each task as a subordinate of the installation task by selecting it as the parent.
    

Employees enter their time on each child task. The parent task then sums up the data from all its child tasks.

Note:

There must be at least one task already associated with the project before the Parent Task field appears.

Important:

You can't assign resources to a parent task because it doesn't track work directly. Parent tasks only track other tasks.

Parent task records track the following data sourced from its subordinates:

-   Start Date - the earliest start date of all subordinate tasks
    
-   End Date - the latest end date of all subordinate tasks
    
-   Estimated Work - the cumulative total estimated work for all subordinate tasks
    
-   Actual Work - the cumulative total actual work done for all subordinate tasks
    
-   Remaining Work - the cumulative total work remaining for all subordinate tasks
    
-   Percent Complete - the overall percentage of work completed
    

If you use Resource Allocations, the Allocated Work and Percent Complete by Allocated Work fields are also sourced from parent task subordinates.

To set up parent and subordinate tasks, open the task record and select a parent in the Parent Task field.

When you view the task list on a project record, each parent tasks shows its subordinates indented beneath it.

![ParentTasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/ParentTasks.png)

Note:

If you use [CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1194713) with projects, please read [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html) regarding task hierarchies.

### Related Topics

-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
-   [Project Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1192945)
-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Project Task Attributes Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1195767.html)
-   [Scheduling Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199494.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Importing Project Tasks from Microsoft Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200868.html)
-   [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
