---
id: "section_N904728"
type: "section"
title: "Weekly Time Tracking"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Weekly Time Tracking"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904728.html"
anchors: ["subsect_161131803985", "bridgehead_4507355876"]
sha256: "40833bec7db88c02acb0499c46e8a9c7196f12e9c46292a94f6f31d355ac8c7b"
---

With weekly time tracking, you can track the hours you and other employees work for a week at a time.

To track time, an administrator should go to Setup > Enable Features > Employees, check the Time Tracking box, and click Save.

Note:

If your company uses weekly timesheets, see [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html).

#### To use weekly time tracking:

1.  Go to _Transactions > Employees > Weekly Time Tracking_.
    
2.  Select the employee whose time you are recording.
    
3.  In the **Date** field, enter the first day of the week you want to track time for, or click the **Pick** link to choose a date.
    
    NetSuite inserts the date that the current week begins as the posting date of this week's time.
    
    You can set the day your company's business week starts by going to _Setup > Accounting > Preferences > Accounting Preferences_. Click the **General** subtab.
    
4.  If you use Project Management, you can import any planned time entries for the selected employee and week. Click **Import Planned Time** to automatically import the project time entries for the current week.
    
5.  If you don't use the Advanced Approvals preference, check the **Supervisor Approval** box if you are a supervisor entering time for an employee.
    
6.  On the **Enter Time** subtab, in the **Customer** column, select a customer or project if the time worked is for a customer or project.
    
    If you use NetSuite OneWorld, the **Intercompany Time and Expense** feature and the related **Intercompany Time** accounting preference determine whether you can select a customer or project with a subsidiary different from yours. If the feature is not enabled, or if the preference is set to **Disallow**, you can't enter intercompany time transactions. Instead, you can select only those customers or projects with the same subsidiary to which you are assigned. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
    
7.  If you use the **Project Management** feature and selected a project in the **Customer** field, use the **Case/Task/Event** column to select an activity associated with the project and time.
    
8.  If your company uses multi-state calculations for payroll, select a **Payroll Item Workplace**.
    
9.  Ensure that the **Billable** box is checked if the time is billable to a customer or project. If this time is billable, you must select a customer or project.
    
    Warning:
    
    In NetSuite CRM+, the **Billable** box is not available. NetSuite CRM+ users can't record billable time, invoice customers for billable time, or record time for payroll items.
    
10.  Select a payroll item if you are tracking time for payroll.
     
11.  Select the service that was provided if you track time spent on services.
     
     If the **Billable** box is enabled, you must select a service item.
     
     If you use NetSuite OneWorld, you should set up service items that are available to all subsidiaries to use in intercompany time transactions. In these transactions, users can't save lines unless they contain service items available to both the employee subsidiary and customer subsidiary. See [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
     
12.  Select a department, class, or location if you track this information.
     
     Important:
     
     If you use NetSuite OneWorld and you are entering intercompany time transactions, you must determine a strategy for using classifications on these transactions. Best practice is to omit them. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
     
13.  If the **Override Rates on Time Records** preference has been enabled on the **Time & Expenses** subtab at Setup > Accounting > Accounting Preferences, the following fields display:
     
     -   **Price Level** - Select a price level. You can use different price levels by going to Setup > Enable Features > Customers/Sales, and checking the **Use Multiple Prices** box.
         
     -   **Rate** - If you selected a price in the **Price Level** field, it automatically appears here. If you don't use multiple prices or if you selected **Custom** in the **Price Level** field, enter a rate for this time transaction. If you are entering time for a payroll item like vacation time, leave this field blank.
         
     -   **Lock this Rate** - If you are billing this time back to a customer, check this box to lock the rate you enter so it's not affected by rate changes that happen before the customer is billed. If you are entering time for a payroll item like vacation time, leave this field blank.
         
14.  Enter a memo.
     
     If you are billing this time back to a customer or project, this memo appears as a description for this line item on the customer invoice.
     
     Note:
     
     Always select an activity in the **Case/Task/Event** or **Service Item** fields before entering a memo. When you select a case, task, event, or service item, the memo field is automatically populated with information from these records. Anything you entered in the memo field prior to selecting one of these records will be deleted. Changing your selection in either of these fields will update the memo field with any information from the newly selected record.
     
15.  Enter the hours for each day in this week.
     
16.  Click **Add**.
     
17.  Repeat steps above for each customer or project you need to enter time against.
     
18.  Click **Save** to save the entries. If you use Advanced Approvals, you can also click **Submit** to save and submit the entries
     

When time is saved, the time then appears on the Time Details subtab of the time tracking for that week.

If you billed time back to a customer or project, it appears when you click Billable Time on the corresponding invoice page.

If you tracked time for hourly wage payroll items, it appears in the Hours column for this employee on the Payroll Run page.

## Copying a Previous Week for a Weekly Timesheet {#subsect_161131803985}

In addition to entering new time each week, you can also copy the time entries from a previous week on to the current week.

#### To copy a previous week for weekly time tracking:

1.  Go to _Transactions > Employees > Weekly Time Tracking_.
    
2.  Click **Copy from Week**. A window opens with the start date of the previous week's time automatically populated.
    
3.  In the **Date** field, you can accept the date automatically entered or use the date selector to select a different date.
    
4.  If your company enables employees to choose to copy hours and memos, clear the **Copy Hours and Memos** box if you don't want hours and memos from the selected week to be copied to the current week.
    
5.  Click **Copy**. Time entries within the selected week are copied to the weekly time tracking page currently being edited. Depending on your company's preferences, copied time entries may include hours and memos.
    
6.  Continue to fill in required information for this time. When you're done, click **Save**.
    

To view a list of all weekly time tracking entries you have permission to view, go to Transactions > Employees > Weekly Time Tracking > List. This list displays the employee, date, hours, and approval status of each week.

## Advanced Approvals {#bridgehead_4507355876}

If your company uses the Advanced Approvals on Time preference, after time is saved on your Weekly Time Tracking page, the background of each entry reflects that entry's approval status.

-   Open - white
    
-   Approved - green
    
-   Rejected - red
    
-   Pending - blue
    

Advanced approvals enables your employees to know the status of their time entries within a single week by looking at the Weekly Time Tracking page. When rejecting transactions, advanced approvals enables you to add a rejection note. For more information about Advanced Approvals, see [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html).

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html)
-   [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html)
-   [Giving an Employee Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html)
-   [Restricting Employee Time Tracking Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html)
-   [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html)
-   [Deleting or Editing Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4502096285.html)
-   [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html)
-   [Using the Timer to Track Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905386.html)
-   [Calculating Total Time Worked](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905783.html)
-   [Entering Time for a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906077.html)
-   [Custom Fields in Time Tracking Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906942.html)
-   [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html)
-   [Custom Workflow-based Approvals for Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554190531.html)
-   [Updating Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156408321759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
