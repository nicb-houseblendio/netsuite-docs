---
id: "section_N907404"
type: "section"
title: "Approving or Rejecting a Time Transaction"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Approving or Rejecting a Time Transaction"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html"
anchors: ["bridgehead_4508220976", "subsect_158799487912", "subsect_156987245671", "subsect_158799489763", "subsect_1537542242"]
sha256: "dcc6412083a5d00d473f0fb4cd7c4414555fbd95da36fb3bb2fb160dfea568c2"
---

Time approval is restricted to the Employee Center and the user role. You can either have your users track and approve time in the Employee Center or you can edit the user role and set employee restrictions. If you don't set employee restrictions on the user role, users can approve all time entries rather than only those of their subordinates.

You can select either a time approver or supervisor.

-   The Time Approver field appears on the Time Tracking subtab of an employee record.
    
-   The Supervisor field shows under Primary Information about an employee record.
    

After you assign a time approver or supervisor to an employee record, that user has the authority to approve time for the employee. Time approvers can't edit or delete existing time entries. If no time approver is selected, then the employee's supervisor approves time entries. If both a supervisor and a time approver are selected, then only the time approver can approve time entries using their Employee Center role. For more information, see [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html).

With **Customize View** you can specify details that you want to appear on timesheets. For example, Allocated Hours or Approval Status.

The employee's supervisor or time approver receives an email notification when time is entered or edited.

If you also use Project Management, you have additional options for approving project time. For more information, see [Approving Time and Expenses for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192683.html).

## Advanced Approvals {#bridgehead_4508220976}

The Advanced Approvals preference offers additional statuses, a color-coded display when viewing weekly time tracking and weekly timesheets, and the ability to reject time entries and add a rejection note. After you have enabled the preference, the Supervisor Approval field on time entries and weekly time tracking and timesheets is replaced by an Approval Status field.

This field is editable by administrators and any role without time and expense restrictions. This field enables you to set the status of time entries to Open, Pending Approval, Approved, or Rejected. When viewing weekly time tracking or timesheets, approved entries are displayed with a green background, open entries have a white background, rejected entries have a red background, and pending entries have a blue background.

### Setting Approval Preferences {#subsect_158799487912}

#### To set approval preferences:

1.  Go to Setup > Accounting > Accounting Preferences.
    
2.  Click the **Time & Expenses** subtab.
    
3.  Check the **Require Approvals on Time Records** box.
    
4.  If you'd like to use Advanced Approvals, check the **Advanced Approvals on Time Records** box.
    
5.  Click **Save**.
    

Warning:

If you decide at a later date to disable the Advanced Approvals preference, you must first adjust any time transactions with an Open or Rejected status to a Pending Approval status. Making these adjustments will prevent any further complications when the preference is turned off.

If you choose to enable Advanced Approvals on Time Records, you can also use SuiteFlow and Approval Routing to create custom approval workflows for your time entries. When using custom approval workflows, the Approve Time page is only available for time entry records. The Approve Timesheets pages is not available for custom approval workflows. For more information, see [SuiteFlow Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4068260113.html) and [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html).

For more help setting up the time tracking feature and related preferences, see [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html).

With Time Tracking, you can approve individual time entries from the Approve Time page.

### Approving or Rejecting Time with Time Tracking {#subsect_156987245671}

#### To approve or reject time with Time Tracking:

1.  Go to _Transactions > Employees > Approve Time_.
    
    Note:
    
    If you also use Weekly Timesheets, approving time defaults to the Approve Timesheets view. For more information see below. You can click **Switch to Time Entry view** to proceed with approving or rejecting time entries individually.
    
2.  On the Approve Time page, select the name of the employee whose time you want to approve or reject.
    
    You can also identify a specific pay period for that employee by selecting a date in the **Week Of** field.
    
    For this employee, each time record displays the following information by default:
    
    -   **Employee name**
        
    -   **Date of the time record**
        
    -   **Case/Task/Event**
        
    -   **Customer**
        
    -   **Service Item**
        
    -   **Payroll Item**
        
    -   **Number of hours entered**
        
    -   **Memo**
        
    -   The **Billable** column indicates if the time entered can be billed back to the customer.
        
3.  Optionally, click **Customize** to add filters or to select the columns to display on the Approve Time page. On the Customize page:
    
    1.  Click the **Criteria**, **Results**, or **Available Filters** subtabs.
        
    2.  Add or remove fields on the **Criteria** subtab to filter the results by other fields. Add or remove fields on the **Results** subtab to change the columns displayed. Add or remove fields on the **Additional Filters** to add filters to the page.
        
4.  In the **Select** column, check the boxes next to the time records you want to approve or reject.
    
    Important:
    
    You can't approve and reject entries together. All the entries you select will either be all approved or all rejected. If you have multiple entries to both approve and reject, you must repeat this process for approval and again for rejection.
    
    Note:
    
    You can approve or reject multiple time entries at one time, but record must be selected. You can't select time entries on a weekly basis from the Approve Time page.
    
5.  Click **Approve** to approve the selected time entries.
    
    Click **Reject** to reject the selected time entries without a rejection note.
    
    Click **Reject with Note** to reject the selected time entries and add a rejection note to each selected entry. You can only add a single rejection note. The note you enter is copied to all the selected time entries.
    
    Warning:
    
    Employees with appropriate permissions can modify previously approved time.
    

If you use Weekly Timesheets, you can approve or reject multiple entries in bulk.

### Approving or Rejecting Time with Weekly Timesheets {#subsect_158799489763}

#### To approve or reject time with Weekly Timesheets:

1.  Go to _Transactions > Employees > Approve Time_.
    
2.  On the Approve Timesheets page, select the name of the employee whose time you want to approve.
    
    You can also identify a specific pay period for that employee by selecting a date in the **Week Of** field.
    
    For this employee, each time record displays the following information by default:
    
    -   **Employee**
        
    -   **Period**
        
    -   **Approvable Hours**
        
        You can click the link in the **Approvable Hours** column to open a popup that displays the individual time entries.
        
    
    Optionally, you can click **Switch to Time Entry view** to display each time entry.
    
3.  Optionally, click **Customize** to add filters or to select the columns to display on the Approve Timesheets page. On the Customize page:
    
    1.  Click the **Criteria**, **Results**, or **Available Filters** subtabs.
        
    2.  Add or remove fields on the **Criteria** subtab to filter the results by other fields. Add or remove fields on the **Results** subtab to change the columns displayed. Add or remove fields on the **Additional Filters** to add filters to the page.
        
4.  In the **Select** column, check the boxes next to the timesheets you want to approve or reject.
    
    Important:
    
    You can't approve and reject timesheets together. All the timesheets you select will either be all approved or all rejected. If you have multiple timesheets to both approve and reject, you must repeat this process for approval and again for rejection.
    
    Note:
    
    When approving or rejecting time entries from the timesheet view, checking the box next to a timesheet will approve or reject all entries listed on the timesheet. When approving or rejecting time entries from the time entry view, each box approves or rejects only the individual time entry.
    
5.  Click **Approve** to approve the selected timesheets.
    
    Click **Reject** to reject the selected timesheets without a rejection note.
    
    Click **Reject with Note** to reject the selected timesheets and add a rejection note to each selected entry. You can only add a single rejection note. The note you enter is copied to all the selected time entries.
    
    Warning:
    
    Employees with appropriate permissions can modify previously approved time.
    

Approved time can be used to bill customers and process payroll.

If you bill time back to a customer or project, the time shows on the Billable Time subtab on the invoice.

If you track time for hourly wage payroll items, the time shows in the Hours column for each employee on the Payroll Run page.

Warning:

NetSuite CRM+ users can't record billable time, invoice customers for billable time, or record time for payroll items.

## Approving or Rejecting Time from the Time Transaction List {#subsect_1537542242}

You can use inline editing and the time transactions list to approve or reject time. If you use the Require Approvals on Time Records preference, you can check the box in the Approved column to update the approval status of individual time transactions with inline editing. The Approval Status field is not available for inline editing with only the approvals preference. If you also use the Advanced Approvals on Time Records preference, you can update the Approval Status field using inline editing.

For more information about Advanced Approvals, see [Advanced Approvals](#bridgehead_4508220976).

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html)
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
-   [Custom Workflow-based Approvals for Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554190531.html)
-   [Updating Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156408321759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
