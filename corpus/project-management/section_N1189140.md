---
id: "section_N1189140"
type: "section"
title: "Assigning Project Resources"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Working with Resources in Project Management > Assigning Project Resources"
parent: "section_N1187445"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html"
anchors: ["bridgehead_N1189256", "bridgehead_N1189443", "bridgehead_N1189556"]
sha256: "1750cab72bb087188c94de317d03e517d28d3d3aabffcd5b3894bb66e56e53b5"
---

After you begin [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html), you can then assign resources to projects and tasks as needed. Resources assigned to a project can enter time against the project. You can calculate resource productivity based on reported time.

While assigning resources, you can use the Target Utilization feature for each Project Resource. For more information, see [Utilization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html#bridgehead_N1191029).

You can also assign generic resources to projects and tasks when you haven't selected a specific person yet. Add generic resources the same way you add regular project resources. For more information, see [Generic Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3897338492.html).

Important:

If you use Resource Allocations, you have to allocate a defined resource to a project before you can assign them to tasks. You can add generic resources to a task even if they're not allocated. For more information, see [Resource Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html).

You can also allocate resources directly to project tasks. For each project, it's best that you choose to either allocate resources directly to project tasks or allocate resources to the project and then assign to project tasks. Using both resource allocations to project tasks and task assignments can create inconsistencies in your project data. For more information, see [Assigning Resources with Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html#bridgehead_4362895283).

Assigning resources works in conjunction with other project preferences you select on the Preferences subtab when you create the project record.

-   **Allow Time Entry** - This preference determines whether time can be entered against the project. You must enable this preference for anyone to record time against a project for billing purposes.
    
    If you select this preference and the Limit Time and Expenses to Resources preference, then only resources listed on the project can enter time.
    
-   **Display All Resources for Project Task Assignment** - Enable this if you want to be able to select from a list of all employees and vendors designated as project resources or previously assigned to any project when assigning resources to project tasks.
    
    Important:
    
    Available project resources and generic resources may be limited by the Employee Restrictions field for any custom roles used to assign resources to the project. For more information, see [Setting Employee Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637690919.html).
    
    After you assign a resource to a project, if you clear the Project Resource box, they'll still be available if you use the Display All Resources for Project Task Assignment preference when creating your project in NetSuite.
    
    If this option isn't enabled, then you can assign only resources listed on the Resource subtab of the project to a project task.
    
    Note:
    
    If you use Resource Allocations, enabling this preference means you don't have to allocate resources before assigning them to tasks. Disabling this preference requires you to allocate defined resources prior to making task assignments. Generic resources can always be assigned to tasks, even if they're not allocated.
    
-   **Limit Time and Expenses to Resources** - This preference determines whether only resources assigned to the project can enter time and expenses against the project and its project tasks.
    
    If you select this preference and Display All Resources for Project Task Assignment, then any resource you assign to a task is automatically added to the Resources subtab and can enter time for the project.
    

You have two options when assigning resources to project tasks. Based on how you set the Display All Resources for Project Task Assignment option for the project, you can assign resources from a list of either:

-   Resources designated on the project record only - see [Assigning Resources Restricted to the Project](#bridgehead_N1189256)
    
-   All project resources - see [Assigning Resources not Restricted to the Project](#bridgehead_N1189443)
    

## Assigning Resources Restricted to the Project {#bridgehead_N1189256}

If you don't select Display All Resources for Project Task Assignment, follow these steps. You can only assign resources that are on the Resources subtab of the project record.

#### To assign resources to the project:

1.  Go to Lists > Relationships > Projects and click **Edit** next to the project.
    
2.  Click the **Resources** subtab.
    
    Note:
    
    If you use Resource Allocations you must first allocate a defined resource to a project before you can assign them to tasks. Generic resources are available for task assignment regardless of project allocation. For more information, see [Resource Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html).
    
3.  In the **Name** column, select the employee or vendor you want to add as a resource.
    
    Note:
    
    An employee or vendor name shows in this list only if they're marked as a Project Resource. For more information, read [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html).
    
4.  In the **Role** column, select a project role for this resource. For more information about project roles, read [Creating a Project Resource Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html).
    
    You can select multiple roles for a single resource by holding down Ctrl while selecting roles with your mouse.
    
5.  If you use Job Costing and Project Budgeting, a cost associated with the selected role or employee fills in automatically. In the **Cost Override** column, you can enter a new cost for this project.
    
6.  Click **Add**.
    
7.  Repeat steps 3 through 5 for each resource you want to assign to this project.
    
8.  Click **Save**.
    

#### To assign resources to project tasks:

1.  Go to Lists > Relationships > Projects and click **Edit** next to the project.
    
2.  On the **Schedule** subtab, click **Edit** next to the task you want to assign resources to.
    
3.  In the Project Task window, click the **Assignees** subtab.
    
4.  In the **Resource** column, select the employee or vendor you want to add as a resource.
    
    Note:
    
    The Resource dropdown displays only the resources that you added to the Resources subtab of this project. If you use Resource Allocations, only allocated defined resources and all generic resources are displayed. For more information, see [Resource Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html).
    
5.  Select the service item required for this resource on this task.
    
6.  Enter a unit cost and unit price for this service item on this task.
    
7.  Click **Add**.
    
8.  Repeat steps 4 through 7 for each resource you want to assign to this task.
    
9.  Click **Save**.
    

Each assigned resource may have a different amount of work on the task and may work at a different rate, such as full-time or half-time. The percentage of time the employee dedicates to a single task is often referred to as their 'full-time equivalent.'

You can also use resource groups to assign multiple resources to a project task at one time. For more information, see [Creating Resource Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547067026.html).

## Assigning Resources not Restricted to the Project {#bridgehead_N1189443}

If the Display All Resources for Project Task Assignment option is selected for a project, then you can assign any designated project resource. This includes any employee or vendor identified as a project resource on the entity record.

Important:

After you assign a resource to a project, if you clear the Project Resource box, they'll still be available if you use the Display All Resources for Project Task Assignment preference when creating your project in NetSuite.

#### Assign resources to project tasks:

1.  Go to Lists > Relationships > Projects and click **Edit** next to the project.
    
2.  On the **Schedule** subtab, click **Edit** next to the task you want to assign resources to.
    
3.  In the Project Task window, click the **Assignees** subtab.
    
4.  In the **Resource** column, select the employee or vendor you want to add as a resource.
    
    Note:
    
    Employees and vendors show up in this list only if they've been marked as a Project Resource, For more information, read [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html).
    
5.  Select the service item required for this resource on this task.
    
6.  Enter a unit cost and unit price for this service item on this task.
    
7.  Click **Add**.
    
8.  Repeat steps 4 through 7 for each resource you want to assign to this task.
    
9.  Click **Save**.
    

Each assigned resource may have a different amount of work on the task and may work at a different rate, such as full-time or half-time. The percentage of time the employee dedicates to a single task is often referred to as their 'full-time equivalent.'

You can also use resource groups to assign multiple resources to a project task at one time. For more information, see [Creating Resource Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547067026.html).

## Overbooking and Underbooking {#bridgehead_N1189556}

Note that resource assignment isn't automatically limited by the time constraints of that resource. For example, someone who works 20 hours a week can still be assigned to 50 hours of tasks. You must assess time reports to determine if resources are under or over their planned utilization across multiple tasks or projects.

For example, Brenda might be scheduled for Task 1 full-time next week (40 hours). You can still assign her to Task 2 full-time for the same week, even though she'll only work 40 hours total.

After resources are assigned on projects and begin to enter time against it, you can do the following:

-   View the progress of the project by clicking View Gantt Chart on the Schedule subtab of the project record.
    
-   Monitor resource productivity by running the [Utilization by Resource Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3748733226.html).
    

### Related Topics:

-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Identifying an Employee as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188347.html)
-   [Identifying a Vendor as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188644.html)
-   [Creating a Project Resource Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html)
-   [Working with Project Management in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182865.html)
-   [Creating Resource Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547067026.html)
-   [Project Resource Work Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189731.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
