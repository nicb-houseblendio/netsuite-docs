---
id: "section_N898879"
type: "section"
title: "Restricting Employee Time Tracking Entries"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Restricting Employee Time Tracking Entries"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html"
anchors: ["subsect_156269527419", "subsect_157304824449"]
sha256: "d0b7523341b6a532161f3855b50b45954b9d77df6e23153a1e9a813f7fcfcb83"
---

Account administrators can control which names display for certain roles in the time entry list by editing user roles. Limits on this list restrict the ability of employees to enter time for other employees.

#### To restrict employees to enter time for only themselves or their subordinates :

1.  Go to _Setup > Users/Roles > User Management > Manage Roles_.
    
2.  Click the **Customize** link next to the role you want to restrict.
    
3.  Enter a new name for the restricted role.
    
4.  On the Role page, in the **Employee Restrictions** field, select **self and subordinates only**.
    
5.  Click **Save**.
    
6.  Repeat steps 2 through 5 for each role you want to restrict from being able to enter time for every employee.
    

You must update your employee records to assign the restricted roles. For more information, see [Assigning Roles to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N897798.html).

For the roles that you customize, additional areas of NetSuite are restricted based on the selection you've made. For more information, see [Setting Employee Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637690919.html).

Period locking is controlled exclusively by the time zone of the subsidiary to which the logged-in user belongs. It can result in up to 26 hours difference in the locking time if logged-in users are out of the subsidiary. If this default behavior causes problems, set the subsidiary time zone to the time zone where the employees usually work. Or adjust the Grace Period so that all employees have enough time to enter their timesheets.

## Locking Timesheet Periods {#subsect_156269527419}

Account administrators can disable the ability for employees to submit, edit, or add a time entry within a specific time period. You can choose to lock timesheets by closed fiscal periods, weekly, or monthly.

Note:

The Weekly Timesheets feature is required to enable locking timesheet periods. For more information, see [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html).

#### To set up a timesheet lock:

1.  Go to _Setup > Accounting > Accounting Preferences_. Click Time & Expenses.
    
2.  Under Time Tracking, in the **Lock Timesheet Period** field, select the time period after which you want time entries to be locked.
    
    -   None - time entries are always allowed.
        
    -   Closed Fiscal Period - time entries are no longer allowed after the accounting period is closed.
        
    -   Weekly - time entries are no longer allowed after the current week has past.
        
    -   Monthly - time entries are no longer allowed after the current month has past.
        
3.  If you select Weekly or Monthly, in the **Grace Period** field, enter the number of days time entries will remain open after the selected period. The grace period depends on which day your timesheets begin. For example, if you choose to close timesheets every week and you enter two in the Grace Period field, if your timesheets begin on Monday, they are locked on Wednesday each week.
    
4.  When you're done, click **Save**.
    

A single timesheet can contain both locked and unlocked time entries if the timesheet spans a locked and unlocked period. Administrators can unlock previously locked timesheets for a specific employee. Administrators can also edit or create time entries for a locked timesheet.

## Unlocking Timesheet Periods {#subsect_157304824449}

You may find it necessary to unlock a time period after it's been locked for employees to update or enter time that may have been forgotten. Administrators can unlock previously locked time periods for individual employees.

#### To unlock a time period:

1.  Go to Transactions > Employees > Unlock Time Period. You can also click **Unlock** on the specific timesheet you want to unlock. To view a specific timesheet, go to Transactions > Employees > Weekly Timesheets.> List. Click **View** next to the timesheet you want to unlock.
    
2.  On the Unlock Time Period page, in the **Employee** field, select the employee you want to unlock the time period for. If you have clicked **Unlock** directly from the timesheet, the employee field is populated with the employee's name.
    
3.  In the **Valid Until** field, select the date you want the lock to be reinstated.
    
4.  In the **Start Date** field, select the start date for the period you want unlocked. If you clicked Unlock on a timesheet, the start date for that timesheet is automatically populated in this field.
    
5.  In the **End Date** field, select the end date for the time period you are unlocking. For example, if you want to unlock a two week period of timesheets, select a date that is two weeks after the selected start date.
    
6.  When you're done, click **Save**.
    

Unlocking timesheet periods is only available for administrators and permission for unlocking timesheet periods is not available for custom roles.

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html)
-   [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html)
-   [Giving an Employee Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html)
-   [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html)
-   [Deleting or Editing Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4502096285.html)
-   [Weekly Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904728.html)
-   [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html)
-   [Using the Timer to Track Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905386.html)
-   [Calculating Total Time Worked](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905783.html)
-   [Entering Time for a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906077.html)
-   [Custom Fields in Time Tracking Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906942.html)
-   [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html)
-   [Custom Workflow-based Approvals for Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554190531.html)
-   [Updating Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156408321759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
