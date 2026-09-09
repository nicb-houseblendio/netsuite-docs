---
id: "section_N1191698"
type: "section"
title: "Entering Time Against Projects"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Managing Time and Expenses for Project Resources > Entering Time Against Projects"
parent: "section_N1190979"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1191698.html"
anchors: ["bridgehead_N1191790", "bridgehead_N1191991", "bridgehead_N1192065"]
sha256: "81d63f22d6cb96bfae7211d4841fc48936cdf76aa0ff8bc5745e128ef371e1af"
---

After you create a project record, you can enter time against the project directly from the project record. You can estimate time budgeted for a task and then track progress being made on the project and the percentage of completion as time is entered.

Entering time against a project also lets you calculate resource productivity and utilization. For more information, read [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html).

Recording project time affects:

-   **Scheduling:** When you enter time for yourself or your employees, NetSuite compares the estimated time to complete each task with the actual time recorded in Time Tracking. It modifies the project schedule as needed based on the task constraint and predecessor attributes.
    
    For example, the estimated time to complete Task A is 4 days. Task A must be finished before Task B can begin. It takes you five days to complete Task A. When you record five days of work against Task A in Time Tracking, NetSuite advances the start and end dates of Task B, and all tasks that depend on Task B, by one day.
    
    The Gantt chart updates to show the actual time worked and the new task start and end dates.
    
-   **Billing:** For Time and Materials projects, time must be entered, marked billable, and approved to be billed. Recording time worked on a project affects the amount billed because invoices reflect only billable time performed. Time entry doesn't affect the timing of billing because invoices are generated at specified intervals. Changes in the amount of time it takes to complete tasks may affect the number of invoices that get generated for a project. For example, tasks that take longer than planned to complete may extend into an additional billing period and trigger an additional project billing cycle for the project.
    
    For Fixed Bid, Interval projects, recording time worked on a project doesn't affect the timing of billing but does affect the amount billed. Bills are generated at specified intervals based on the expected percentage of work completed for each interval. Resources must account for all planned time in each billing interval to ensure that invoices are generated for worked performed rather than for work planned. As with time and materials projects, the number of billing cycles may also increase or decrease based on project progress.
    
    For Fixed Bid, Milestone projects, billing depends on completing a set of tasks. If the task completion dates change, then the time when invoices can be created and sent to customers also changes.
    
-   **Reporting:** Project time and utilization report information is based on the time classification attributes selected on the Info subtab for the project. For more information about productivity and utilization, see Project Resource Time and Expense Management and Project Management Reports.
    
    Planned time entries are available in both search and reporting and you can use them to report on expected future work.
    
-   **Project Management:** Each project task record displays the estimated, actual, and remaining work needed to complete the task. This enables you to manage the project from within the project record. You can access Time Tracking directly from each task to record project hours.
    

## Entering Time for a Project {#bridgehead_N1191790}

Time can be tracked against a project directly from the project record or by selecting the project in the Customer:Project field on time transactions. Time should be tracked primarily from the Employee Center role or a role with similar time restricted permissions. Implementing this best practice maintains approval and status preferences. CRM tasks associated with a project are also available for time entry. Select a CRM task from the Case/Task/Event dropdown list.

Important:

If you selected Approve Automatically on the project's preferences subtab, time should only be entered through the Employee Center role. When using any role with additional time tracking permissions, you must manually set the Approval Status field on individual time transactions or submit a weekly timesheet for time to be approved. For more information, see [Setting Up Project Record Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4585905289.html) and [Approving Time and Expenses for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192683.html).

#### To enter time against a project from the project record:

1.  Go to Lists > Relationships > Projects.
    
2.  Click **Edit** next to a project in the list to open the record.
    
3.  Click the **Resources** subtab.
    
4.  Click the **Time Tracking** subtab.
    
5.  On the **Time Tracking** subtab, you can choose to enter time against the project in one of two formats:
    
    -   Single Entry Format - Enter a single instance of time a resource worked on a project.
        
        Click **New Time** to open a single entry format time entry form.
        
    -   Weekly Entry Format - Enter the time resources worked on projects a week at a time.
        
        Click **New Weekly Time** to open a weekly format time entry form.
        
6.  A window opens with the time entry form. The **Project** field is autofilled with the project name. In the **Case/Task/Event** field, select a project task.
    
    For more information about completing time entry forms, click one of the links below:
    
    -   For details on the New Time form, read [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html).
        
    -   For details on the New Weekly Time form, read [Weekly Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904728.html).
        
    -   For details on the Timesheets form, read [Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3891941390.html).
        
7.  When you have completed the form, click **Save**. The time data is updated on the project record.
    

You can also choose to enter time for a project by going to _Transactions > Employees > Track Time_ or to _Transactions > Employees > Weekly Time Sheet_ and selecting a project in the Customer:Project field.

## Entering Project Time Against a Case, Task, or Event {#bridgehead_N1191991}

If you track time in NetSuite, employees and other project resources can enter time against a project task, case, CRM task, or other activity by selecting an item in the Case/Task/Event field when entering time. This field is available only if you use Project Management. The items that appear in the dropdown list for this field vary depending on the features that you enable for your organization.

-   If you enable both Project Management and Time Tracking for CRM, then the Case/Task/Event field shows only the uncompleted project tasks assigned to the employee or resource. The dropdown list also shows all activities and cases associated with the customer and project selected in the Customer:Project field, regardless of who the activities and cases are assigned to. In this configuration, a resource can enter time for their own project tasks, but can also enter time against all CRM tasks associated with the customer and project.
    
    The Time Tracking subtab appears on case, task, and event records.
    
    Note:
    
    If a case, task, or event has more than 9500 time entries, then the Time Tracking subtab shows a static list of time entries. You can't edit entries directly from the list.
    
-   If you enable Project Management but not Time Tracking for CRM, then the Time Tracking subtab isn't available on activity or case records. Resources can still enter time against activities and cases. The Case/Task/Event field shows up in time transactions and lists uncompleted project tasks for the resource, plus all events, calls, and cases for the customer and project.
    
-   If you don't enable Project Management, then the Case/Task/Event field won't appear.
    

The Case/Task/Event dropdown identifies the type of item in parentheses () after the item name. Items in the dropdown list are sorted by type and then name.

Project task - (Project Task)

CRM task - (Task)

Other activities - (Phone call) (Event)

Note:

Cases only show the case number, not the case name (for example, Case #125).

Note:

If you plan to enter a memo for the time transaction, always select an activity in the Case/Task/Event field before you enter the memo.

## Deleting Project Time {#bridgehead_N1192065}

You can delete time entered against a project if the time hasn't been approved by the project manager or resource supervisor yet.

#### To delete time entered for a task:

1.  On the **Schedule** subtab for a project, click a task name.
    
2.  On the **Time Tracking** subtab, click **Edit** next to the item you want to delete.
    
    You can only edit unapproved time.
    
    Note:
    
    If a case, task, or event has more than 9500 time entries, then the Time Tracking subtab shows a static list of time entries. You can't edit entries directly from the list.
    
3.  If you use Time Tracking, the time entry record opens. In the More Actions menu, click **Delete**.
    
    Close the window to return to the **Schedule** subtab.
    
    Note: NetSuite deletes only the selected time transaction if there are multiple time entries in the time record.
    
4.  If you use Timesheets, the timesheet record opens. Find the entry you want to delete and remove it. Click **Done** to save the line. When you're finished, click **Submit** to submit the timesheet for approval or **Save for Later** to save the timesheet without submitting.
    

### Related Topics:

-   [Restricting Time Entry on Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192197.html)
-   [Approving Time and Expenses for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192683.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)
-   [Working with Projects in Multiple Time Zones](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201840.html#bridgehead_N1201894)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
