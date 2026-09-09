---
id: "section_N904108"
type: "section"
title: "Entering a Time Transaction"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Entering a Time Transaction"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html"
anchors: ["subsect_9020627593", "subsect_9020627594", "subsect_9020627595"]
sha256: "b935c8e97f76c0b2ddd1286db2fd04e26286d898b954be781c23fbfa32122c01"
---

Enter time transactions to track the hours you and other employees work.

#### To enter a time transaction:

1.  Go to _Transactions > Employees > Track Time_.
    
    The preferred time tracking form configured for your account opens.
    
2.  Complete the fields in the **Primary Information** section. For guidance on filling them, refer to the [Primary Information Section Standard Fields](#subsect_9020627594).
    
3.  Complete the fields in the **Classification** section. For guidance on filling them, refer to the [Classification Section Standard Fields](#subsect_9020627595).
    
4.  Click **Save**.
    
    At the bottom of the page, the saved information appears on the **Time Details** section.
    

If your company uses Approval Routing or Advanced Approvals for Time, the employee's supervisor or time approver receives an email notification when time is entered or edited.

The employee receives an email notification when the status on the Time record changes. The subject of this email says either that the time was approved or that the time was rejected.

You can also enter a time transaction on a customer or project record. To do so, go to _Transactions > Employees > Track Time_. Click **Edit** next to the customer.

## Time Tracking Form Fields {#subsect_9020627593}

Refer to the following tables for guidance on how to fill time tracking form fields.

For more information about customizing fields in forms, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).

### Primary Information Section Standard Fields {#subsect_9020627594}

| Field | Description | Field Availability |
| --- | --- | --- |
| Custom Form | Lists the forms that you can use to enter time. Select a form for this transaction. | May be shown or hidden |
| Employee | Shows the employee list. Select the employee whose time you are recording. | Always shown |
| Date | Automatically populates the current date as the posting date of the time entry. If needed, type or pick another date. | Always shown |
| Start Time | Enter the time when work started, in hours and minutes, in the format h:mm, followed by am or pm. This field is available only to implementations using the Time Tracking, New Weekly Timesheets, or Enhanced Timesheets with Workforce Management (WFM) Wage Rules feature. | May be shown or hidden |
| End Time | Enter the time when work ended, in hours and minutes, in the format h:mm, followed by am or pm. This field is available only to implementations using the Time Tracking, New Weekly Timesheets, or Enhanced Timesheets with Workforce Management (WFM) Wage Rules feature. | May be shown or hidden |
| Duration | Enter the duration using one of the following ways:
-   **Direct Entry** - In the **Duration** field, enter the amount of time worked for the day.
-   **Timer** - If you want to time yourself as you work or time the length of your break, click the Timer icon next to the **Duration** field. The elapsed time in the timer fills in the **Duration** field when you click **Submit**
-   **Calculate Time** - Click the Calculator icon. In the Calculate Time popup window, enter the start time and end time. Optionally, you can enter your break duration. The duration appears on the Total field. When you click **Save**, the total work hours appear in the Duration field.

**Guidelines When Entering the Duration**

-   When you enter time, minutes that total more than 59 are automatically converted to hours to be added to the total time. Time entries can have minutes entered and saved in a range of 0 to 59. For example, if you enter **:125**, it's interpreted as 125 minutes and is converted to display as 2:05. Likewise, these time entries are converted as follows:
    -   **0:125** is converted to 2:05 (2 hours and 5 minutes)
    -   **1:80** is converted to 2:20 (2 hours and 20 minutes)
    -   **1:120** is converted to 3:00 (3 hours and zero minutes)
-   If your form has been configured to display the **Start Time** and **End Time** fields and you entered values in them, the **Duration** field doesn't automatically calculate the total work hours. You must enter the duration.

 | Always shown |
| Customer | Select a customer or project if the time worked is for a customer or project. If you use NetSuite OneWorld, the **Intercompany Time and Expense** feature and the related **Intercompany Time** accounting preference determine whether you can select a customer or project with a subsidiary different from yours. If the feature is not enabled, or if the preference is set to **Disallow**, you can't enter intercompany time transactions. Instead, you can only select customers or projects with the same subsidiary to which you are assigned. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html). If you billed time back to a customer or project, it appears when you click **Billable Time** on the corresponding invoice page. | May be shown or hidden |
| Case/Task/Event | If you use the **Project Management** feature and selected a project in the **Customer** field with which this time is associated, you can select a related case, event, or task for the project. | May be shown or hidden |
| Item or Service Item | Select the service that was provided if you track time spent on services. If you selected a customer or project, you must select a service item. Note: The service item description is automatically copied to the memo field for the time transaction. You may turn off this preference at Setup > Accounting > Preferences > Accounting Preferences (Administrator) on the Time & Expenses subtab. If you use NetSuite OneWorld, you should set up service items that are available to all subsidiaries to use in intercompany time transactions. In these transactions, users can't save lines unless they contain service items available to both the employee subsidiary and customer subsidiary. See [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html). | May be shown or hidden |
| Payroll Workplace or Payroll Item Workplace | If your company supports Multi-State Calculations for payroll, select the **Payroll Item Workplace** for this time entry. | May be shown or hidden |
| Billable | Ensure that the **Billable** box is checked if the time is billable to a customer or project. Warning: In NetSuite CRM+, the **Billable** box isn't available. NetSuite CRM+ users can't record billable time, invoice customers for billable time, or record time for payroll items. | May be shown or hidden |
| Utilized | Displays a check mark if the employee's time directly contributed to the revenue for a project. | May be shown or hidden |
| Productive | Returns a check mark if the time bill includes time worked on a project but not included when calculating revenue for the project. Productive time is not billed to the customer. | May be shown or hidden |
| Exempt | Displays a check mark if the time bill is exempt from taxation. | May be shown or hidden |
| Payroll Item | If you are tracking time for payroll, select the payroll item that applies to this time entry. Selecting the correct payroll item ensures that the correct rate is applied. | May be shown or hidden |
| Paid Externally | Check the **Paid Externally** box if time has been or will be paid outside of NetSuite. This removes the time from payroll transactions. You can't check this box if this time record is already associated with a paycheck in NetSuite. If you tracked time for hourly wage payroll items and did not check the **Paid Externally** box, the time appears in the **Hours** column for this employee on the Payroll Run page. | Always shown |
| Type | The type of time transaction is displayed here. Actual time is time that has been worked by an employee. Planned time is time that has been accounted for when planning a project. Allocated time is time that has been assigned due to a resource allocation. | May be shown or hidden |
| Price or Price Level | If the **Override Rates on Time Records** preference has been enabled on the **Time & Expenses** subtab at Setup > Accounting > Accounting Preferences, the following fields display: Price Level, Rate, and Lock this Rate. Select a price level. You can use different price levels by going to Setup > Enable Features > Customers/Sales, and checking the **Use Multiple Prices** box. | Always shown |
| Rate | If you selected a price in the **Price Level** field, it automatically appears here. If you don't use multiple prices or if you selected **Custom** in the **Price Level** field, enter a rate for this time transaction. If you are entering time for a payroll item like vacation time, leave this field blank. | Always shown |
| Lock this Rate | If you are billing this time back to a customer, check this box to lock the rate you enter so it's not affected by rate changes that happen before the customer is billed. If you are entering time for a payroll item like vacation time, leave this field blank. | May be shown or hidden |
| Memo | Optionally enter a memo. You can search for the text you enter here to find this transaction later. If you are billing this time back to a customer or project, this memo appears as a description for this line item on the customer invoice. Note: Always select an activity in the **Case/Task/Event** or **Service Item** fields before entering a memo. When you select a case, task, event, or service item, the memo field is automatically populated with information from these records. Anything you entered in the memo field prior to selecting one of these records will be deleted. Changing your selection in either of these fields will update the memo field with any information from the newly selected record. | May be shown or hidden |
| Rejection Note | If you are rejecting this time entry, enter a rejection note for this time entry. Rejection notes are used to explain why an entry was rejected. | May be shown or hidden |
| Supervisor Approval | Check this box if you have authority as a supervisor to approve this time entry. | May be shown or hidden |
| Approval Status | If your company uses Advanced Approvals for Time and you are a supervisor or time approver, select a status for this time entry in the **Approval Status** field. | May be shown or hidden |
| Next Approver | If you use Approval Routing, you can also select another approver in the **Next Approver** field. For more information, see [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html). | May be shown or hidden |

### Classification Section Standard Fields {#subsect_9020627595}

| Field | Description | Field Availability |
| --- | --- | --- |
| Subsidiary | The subsidiary associated with the employee is displayed here. | May be shown or hidden |
| Department | Select the department that applies to this transaction. To set up a new department, click **New**. | May be shown or hidden |
| Class | Select the class that applies to this transaction. To set up a new class, click **New**. | May be shown or hidden |
| Location | Select a location to associate with this transaction. To set up a new location, click **New**. | May be shown or hidden |
| Billing Class | Select a billing class for this time entry. If a billing class is selected for this employee, it is automatically selected. | May be shown or hidden |

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html)
-   [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html)
-   [Giving an Employee Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html)
-   [Restricting Employee Time Tracking Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html)
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
