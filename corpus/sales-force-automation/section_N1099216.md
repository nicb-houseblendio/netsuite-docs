---
id: "section_N1099216"
type: "section"
title: "Tracking Time on Relationship Records"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Tracking Time on Relationship Records"
parent: "chapter_N1074872"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099216.html"
anchors: ["procedure_N1099284", "procedure_N1099578"]
sha256: "1ed7173e512419343a7c5b6fcb73a7d4db53057a063cb3acc2d08542475e1443"
---

You can track time and view reports for the amount of time spent working for or with leads, prospects or customers.

To track time, an administrator needs to go to Setup > Company > Enable Features. In the Employees subtab, click the **Time Tracking for CRM** box. With Time Tracking for CRM, you can track time on tasks, phone calls, events, and cases.

Tracking time on activities per customer can help you manage your company's time and bill time back to customers. For more information, see [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html).

#### To track time on relationship records: {#procedure_N1099284}

1.  On the lead, prospect or customer record, click the **Financial** subtab.
    
2.  Under the **Financial** subtab, click the **Time Tracking** subtab.
    
    Note:
    
    If any case, task, or event record has more than 9500 time entries displayed, all records show a static list of time entries. You can't edit entries directly from the list.
    
3.  Click **New Time**.
    
4.  Under Primary Information:
    
    Your name appears in the **Employee** field. Depending on your role access, you can select another employee if you're entering time for someone else.
    
    1.  In the **Date** field, enter the date for this time entry.
        
    2.  In the **Duration** field, enter or calculate how much time this employee worked on this call in hours.
        
    3.  If the time is tracked for a project task, select the project task in the **Task** field.
        
    4.  In the **Service Item** column, select the service item associated with this call.
        
    5.  Ensure that the **Billable** box is checked if you want to be able to bill this time to the customer.
        
        Now you can bill this customer for this time on the **Billable Time** subtab of invoice transactions.
        
    6.  Check the **Utilized** box if this time isn't considered utilized time spent toward completing a project task.
        
    7.  Check the **Productive** box if this time is spent toward completing a project task.
        
    8.  Check the **Exempt** box if this time isn't considered for utilization calculation.
        
    9.  In the **Payroll Item** field, select the payroll item to pay this employee for this time entry.
        
    10.  In the **Memo** field, write a brief description about what this employee did during this time.
         
5.  Under Classification, if you track departments, locations or classes, select the corresponding information for this time.
    
6.  Click **Save**.
    
7.  Repeat this process to track time for additional employees.
    
8.  When you finishd entering information for this record, click **Save**.
    

Employees still need to enter their time in the Employee Center, but you can see their time spent per customer at _Reports > Time & Billables > Time by Customer > Detail_.

All employee names are listed on the **Time** subtab, by default. Administrators can control which names show for certain roles in this list by going to Setup > Users & Roles > Manage Roles.

#### To restrict employees to enter time for only themselves or their subordinates: {#procedure_N1099578}

1.  Go to _Setup > Users/Roles > User Management > Manage Roles_.
    
2.  Click **Customize** next to the role you want to restrict.
    
3.  Create a new name for the restricted role.
    
4.  In the **Employee Restrictions** field, select one of the following:
    
    -   **none - no default** - Employees can select any employee in lists and track time for anyone.
        
    -   **none - default to self** - Employees can select any employee in lists and track time for anyone, but the Employee field defaults to the person entering the time.
        
    -   **own, subordinates, and unassigned** - Employees can select either their own name, the names of their subordinates, or unassigned employees.
        
        Employees are considered your subordinate if you're selected as their supervisor on employee records. Unassigned employees have no supervisor assigned.
        
    -   **own and subordinates only** - Employees can select either their own name or the names of their subordinates.
        
        Employees are considered your subordinate if you're selected in the Supervisor field on employee records.
        
5.  Click **Save**.
    
6.  Repeat these steps for each role you want to restrict from being able to enter time for every employee.
    

Now, go to _Lists > Employees > Employees_. Reassign your employees the new custom role.

For customized roles, the list of employees on the **Time** subtab only includes that employee's name and the name of that employee's subordinates. The **Time** subtab appears on the event, task, phone call, and case records.

### Related Topics

-   [Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1074872.html)
-   [Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1075037.html)
-   [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html)
-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)
-   [Prospect Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1096136.html)
-   [Competitors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1096618.html)
-   [Other Name Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1096940.html)
-   [Records as Multiple Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099012.html)
-   [Entering an Address on a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099791.html)
-   [Printing Mailing and Shipping Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099985.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
