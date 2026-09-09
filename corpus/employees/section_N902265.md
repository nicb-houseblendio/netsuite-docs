---
id: "section_N902265"
type: "section"
title: "Understanding Time Tracking"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Understanding Time Tracking"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html"
anchors: ["bridgehead_4508296478", "bridgehead_4351562768", "bridgehead_4647900551"]
sha256: "3d0a46239420f9784b4b1811d59ed494e26c67dce17a982bc1a8fcf9b9088dae"
---

Use time tracking to record the hours worked by employees.

You can record billable hours and invoice your customers for them. If you use Projects or Project Management, you can also record how many hours are spent on each project and use time reports to plan for future projects and hiring needs. For more information about Time Tracking and Projects, see [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html) , [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html), and [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html).

With the appropriate role access, you can track time for employee payroll items like hourly wages. Employees who have the Restrict Time and Expenses box checked and the Track Time permission enabled can enter time for themselves using their default roles without having to switch to the Employee Center role to track their time. For more information, see the topics under [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html).

Warning:

NetSuite CRM+ users can't record billable time, invoice customers for billable time, or record time for payroll items.

If your role has the Track Time permission, customer records include a Time Tracking subtab that shows associated time records and enables you to enter new ones. If you use Projects or Project Management, project records also include a Time Tracking subtab.

A user with the Enable Features permission must enable the Time Tracking feature at Setup > Company > Enable Features, on the Employees subtab.

To set preferences for tracking time, go to _Setup > Accounting > Preferences > Accounting Preferences_ and click the Time & Expenses subtab. For more information, see [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html).

Note:

If you use NetSuite OneWorld, the **Intercompany Time and Expense** feature and the related **Intercompany Time** accounting preference affect users' ability to enter time worked for customers or projects with subsidiaries other than their own. If the feature isn't enabled, or if the preference is set to **Disallow**, users can't enter intercompany time transactions. Instead, they can only select customers or projects with the same subsidiary to which they're assigned. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).

## Time Thresholds {#bridgehead_4508296478}

You can set time thresholds to limit how employees and vendors enter time. Time threshold preferences enable you to specify the minimum and maximum number of hours permitted per day and week. You can set one or all of these preferences to limit the number of hours permitted to be tracked on a weekly basis. You can opt to set the limits manually, or you can have the limits set automatically based on the work calendar. You can also choose to permit time transactions to be submitted outside the limits you set. You can choose whether to apply your time thresholds to vendor time.

Note:

Time thresholds aren't available when using SuiteScript, SuiteFlow, or custom approval routing.

Daily time threshold preferences account for holidays and non-working days based on the selected work calendar. NetSuite doesn't verify non-working days, holidays, or entries on a timesheet that haven't been filled yet.

For employees without a selected work calendar, time thresholds use the system default work calendar to determine holidays and non-working days. Zero time entries are considered filled entries and are verified according to set limits. Regardless of work calendars, employees can still track time on non-working days and holidays and time threshold limits are applied accordingly.

If you also use advanced approvals, you can choose to require time entries to be entered for each working day.

Important:

NetSuite validates set time thresholds within the browser. When an entry is made for the duration of a time transaction, NetSuite validates that the entry fits within the set limits. If an entry is left blank, NetSuite won't validate for that entry. This can create a situation where time transactions are saved that don't meet set threshold limits.

If you use Weekly Timesheets, thresholds are validated on both individual time entries and each timesheet. It's possible for a single time entry to satisfy a daily limit but not the weekly limit. In this situation the time entry would generate a warning because of the timesheet the entry is a part of. You can choose to allow time to be submitted after warnings are displayed.

Time thresholds are checked upon submission of the time entries. You can also choose to have the time entries validated again when they're approved.

To set time thresholds, go to _Setup > Accounting > Accounting Preferences_ and make selections for time thresholds at the bottom of the Time Tracking section.

For more information about time thresholds, see [Time & Expenses Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391368.html).

## Enabling Time Tracking for CRM {#bridgehead_4351562768}

With Time Tracking for CRM, users can track time on tasks, phone calls, events and cases. Tracking time on these activities can help you manage your company by being aware of how much time is spent on certain activities.

Important:

The Time Tracking feature and the associated permissions are required to use Time Tracking for CRM.

An administrator must enable the feature before users can track time.

#### To enable Time Tracking for CRM:

1.  Go to _Setup > Company > Enable Features_
    
2.  Click the **Employees** subtab, and check the **Time Tracking for CRM** box.
    
3.  Click **Save**.
    

Important:

If you also use the Projects feature and want to track time for customers, you must disable the **Show Projects Only for Time and Expense Entry** preference located on the Time & Expenses subtab at _Setup > Accounting > Accounting Preferences_. When this preference is enabled, time can only be tracked for CRM Tasks associated with a project record.

## Enabling Weekly Timesheets {#bridgehead_4647900551}

The Weekly Timesheets feature works in conjunction with the existing Time Tracking feature to offer a method of capturing time entries in a weekly format that can be further customized.

Important:

The Time Tracking feature and the associated permissions are required to use Weekly Timesheets.

An administrator must enable the feature before users can track time using the weekly timesheet.

#### To enable Weekly Timesheets:

1.  Go to _Setup > Company > Enable Features_
    
2.  Click the **Employees** subtab, and check the **Weekly Timesheets** box.
    
3.  Click **Save**.
    

Note:

Weekly Timesheets is an additional feature that offers a method for entering time on a weekly basis. The Time Tracking feature includes a Weekly Time Tracking page which can be used to track time on a weekly basis without any additional customizations. If enabled, Weekly Timesheets will take the place of the included Weekly Time Tracking.

For more information about using weekly timesheets, see [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html).

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html)
-   [Giving an Employee Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html)
-   [Restricting Employee Time Tracking Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html)
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
