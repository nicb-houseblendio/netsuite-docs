---
id: "section_N895403"
type: "section"
title: "Entering Human Resources Information for an Employee"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Employee Information Management > Adding an Employee > Entering Human Resources Information for an Employee"
parent: "section_N894212"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N895403.html"
anchors: ["bridgehead_N895821", "procedure_N895863"]
sha256: "4de46fa780f898f70d6db0ca55c6d7439f6faead5780bb8baf5590cc9d11f72b"
---

On the Human Resources subtab of the employee record, you can enter an employee's social security number, supervisor, hire date, and other information.

#### To enter Human Resources information for an employee:

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the employee's name.
    
3.  Click the **Human Resources** subtab.
    
4.  In the **Social Security** field, enter the employee's social security number. For information regarding social security number masking and encrypting, see [Working with Employee Social Security Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901259.html).
    
5.  Enter this employee's birth date.
    

#### To enter job information for an employee:

1.  From the **Type** list, select the type category that applies to this employee. For more information, see [Setting Up Employee Related Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1394576.html).
    
    The type determines whether the employee data is included in employee-related key performance indicators.
    
    To create new **Types**, go to _Setup > Accounting > Employee Related Lists > New_.
    
2.  Select the status of this employee's employment with your company.
    
    To create new selections for this field, go to _Setup > Accounting > Employee Related Lists > New_. For more information, see [Setting Up Employee Related Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1394576.html).
    
3.  Enter a job description for this employee.
    

Note:

If you use the Effective Dating feature and are assigned to a role with the Employee Effective Dating permission, note the following. You can see historical changes to an employee's status and type on the employee timeline. For more information, see [Viewing an Employee's Timeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156216462597.html).

#### To enter job information for sales reps:

1.  For sales reps, choose one of the following:
    
    -   If you don't use Team Selling, check the **Sales Rep** box to assign sales territories to the employee. You can also select them in the **Sales Rep** field on customer records and sales transactions.
        
    -   If you use Team Selling, and if the employee is a part of the sales team, select a field in **Sales Role**. For more information, see [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html).
        
    
    When the **Sales Rep** box is checked or a **Sales Role** is selected for an employee, NetSuite creates a customer record. The employee is selected as the default sales rep on the customer record.
    
2.  To assign cases or territories to the employee, check the **Support Rep** box.
    
3.  To assign the employee to work on projects and project tasks, check the **Project Resource** box.
    
    If the employee is a project resource, check the **Project Manager** field to add them to the Project Manager selection on project records.
    
    If the employee is a project resource, select a role in the **Default Projects Resource Role** field. When the employee is assigned to a project, the selected role is automatically assigned.
    
    When an employee is marked as a Project Resource, the **Target Utilization** field appears.
    
4.  Select a work calendar for the employee.
    
5.  In the **Labor Cost** field, enter the hourly overhead labor cost rate for this employee to calculate project costs and profitability.
    
6.  In the **Hire Date** field, enter the date the employee was hired.
    
7.  In the **Last Review Date** field, enter the date of the employee's last review.
    
8.  In the **Next Review Date** field, enter the date of the employee's next review.
    
9.  In the **Termination/Release Date** field, enter the person's last date of employment.
    
    #### Supervisor Change Hist. {#bridgehead_N895821}
    
    1.  This subtab shows system notes about changes to the employee's supervisor. For more information, see [Assigning a Supervisor to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898466.html).
        
    
    #### Work Status {#procedure_N895863}
    
    1.  Select the Employee's resident status.
        
        You can find this information in Section 1 of the employee's completed I-9 form.
        
        To create new selections for this field, go to _Setup > Accounting > Employee Related Lists > New_.
        
    2.  Select the employee's **Visa Type**.
        
        To create new selections for this field, go to _Setup > Accounting > Employee Related Lists > New_.
        
    3.  Enter the Visa's expiration date.
        
    4.  Enter the **Alien Number**.
        
        You can find this information in Section 1 of the employee's completed I-9 form.
        
        This step is required only if the employee's work status is **Alien authorized to work**.
        
    5.  Enter the date through which the employee is authorized to work.
        
        You can find this information in Section 1 of the employee's completed I-9 form.
        
        This step is required only if the employee's work status is **Alien authorized to work**.
        
    6.  On the **Work Status** subtab, check **I-9 Verified** if the employee has completed an I-9 form.
        
    

#### To enter expense and purchasing information:

1.  In the **Expense Limit** field, enter the amount the employee can expense without approval.
    
    This field defaults to $0, which requires all expenses to be approved.
    
2.  In the **Expense Approver** field, select the person that approves the employee's expense reports.
    
    If no approver is selected, the supervisor approves expense reports. If a supervisor and an expense approver are selected, either can approve expense reports. For more information about approvers and approval limits, see [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html).
    
3.  In the **Expense Approval Limit** field, enter the maximum amount an employee is allowed to approve on an expense report when specified as an approver.
    
4.  In the **Purchase Limit** field, enter the amount the employee can purchase without approval.
    
    This field defaults to $0, which requires all purchases to be approved.
    
5.  In the **Purchase Approver** field, select the person that approves the employee's purchase requests.
    
    If no approver is selected, the supervisor approves purchase requests. If both a supervisor and a purchase approver are selected, either can approve the purchase request.
    
6.  In the **Purchase Approval Limit** field, enter the maximum amount an employee can approve on a purchase request when specified as an approver.
    
7.  In the **Account** field, enter this employee's account number if needed.
    

#### To enter personal information for an employee:

1.  Select the employee's marital status.
    
    To create new selections for this field, go to _Setup > Accounting > Employee Related Lists > New_.
    
2.  Select the employee's ethnicity.
    
    To create new selections for this field, go to _Setup > Accounting > Employee Related Lists > New_.
    
3.  On the **Personal** subtab, select the employee's gender.
    
4.  Use the following information to enter or verify information in the additional subtabs on the **Human Resources** subtab.
    
    After you have entered all necessary information, click **Save**.
    

#### To enter medical insurance information (SuitePeople U.S. Payroll customers only)

For more information, see [Medical Insurance Information for New Hire Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0723111210.html).

1.  On the Medical Insurance subtab, check one or more of the following boxes, as appropriate:
    
    -   Medical Insurance Availability: Check this box if medical insurance is available for this employee.
        
    -   Medical Insurance Enrolled: Check this box if the employee is enrolled in medical insurance.
        
    -   Dependent Medical Insurance Availability: Check this box if the employee has medical insurance available for any dependents.
        
    -   Dependent Medical Insurance Enrolled: Check this box if the employee has any dependents enrolled in medical insurance coverage.
        
2.  To select all of the boxes, check **Select All**.
    
3.  If you have checked any of the boxes, enter the date when the employee qualifies for medical insurance for themselves or dependents in the **Medical Insurance Eligibility Date** field.
    

#### To enter emergency contacts for an employee:

1.  Enter the name of the employee's emergency contact.
    
2.  Enter the relationship between the contact and employee.
    
3.  Enter the address of the emergency contact.
    
4.  Enter the phone number for the emergency contact.
    
5.  Click **Add/Edit**.
    

#### To enter education information:

1.  On the **Education** subtab, select the employee's level of education.
    
    To create new selections for this field, go to _Setup > Accounting > Employee Related Lists > New_.
    
2.  Enter the **Degree** received.
    
3.  Enter the date the degree was conferred.
    
4.  Click **Add/Edit**.
    

### Related Topics

-   [Entering Communication Information on the Employee Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894944.html)
-   [Entering an Address for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N895137.html)
-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
