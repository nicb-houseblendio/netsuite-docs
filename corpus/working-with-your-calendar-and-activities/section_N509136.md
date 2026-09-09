---
id: "section_N509136"
type: "section"
title: "Tracking Time on CRM Tasks"
branch: "working-with-your-calendar-and-activities"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Your Calendar and Activities > Working with CRM Tasks > Tracking Time on CRM Tasks"
parent: "section_N506499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509136.html"
anchors: ["procedure_N509190"]
sha256: "6d97997bbeff09ab90e8addb3d4bf4a41607bf670c7b93469d64799ea88a770b"
---

You can enter time transactions to track the amount of time spent on each task. To track time on tasks an administrator must enable the Time Tracking for CRM feature. See [Enabling Time Tracking for CRM](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html#bridgehead_4351562768).

With Time Tracking for CRM, you can track time on tasks, phone calls, events, and cases. Tracking time on these activities helps you manage your company by making you aware of how much time is spent on different activities.

#### To track time on CRM tasks: {#procedure_N509190}

1.  Click **Edit** next to an existing task record on the Tasks list at Activities > Scheduling > Tasks. For more information, see [Creating CRM Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N508608.html).
    
2.  Click the **Time Tracking** subtab on the task record.
    
    Note:
    
    If any case, task, or event record has more than 9500 time entries on the Time Tracking subtab, all CRM tasks display a static list of time entries. You can't edit entries directly from the list.
    
    Note:
    
    If you use the Project Management feature, you can include CRM tasks in project totals. Note, however, that you must use project task records to track tasks associated with specific projects.
    
    The fields below display on the **Time Tracking** subtab only when you use the Project Management feature.
    
    ![Time Tracking subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/Calendars_Tasks_TimeTracking.png)
    -   **Initial Time Budget** - Enter your first estimate of the time needed for this task. Later you can update your estimate in the **Current Time Budget** field. Keeping your initial time estimate in this field lets you compare it to your current estimate. If you entered a time estimate on a project task template, that amount shows in this field.
        
    -   **Current Time Budget** - If your estimate of the time changes from your original estimate, enter the new estimate in this field.
        
    -   **Actual Time** - This field shows the total amount of time entered against this task.
        
    -   **Time Remaining** - This field shows the estimated remaining amount of time for this task. Time remaining is calculated as (Initial Time Budget - Actual Time).
        
        If you've entered a **Current Time Budget** amount to update your initial time budget, then the time remaining for the task is calculated as (Current Time Budget - Actual Time).
        
    -   **Percent Time Complete** - This field shows the calculated total of work that has been completed to date in percent format. The percent complete is calculated as (Actual Time \* 100%) / Initial Time Budget.
        
        If you've entered a **Current Time Budget** amount, then the percent complete is calculated as follows (Actual Time \* 100%) / Current Time Budget.
        
    -   **Percent Complete** - Enter an estimate of how much of the total amount of work for this task is already completed. For example, if half the work is done, enter **50%**. The percentage you enter in this field overrides the system calculation in the **Percent Time Complete** field and is used for task calculations.
        
3.  Your name appears in the **Employee** field. Depending on your role access, you can select another employee if you're entering time for someone else.
    
    Note:
    
    For private tasks, only employees assigned to the task can track time against the task.
    
4.  Enter information for this time transaction.
    
    For more information about entering time for Time Tracking, see [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html).
    
    For more information about entering time for Timesheets, see [Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3891941390.html).
    
5.  Repeat this process to track time for more customers or employees for this task.
    
6.  Click **Save**.
    

For instructions on limiting employees' ability to enter time records, see [Restricting Employee Time Tracking Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html) . Employees can also use the Employee Center to track their time. For more information, see [Giving an Employee Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html).

You can view employee time on the Reports page under the Time & Billables heading.

### Additional Information

-   [Entering Time Against Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1191698.html)
-   [Setting Up Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182249.html)
-   [Personal Preferences for Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N482375.html)

### Related Topics

-   [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html)
-   [Creating CRM Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N508608.html)
-   [Tasks and Project Tasks Portlets on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509646.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
