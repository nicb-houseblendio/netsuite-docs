---
id: "section_N1199494"
type: "section"
title: "Scheduling Project Tasks"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Tasks > Scheduling Project Tasks"
parent: "section_N1192913"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199494.html"
anchors: ["bridgehead_N1199520", "bridgehead_N1199562", "bridgehead_N1199583", "bridgehead_N1199600", "procedure_N1199620", "bridgehead_N1199631", "bridgehead_N1200398", "procedure_N1200446"]
sha256: "7bc166573effef7f36f2ef1f31b6e545aff661fe85a2e48169ebc62449f98aad"
---

NetSuite creates a schedule for each project based on project start date or end date, task durations, predecessors, constraints, and resource work calendars. The schedule drives planning, billing, and management for the entire project.

For forward scheduling projects, the project Start Date sets the date from which the project schedule is calculated. For backward scheduling projects, the project End Date sets the date from which the project schedule is calculated.

To view the schedule for a project, go to Lists > Relationships > Projects and click View next to the project. On the project record, the Schedule subtab is the top subtab.

## Resource Assignment and Project Scheduling {#bridgehead_N1199520}

Project scheduling is also based on resource and work data entered on task records. The schedule is based on the duration of the tasks. Task duration is calculated as \[estimated work x units\] for all task resource rows and helps determine the start and end dates for each task.

For example, a task requires 16 hours of work. Two resources are assigned to the task, each set to work at 100% capacity and for 8 estimated hours. Each resource is assigned to the default work calendar of eight hours per day, Monday through Friday. The task is scheduled across two calendar days, so the project work schedule is 2 days in duration. The schedule also takes into account any time off requested by the assigned resources.

Note:

The task duration calculation is also affected by task relationships. See [Adaptive Scheduling](#bridgehead_N1199631) below.

Depending on the scheduling method, the start date or end date of a project task is calculated by assessing the number of hours assigned to each task resource. For each assignment, the resource's work calendar is used to add the specified number of hours to the start date-time or end date-time to arrive at the tasks dates. If the start date or end date of your project changes, NetSuite automatically updates the task dates based on the scheduled tasks. If time off is submitted after the schedule is created, you'll need to recalculate the project to adjust. For more information about scheduling methods, see [Project Scheduling Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182526.html#subsect_156296935424).

The total number of hours for the project task is calculated by summing the hours assigned to each resource.

## Work calendars {#bridgehead_N1199562}

Work calendars define the work capacity for resources. That capacity determines when tasks can be scheduled. For details, read [Project Resource Work Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189731.html).

## Creating Planned Time Entries {#bridgehead_N1199583}

When you create a project task, you enter the resource work capacity as percentage of available scheduling time in the Units column. NetSuite uses the work capacity and work calendars for resources assigned to project tasks to create the project schedule and generate planned time entries. If you create planned time entries for a project, NetSuite limits the number of time entries that can be created.

To prevent projects from having too many tasks and time entries, the following rules apply:

### Project tasks {#bridgehead_N1199600}

When assigning a resource to a project task, the resource capacity or units must be 5% or greater. The estimated work for the resource must be 2080 hours or less.

Planned time entries depend on the work calendar. For an eight hour workday, the minimum planned time entry is 24 minutes. The smallest planned time entry possible is 3 minutes (5% of 1 hour, which is the minimum allowed per day).

The maximum number of planned time entries per task for a resource is 260. This is the maximum number of work days a resource can be assigned to work on a task.

### Projects {#procedure_N1199620}

The total number of planned time entries for all project resources must be 5200 or less. The total amount of work days scheduled for a project can't exceed 20 person years of work.

## Adaptive Scheduling {#bridgehead_N1199631}

Project tasks are capable of adaptive scheduling. This means that when the current project schedule is viewed, the project schedule accurately reflects necessary changes to the project.

For example, when a project plan is initially created based on task dependencies and resource work calendars, the schedule represents an idealized estimate. This initial estimate doesn't reflect any actual project work if no actual time has been entered against the project from resources working on the project.

As work on the project begins, resources enter their time. After time is entered, some project task details may start to shift, such as:

-   project costs
    
-   start and end dates
    
-   work and actual work
    

For example, the work for TaskOneA is 40 hours: 8 hours per day, Monday through Friday. If a resource assigned to the task enters 4 hours for Monday, then the schedule automatically recalculates so that the project plan shows 4 hours of actual time worked on Monday, 8 hours of planned work scheduled Tuesday through Friday, and 4 hours of planned work scheduled the following Monday for a total of 40 hours.

Tasks with predecessor relationships are set to start based on the start and finish dates of other tasks. If the duration of one task changes, all tasks related to it may be recalculated to show an updated duration and new start and end dates. For more information, read [Predecessor-successor relationships](#procedure_N1200446) below.

The Time subtab on task records shows Planned Time and contributes to a real-time picture of project schedule.

-   If resources complete the project task early, it pulls in the projected end date of the project.
    
-   If resources cannot complete tasks as quickly as anticipated, the end date is pushed out accordingly.
    

## Task setup and scheduling {#bridgehead_N1200398}

The characteristics of a project task are largely derived from its relationship to other tasks in the project. Task relationships can be one of the following:

-   parent-child relationships
    
-   predecessor-successor relationships
    

Tasks for a project can be arranged in a hierarchy by assigning parent-child relationships. For example, you may create Task One. Then, you create tasks TaskOneA, TaskOneB, and TaskOneC, and assign Task One as the parent task for all three tasks. [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html) are tasks that have child tasks assigned to it.

The parent task, Task One, is also known as a summary task. The data values shown on a summary task are derived from its children. For example, a summary task's start date is the earliest start date of its child tasks, and its end date is the latest end date of its child tasks. Its work is the total of all its child tasks.

## Predecessor-successor relationships {#procedure_N1200446}

In addition to a hierarchical structure, project tasks relationships can also be defined in terms of dependency. For each task, you can define how that task relates to other project tasks based on when the task should start. Each task is a predecessor or a successor, even if the task runs concurrent to other tasks.

For example, the completion of TaskOneB requires components that are assembled during TaskOneA. Therefore, TaskOneA is a predecessor of TaskOneB. TaskOneB can't begin until TaskOneA is completed.

Dependency types that can be assigned on tasks are

-   Finish-to-Start (FS) - Task starts when preceding task finishes. Start date is adjusted based on the preceding task's finish date.
    
-   Start-to-Start (SS) - Task starts after preceding task starts. Start date is adjusted based on the preceding task's start date.
    
-   Start-to-Finish (SF) - Task finishes after the preceding task starts. Start date is adjusted based on the preceding task's start date.
    
-   Finish-to-Finish (FF) - Task finishes after the preceding task finishes. Start date is adjusted based on the preceding task's finish date.
    

Some data on a project task are calculated using input from its dependency relationships. For example, in a start-to-finish dependency, the task's start date is the latest end date of all its predecessors. In a start-to-start case, it's the last start date of all its predecessors.

Project tasks that have no predecessors start on the start date of the project.

### Related Topics

-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
-   [Project Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1192945)
-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Project Task Attributes Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1195767.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Importing Project Tasks from Microsoft Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200868.html)
-   [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
