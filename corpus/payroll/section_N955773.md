---
id: "section_N955773"
type: "section"
title: "Allocating Paycheck Expenses to Projects"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Transactions > Allocating Paycheck Expenses to Projects"
parent: "chapter_N945815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N955773.html"
anchors: ["procedure_N955823"]
sha256: "968c7e09e44c1af8b1d60d090530cb7ade17e13c16893661b55caed21d05ba1c"
---

The Time Tracking feature enables you to record the hours that employees work. If the Project Management feature is also enabled, you can link employees' hours worked to specific projects. If you use these two features with SuitePeople U.S. Payroll, you can allocate payroll expenses to specific projects to track projects' profitability.

To allocate paycheck expenses to projects, the following should be true:

-   When both hourly and salaried employees submit time entries, they must link their time worked with a project. Employees can select projects from the **Customer:Project** field.
    
-   The project that employees track time for must be associated with a customer. For more information, see [Creating a Basic Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1179164.html).
    

After the payroll run is complete, you can allocate the expenses by creating journal entries to associate payroll amounts with specific projects. This means that only Actual Time/Hours worked are used for expense allocation.

For salaried employees, earnings and company contribution expenses can be allocated to projects.

Note:

To determine the amounts to allocate to a project, note the following. NetSuite calculates a percentage based on the amount of time entered for a project over the amount of time recorded for the pay period. This percentage is applied to the paycheck lines that are posted for an expense account or a Cost of Goods Sold (COGS) account. If an employee enters time for a project but does **not** select a payroll item for that project, note the following. That time is used in the calculation of the allocation percentage even though the time is not included in payroll.

#### To allocate paycheck expenses to projects: {#procedure_N955823}

1.  Go to _Transactions > Employees > Allocate Paycheck Expenses to Projects_.
    
    This page shows unallocated payroll amounts for employees who entered time worked for the pay period and selected a project associated with a customer. To narrow the list of amounts, you can select from the **Date** field or enter dates in the **From** and **To** fields.
    
2.  In the **Journal Entry Date** field, enter the date that you want to use for the paycheck allocation journal entries.
    
3.  For each paycheck amount you want to allocate to a project, check the **Select** box. To select all payroll amounts, click **Mark All**.
    
4.  To create journal entries for the selected payroll amounts, click **Allocate**.
    
    For each amount:
    
    -   The amount is credited to the Payroll Funding Account.
        
    -   An equal amount debits the account associated with the project.
        
    -   The names of the project and payroll item appear in the Memo field on the journal entry.
        
    
    Amounts on each paycheck must be allocated using only one journal entry. A journal entry allocation can have a maximum of 200 lines. For more information about line limitations, see [Limitations for Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159361107074.html).
    

Note:

Time entries do not determine the classifications (class, department, or location) or custom segments for allocated paycheck expenses. Instead, the paycheck record determines the classifications and the employee record determines the custom segments for allocated paycheck expenses.

### Related Topics

-   [Processing Payroll Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N947159.html)
-   [Searching for Paychecks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N950964.html)
-   [Payroll Dashboard Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544802669.html)
-   [Print Payroll Checks or Vouchers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N955656.html)
-   [Payroll Reversals and Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951824.html)
-   [Recording Third-Party Sick Pay Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N953245.html)
-   [Payroll Transaction Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N953616.html)
-   [Making Payroll Liability Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N954201.html)
-   [Complete Quarterly or Yearly Payroll Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N954521.html)
-   [Payroll Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N945815.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
