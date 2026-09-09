---
id: "section_N2397278"
type: "section"
title: "Using Custom Workflow-Based Approvals for Expense Reports"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Expense Reports and Purchase Requests > Expense Reporting > Approving an Expense Report > Using Custom Workflow-Based Approvals for Expense Reports"
parent: "section_N2396195"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2397278.html"
anchors: ["procedure_N2397865"]
sha256: "fff6ce9f9ca80da699f623fad6bf2d8e3c5008c2428b0ab3ae560cbb285c657c"
---

You can use SuiteFlow to create a custom workflow to process approvals for expense reports. Using SuiteFlow for expenses provides more flexible processes for approvals.

For example, using workflows to process expenses allows for using a non-sequential approval process or conditionalized routing. You can set up a workflow that requires action from specific employees. You can show buttons on forms at certain stages, sends email based on actions taken, and much more.

Note:

If you previously used the Approval Routing feature for purchase approvals, read [Switch From the Approval Routing Feature to Suiteflow for Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3960252081.html) before you proceed.

#### To use SuiteFlow to process expense reports:

1.  To enable features, go to _Setup > Company > Setup Tasks > Enable Features (Administrator)_.
    
    1.  On the **Transactions** subtab, enable the **Expense Reports** feature.
        
    2.  On the **SuiteCloud** subtab, check the **SuiteFlow** box.
        
    3.  Click **Save**
        
    4.  On the **Employees** subtab, check the **Approval Routing** box.
        
    5.  click **Save**
        
        This feature must be enabled to use these fields on employee records:
        
        -   Purchase Limit
            
        -   Purchase Approver
            
            These fields are required for use with the workflow.
            
2.  To enable Approval Routing for expense reports, go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
    1.  To use SuiteFlow for expense approvals, on the **Approval Routing** subtab, check the **Expense Reports** box.
        
3.  Set up an approval workflow. You must use SuiteFlow to create a workflow to apply to your expense reports.
    
    For more information, see [Creating Your First Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html).
    
    You can incorporate the following options into your expense approvals workflow:
    
    -   Hierarchical or custom routing rules
        
    -   Email notifications that include links to drill down to records for approval
        
    -   Approve and Reject buttons
        
    -   Respecting approval limits
        
    -   Updating the Approval Status and Next Approver field on records
        
    -   Preventing records that are pending approval from being edited
        
    -   Designating an alternate approver
        

Note:

If a record goes through several approval levels with different users in a routing loop, use a custom workflow field that refers specifically to the current approver's approval status. This way, you can track the current approver's approval status separately from the overall status of the record.

## Approving an Expense in the Employee Center Using SuiteFlow {#procedure_N2397865}

When you use SuiteFlow for expense approvals, the Employee Center is the primary workspace for processing expense approvals.

-   The Employee Center shows the Expense Reports to Approve reminder and Approve Expense Reports queue.
    
-   Employees are shown all expenses for which they are the next approver.
    
-   Users aren't required to have the Full permission for the Employee Center to approve and reject expenses through the Employee Center. They can do so with only the View permission.
    
-   Reminders that show in the Employee Center drill down to the approval queue page for expense reports. You can still click through notification email and use the buttons on the expense form (such as Approve, Reject, and so on.)
    
-   An approver associated with one subsidiary is able to see only records that are associated with the same subsidiary to make approvals.
    

#### To approve an expense using SuiteFlow:

1.  Log in to the Employee Center.
    
2.  Click **Approve Expense Requests**.
    
3.  Select a process in the **Action** field.
    
    The Action field lists the available actions of all expense workflows. For example, you can select the workflow action of Approve, or alternately select the action Reject.
    
    Actions available in the field are shown as follows:
    
    Workflow name : Workflow state : Workflow action
    
    This is an example of a workflow action selection:
    
    Expense Approval Routing : Pending Approval : Approve
    
    The third section shows the action that will be implemented for the selected purchases. In the case above, that action is to Approve.
    
    The selection you make in the Action field filters the list of purchases that are displayed.
    
    For example, select the action 'Expense Approval Routing : Pending Approval : Approve.' The list of expenses that appear are only ones that meet the following conditions:
    
    -   Uses the workflow named Expense Approval Routing
        
    -   Has a status of Pending Approval
        
    
    You can select All in the Action field to show expenses associated with all workflows and actions.
    
4.  After you select the workflow and action, check the **Select** box next to each expense you want to process using the action you have selected.
    
5.  Click **Submit**.
    

You also have the option of manually selecting a status in the **Approval Status** field on an expense.

### Related Topics

-   [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
