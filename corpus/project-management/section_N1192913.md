---
id: "section_N1192913"
type: "section"
title: "Project Tasks"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Tasks"
parent: "part_3746040281"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html"
anchors: ["bridgehead_N1192945", "bridgehead_N1194466", "bridgehead_3739383427", "procedure_N1194478", "procedure_N1194583", "bridgehead_3898990487", "procedure_N1194636", "bridgehead_N1194659", "bridgehead_N1194685", "bridgehead_N1194697", "bridgehead_N1194713", "bridgehead_N1194777", "bridgehead_N1194797"]
sha256: "ae718901a6a1244df6b970aaf14e7e82da74a1c855256a36d5e5602c9d972cf7"
---

When you use the Project Management feature, you can create project task records to track the activities you need to finish. Project tasks are the individual steps you need to complete to reach your goal. A project is finished when all the project tasks are completed.

When you're creating your project record, create a project task for each activity you need to accomplish to finish the project.

Important:

You should break up long, multi-year projects into smaller parts to improve performance when working with project records.

You can't create project tasks on their own, they must be linked to a project record. Project tasks help with project planning and are only created on the project record.

Tasks you create with Project Management can also collect information automatically. For example, you can track the time budgeted and remaining for a task and calculate what percent has been completed.

## Project Task Records {#bridgehead_N1192945}

Project tasks list all of the actions you must complete to reach your goal. Enter a task record for each project task you need to complete.

For example, to track a basic office furniture sales and delivery project, you could create a task record for each of the following:

-   Order Items From Supplier
    
-   Assemble Items
    
-   Furniture Delivery and Installation
    
-   Bill Customer For Delivery and Items
    

After you've created a project record, you can create task records for each task needed to finish the project. On the Schedule subtab of a project record, click New Project Task to create a new task.

![NewProjTaskButton](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/NewProjTaskButton.png)

Note:

The Schedule subtab appears only after you save a project record.

The previous example was a simple four-task project, but most projects are more complex and need more details to be tracked. When you have lots of details to enter, it's best to keep everything organized so that the task runs smoothly.

The task record you create has all the information you need to know, such as the type of task, duration, dependency on other tasks, start and finish dates, and assigned resources.

Assign resources and define the service type, cost, and estimated work. NetSuite uses this information to price project work and figure out the expected gross margin. You can assign more than one resource to a task.

Note:

You can only select non-fulfillable or receivable service items for project tasks.

The estimated work for the task must be specified in hours. Similarly, service items to be used on the project task must be priced in hours.

For more details about creating a task record, read [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html).

### Organizing Tasks {#bridgehead_N1194466}

Some tasks are goals with their own sub-tasks. To keep these tasks organized, group them based on which ones should be completed together and set up task hierarchies.

### Milestones {#bridgehead_3739383427}

Project milestones mark key points in your project, like finishing a group of tasks, or serve as a project health check to determine if you're on schedule.

Project milestones can't have estimated hours, assignees, or a Finish No Later Than (FNLT) constraint. When viewing a project Gantt chart or schedule, milestone tasks look different from regular project tasks.

For more information, see [Creating Milestone Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740066806.html).

### Parent Tasks and Work Tasks {#procedure_N1194478}

When you're creating project task records, you can organize tasks in a hierarchy of parent tasks and subordinate tasks to structure the component parts of a project. Tasks can be one of the following:

-   Work task - A task record that tracks project activity, such as time worked.
    
-   Parent task - A task record that only tracks cumulative information about subordinate tasks that are required to complete a project.
    

On task records, you can select a parent in the Parent Task field to set up a hierarchy of tasks and subordinate tasks. Then, parent tasks are summary tasks only, have no resources assigned, and only track cumulative data about subordinate tasks.

For example, you can create the task Build fence. Then, create these tasks:

-   Acquire fence material
    
-   Construct the fence
    
    -   Mark fence line and posts
        
    -   Install posts
        
    -   Install fencing and posts
        
    -   Paint and stain fence
        

On each of the two tasks, you select Build fence as the Parent task. Then, these tasks are grouped together and child tasks are indented below the parent task, as shown below.

![Grouped\_childParent\_Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/Grouped_childParent_Tasks.png)

The parent task record shows data for all child records. You can't assign resources to parent tasks, they must be assigned to the child tasks.

Note:

When you create a parent task, it might first be saved as a milestone. When you add child tasks, it turns into a parent task. For more information, see [Milestones](#bridgehead_3739383427)

Another way to organize tasks is to show if they depend on other tasks. You do this by setting up predecessors.

### Predecessors {#procedure_N1194583}

Predecessor settings define the dependencies for a task. Dependencies are timing relationships among a group of tasks.

-   Finish-to-Start (FS) - Task starts when preceding task finishes. Start date is adjusted based on the preceding task's finish date.
    
-   Start-to-Start (SS) - Task starts after preceding task starts. Start date is adjusted based on the preceding task's start date.
    
-   Start-to-Finish (SF) - Task finishes after the preceding task starts. Start date is adjusted based on the preceding task's start date.
    
-   Finish-to-Finish (FF) - Task finishes after the preceding task finishes. Start date is adjusted based on the preceding task's finish date.
    

Commonly, a completed project plan is a group of milestones, work tasks, and parent tasks, each parent being one phase of the total plan. The Schedule subtab of the project shows an organized view of the complete plan, as shown below:

![ProjInitialTemplateSchedSubtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/ProjInitialTemplateSchedSubtab.png)

When entering predecessors, you can also add lag time between your tasks. Lag time is a delay between tasks that have a dependency. You can enter lag time to adjust your project schedule. To enter lag time, enter the number of days in the Lag Days field on the Predecessor subtab.

### Copying Tasks {#bridgehead_3898990487}

You can copy project tasks between projects and within projects. When copying a project task, you can choose to also copy the task assignments, budgets, and any child tasks. On the Schedule subtab of the project record, click Copy next to the project task you want to copy. For more information, see [Copying Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3897401475.html).

### Task Views {#procedure_N1194636}

You can choose from several ways to view a complete project in the View field. You can choose a Planning view, Tracking view or Variance view. For more information about these view options, read [Working with the Project Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html).

To view a list of projects tasks by assignee, go to Activities > Scheduling > Project Tasks. The Project Task list shows both tasks from the project and templates.

### Project Plans {#bridgehead_N1194659}

Creating, viewing, and organizing tasks for a project are all part of utilizing the project plan. For more information, see [Working with the Project Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html).

Project plan is a term to describe the means to schedule and manage project tasks. It organizes the tasks as parts of the project as a whole and defines how they should work together. You'll find the project plan on the Schedule subtab, where you can see the project's scope, progress, and cost.

### Task Baselines {#bridgehead_N1194685}

After you've entered all the necessary tasks, task durations, task dependencies, resource assignments, and cost estimates, take a baseline snapshot to compare intended activity to actual activity. Then, when you record the actual timing of tasks, actual resource time investment and actual costs, you can make a comparison.

### Resource Time Entry on Project Tasks {#bridgehead_N1194697}

The project record tracks the estimated time entered for each resource on a task. Then, when the resource enters time against the project, it tracks the actual hours worked.

The Time subtab on the task record displays the planned time entries.

### CRM Tasks {#bridgehead_N1194713}

Other task records you can choose to create are CRM task records. CRM tasks are "to do" activities that need to be completed. For example, a CRM task might be an upcoming meeting or phone call with a potential new client.

Like project tasks, each CRM task record tracks what needs to be done and who's responsible. Unlike project task records, CRM task records can be independent and don't need to be associated with a project.

Important:

To track information for projects, you should use project task records, not CRM task records. For more information, read:

-   [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html)
    
-   [Project Task Records](#bridgehead_N1192945)
    

### CRM Tasks and Project Management {#bridgehead_N1194777}

CRM tasks can be associated with a project, but they aren't considered part of the project's cost and time data unless you check the Include CRM Tasks in Project Totals box. CRM tasks associated with a project don't show up in the project schedule. For more information, read [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html).

### Viewing Project Tasks on Your Dashboard {#bridgehead_N1194797}

Add the Project Tasks portlet to your dashboard to see project tasks assigned to you or others. You can customize the portlet to display project tasks in a way that is meaningful to you. For example, customize the portlet to display a list of your project tasks filtered by project. Or, if you are a senior project manager, display a list of late tasks across all projects. This portlet is available only if you use the Project Management feature. From the portlet, you can quickly view or edit task details.

If you use the Inline Editing feature, you can update the status and priority of a project task in the portlet. Making changes in the portlet works the same as using Inline Editing in a list view. Since the portlet only shows a few fields, click Customize View or Edit View on a custom task view to reorder the fields and show the status and priority fields if needed.

Note:

The Priority field is not shown on the standard project task form. To display project task priorities as a column in the portlet, you must view a custom project task form in the portlet that includes the Priority field.

The portlet is available for full-access and Employee Center users who have View access to project tasks. If you want to view and update your CRM tasks or create new ones, add the Tasks portlet to your dashboard.

Use the portlet filter options to select which project tasks to show in the portlet. For more information, read [Tasks and Project Tasks Portlets on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509646.html).

### Related Topics

-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Project Task Attributes Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1195767.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Scheduling Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199494.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Importing Project Tasks from Microsoft Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200868.html)
-   [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
