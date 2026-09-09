---
id: "section_N1194983"
type: "section"
title: "Creating a Project Task Record"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Tasks > Creating a Project Task Record"
parent: "section_N1192913"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html"
anchors: ["bridgehead_3740052480"]
sha256: "2d99abc860cc5ee7797148d10ce038371ae859f214a5cb2600bbab797a4d8c16"
---

Create a project task record for every step you need to finish a project. Project tasks are always linked to projects and can only be created on the project record. For information about project tasks, see [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html).

Note:

For details about creating CRM tasks, read [Creating CRM Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N508608.html).

#### To create a new project task:

1.  Go to Lists > Relationships > Projects and click **View** next to the project you want to create a project task for.
    
2.  On the project record, click **New Project Task** on the **Schedule** subtab.
    
    A new project task window opens.
    
3.  Under Primary Information:
    
    1.  In the **Custom Form** field, select the form you want to use to enter this record. This field only appears when you have at least one custom form. You can customize this form by clicking Customize Form at the top of the page.
        
    2.  Enter a name for this task.
        
    3.  Select a parent task if the new task is part of a group of tasks. The parent task summarizes data for all of its subordinate tasks.
        
        You cannot assign resources to a parent task.
        
    4.  In the **Insert Before** field, place the new task in the proper order in the schedule, by selecting the task that follows it.
        
    5.  Select a status for this project task.
        
    6.  Check the **Non-billable** box to designate this task as non-billable.
        
        When time is entered against this task, it's automatically marked as non-billable and can't be changed to billable.
        
4.  Under Project Task Overview, in the **Estimated Work** field, enter the estimated time needed to finish this task.
    
    The remaining fields are populated after the task record is saved and work has started.
    
    Note:
    
    The Estimated Work field updates automatically when resources are assigned or allocated to the project task. If you add multiple resources, the field displays the sum of all estimated work. If this is a parent task, the field automatically updates to include the sum of estimated work for all child project tasks.
    
    If you also use Resource Allocations, when the Allow Allocated Resources to Enter Time to All Tasks project preference is enabled, estimated work includes the total of all planned time from assigned resources and any tracked time from resources not assigned to this specific task.
    
    Important:
    
    Saving a project task with no estimated work, assigned resources, and Finish No Later Than date creates a project milestone. You can turn milestones into project tasks by adding estimated work or resources. For more information, see [Creating Milestone Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740066806.html).
    
5.  Under Project Task Dates:
    
    1.  In the **Constraint Type** field, specify how to determine the start and end dates for the task.
        
        -   **As Soon As Possible** - For forward scheduled projects, NetSuite calculates the earliest possible start date for a task based on its predecessors and sets the end date based on the assigned resource's available work time.
            
        -   **As Late As Possible** - For backward scheduled projects, NetSuite calculates the latest possible end date for a task based on its predecessors and sets the start date based on the assigned resource's available work time.
            
        -   **Fixed Start** - The task starts on the date you specify. Predecessor relationships are ignored. The task end date is based on the estimated work for the task and the assigned resource's available work time.
            
    2.  The **Start Date** field indicates the estimated date to start the task.
        
        -   If the task constraint is Fixed Start, enter the date to begin work on the task.
            
        -   If the constraint is As Soon As Possible or As Late As Possible, NetSuite determines the Start Date based on the schedule.
            
    3.  If the task constraint type is Fixed Start, you can optionally enter the time to begin work on the task in the **Start Time** field. If you leave it blank, the start time is 12:00 am. You can't enter a start time if the task constraint type is As Soon As Possible.
        
        For information about project tasks in multiple time zones, see [Working with Projects in Multiple Time Zones](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201840.html#bridgehead_N1201894).
        
    4.  In the **Finish No Later Than** field, you can select the date this task must be finished by.
        
        Note:
        
        This constraint takes precedence over task relationships and start dates are adjusted to match the fixed end date of a task with a Finish No Later Than constraint.
        
6.  Under **Notes**, you can enter additional information for this task in the Notes filed.
    
7.  Under **Assignees** you can add resources to this project task. For more information, see [Assigning Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html).
    
    If you use Resource Allocations, you can choose to allocate resources to the project and then assign tasks using the steps below. You can also allocate resources directly to tasks to eliminate the need to assign tasks. For more information, see [Assigning Resources with Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html#bridgehead_4362895283).
    
8.  On the **Predecessors** subtab, set dependency types for the task:
    
    1.  Select an existing project task in the **Task** field.
        
    2.  Select a dependency type for the existing task as it relates to the current task.
        
        -   **Finish-to-Start (FS)** - Task starts when preceding task finishes. Start date is adjusted based on the preceding task's finish date.
            
        -   **Start-to-Start (SS)** - Task starts after preceding task starts. Start date is adjusted based on the preceding task's start date.
            
        -   **Start-to-Finish (SF)** - Task finishes after the preceding task starts. Start date is adjusted based on the preceding task's start date.
            
        -   **Finish-to-Finish (FF)** - Task finishes after the preceding task finishes. Start date is adjusted based on the preceding task's finish date.
            
    3.  If you want to add lag time to your tasks, enter the number of days in the **Lag Days** field.
        
    4.  Click **Add**.
        
    5.  Repeat these steps for each task dependency you need to set up.
        
9.  If you use Project Budgeting, enter cost and billing budgets for this task on the **Budget** subtab.
    
    For more information, see [Creating Project Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751156905.html).
    
10.  On the **Communication** subtab, you can enter notes about this task and attach files from the File Cabinet or upload new files associated with this project.
     
11.  On the **Time** subtab, you can choose to enter time against the project. For details on time tracking features, read [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html), [Weekly Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904728.html), or [Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3891941390.html).
     
12.  When you're done, click **Save**.
     

Important:

When you edit project tasks, refresh your view of the project record to see updated data on the **Financial** subtab.

Tip:

For best performance, keep most projects shorter than one year and with fewer than 1,000 tasks. Use sub-projects when you can.

## Working with Task Records {#bridgehead_3740052480}

After you've saved a task record and started work on your project, NetSuite updates fields on the project task record to reflect changes in your task details.

To view a project task record, go to Lists > Relationships > Projects. Click View next to the Project your task belongs to. On the Schedule subtab, click the name of the task you want to view. The project task record opens.

When you view the project task record, following fields update as your project progresses:

-   The Actual Work field shows the amount of time entered against this project task. This total includes approved and unapproved time.
    
-   The Remaining Work field shows the time for work yet to be done on this project task. It's calculated as:
    
    \[Estimated Work - Actual Work\]
    
    Before work starts on a task, Remaining Work is the same as Estimated Work. When a task is marked Completed, this number is 0.
    
-   Percent Complete is calculated as:
    
    \[Actual Work time divided by Estimated Work time\]
    
    The percentage is 100% when the task status is Completed.
    
-   Depending on the project scheduling method, the Start Date or End Date field shows the estimated date when the task will start or finish, based on the estimated work and other dependencies. These dates can change during project if the amount of work, resources assigned, or task dependencies change. For more information, see [Project Scheduling Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182526.html#subsect_156296935424).
    
-   If you use Resource Allocations, the Allocated Work field displays the number of hours allocated to this task. The Percent Complete by Allocated Work field displays the progress of the project based on the allocated resources. This can help you spot when a project needs more effort than planned.
    

### Related Topics

-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
-   [Project Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1192945)
-   [Project Task Attributes Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1195767.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Scheduling Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199494.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Importing Project Tasks from Microsoft Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200868.html)
-   [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
