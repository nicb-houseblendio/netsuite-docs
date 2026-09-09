---
id: "section_N898466"
type: "section"
title: "Assigning a Supervisor to an Employee"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Employee Information Management > Assigning a Supervisor to an Employee"
parent: "chapter_N894090"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898466.html"
anchors: ["procedure_N898508", "subsect_160650392779"]
sha256: "25c7993eea0da7aaaec8f8aedeceb879aedbae571999a8fe1265ba86222b79e4"
---

In NetSuite, supervisors can approve the following for their supervised employees:

-   Expense reports, if no expense approver is assigned
    
-   Purchase orders, if no purchase approver is assigned
    
-   Time-off requests, if the Time-Off Management feature is enabled
    

If you enable the Employee Change Requests feature, supervisors can create employee change requests for their supervised employees. For more information, see [Employee Change Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156025845557.html).

For someone to be considered a supervisor in NetSuite, that person must be selected as the supervisor of another employee on that employee's record. The supervisor receives email when an employee enters a new time-off request, a new expense report, or a new purchase request that needs approval. For more information, see [Approving or Rejecting Time-Off Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4762829774.html) and [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html).

Note:

You can't make an employee's supervisor someone who is beneath that employee in the reporting hierarchy. In other words, you can't create a circular reporting structure.

#### To assign or change supervisors on employee records: {#procedure_N898508}

1.  Go to Lists > Employees > Employees.
    
2.  Click **Edit** next to the name of the person whose supervisor you want to assign or change.
    
3.  Under Primary Information, in the **Supervisor** dropdown, select the person who should be the supervisor of this employee. The employees who appear in this dropdown are the ones that you are permitted to assign as a supervisor to this employee. In other words, you can't assign someone below this employee in the reporting hierarchy.
    
4.  When you have finished editing the employee's record, click **Save**.
    

## Supervisor Changes and Commissions {#subsect_160650392779}

Supervisor changes can affect commissions for the supervisor, depending on their commission schedule. For example, the effective date for a supervisor change isn't the same as the date when the employee is updated. Therefore, the supervisor could be credited with less or more commissions than they should be. To avoid this, change the effective date for a supervisor change to a date in the future or in the past.

Note:

A change to a supervisor effective date doesn't cause a commission recalculation, which may be necessary to correct the commission amount.

#### To update a supervisor assignment:

1.  Go to Lists > Employees > Employees.
    
2.  Click **Edit** next to the employee.
    
3.  Under Primary Information, in the **Supervisor** field, select the supervisor's name.
    
4.  Click **Save**.
    

#### To update the supervisor change history for an employee:

1.  Go to Lists > Employees > Employees.
    
2.  Click **Edit** next to the employee.
    
3.  Under Primary Information, in the **Supervisor** field, confirm that the employee has the correct supervisor.
    
4.  Click the **Human Resources** tab.
    
5.  Click the **Supervisor Change Hist.** subtab.
    
6.  On the row with the relevant supervisor change, click **Edit**. Enter the correct date in the Effective Date field. Note that you can't enter effective dates of assignments that overlap. For example, an employee can't report to two supervisors at the same time. Click **Save**. Click **Close**.
    
7.  To save the employee record, click **Save**.
    

Note:

This manual change to the supervisor change history doesn't use the SuitePeople Effective Dating feature.

### Related Topics

-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
-   [Adding Employees by Importing a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322503072.html)
-   [Editing Employee Records Using CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322804075.html)
-   [Giving an Employee Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html)
-   [Viewing and Editing an Employee Record with Effective Dating](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494510731.html)
-   [Rehiring a Terminated Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160763200766.html)
-   [Searching for Effective-Dated Changes to the Employee Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503337187.html)
-   [Viewing an Employee's Timeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156216462597.html)
-   [Employee Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899090.html)
-   [Creating an Employee Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899487.html)
-   [Working with Employee Social Security Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901259.html)
-   [Printing Mailing Labels for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N916939.html)
-   [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
