---
id: "section_N2396195"
type: "section"
title: "Approving an Expense Report"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Expense Reports and Purchase Requests > Expense Reporting > Approving an Expense Report"
parent: "section_N907845"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html"
anchors: ["bridgehead_3960271715", "bridgehead_N2396336"]
sha256: "6bd2450726884444d4bcd43a083e7844f7289eb098bc548f2d98c7116b31df40"
---

If you use the Approval Routing feature for expenses, they must be approved before they can be processed.

Expenses are generally processed through the Employee Center. You must have the Employee Center role to access the Employee Center. An administrator can add the Employee Center role on your employee record. For more information, see [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html).

Note:

In OneWorld accounts, note the following when a user who is a supervisor or approver logs in to the Employee Center. Approval queues display purchase requests, expense reports, and requisitions entered by employees associated with all subsidiaries. Role-level subsidiary restrictions that apply to other records and transactions don't apply to approvals of purchase requests, expense reports and requisitions.

## Approving Expenses Using the Approval Routing Feature {#bridgehead_3960271715}

To approve an expense report, you must first log in to the Employee Center. You must have the Employee Center role to access the Employee Center. An administrator can add the Employee Center role on your employee record.

#### To approve an expense report:

1.  Log in to the Employee Center.
    
2.  Go to _Transactions > Employees > Enter Expense Reports > List_.
    
3.  View the report.
    
    If you're a supervisor and your direct reports submit an expense report, the **Approve** button is displayed.
    
4.  Click **Approve**.
    

Expense reports have no accounting impact until they're approved by someone with accounting authority. When expense reports are approved by a supervisor or approver, their totals remain in an unapproved non-posting account until approved by accounting. For more information, see [Giving Accounting Approval for Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913502.html).

If you don't use Approval Routing, the report is automatically routed to the employee's immediate supervisor and then to accounting.

If you use Approval Routing, the supervisor or approver must have an expense approval limit greater than or equal to the amount of the report. If the amount is greater than the expense approval limit of the supervisor or approver, the report is sent to the next level of management. This continues until it is approved by an authorized supervisor or approver.

If an expense approver is specified for an employee, the supervisor isn't part of the approval hierarchy.

Supervisors can automatically be notified when they have reports to approve. Only an administrator can enable supervisor notification. To enable this feature, go to _Setup > Accounting > Preferences > Accounting Preferences_. Check the Automatically Notify Supervisor box.

In the Employee Center, your employees can view the status and approval history of their expense reports. Employees click View & Edit Unapproved Expense Reports, or View Approved Expense Reports.

## Approving Expenses Using SuiteFlow {#bridgehead_N2396336}

If you use SuiteFlow for expense approvals, the steps to approve an expense depend on the way the workflow is set up. For more information, see [Using Custom SuiteFlow Workflows for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396465.html) and [Using Custom Workflow-Based Approvals for Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2397278.html).

### Related Topics

-   [Switch From the Approval Routing Feature to Suiteflow for Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3960252081.html)
-   [Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908140.html)
-   [Employee Access to Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908637.html)
-   [Enter an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N911232.html)
-   [Editing an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550694498.html)
-   [Deleting an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746063133.html)
-   [Rejecting an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751910971.html)
-   [Corporate Card Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531259544.html)
-   [Reviewing Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913094.html)
-   [Giving Accounting Approval for Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913502.html)
-   [Paying Expenses on Employee Paychecks with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914230.html)
-   [Giving an Employee Access to Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914882.html)
-   [Notifying a Supervisor or Approver About Required Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N910874.html)
-   [Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907845.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
