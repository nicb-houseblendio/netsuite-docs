---
id: "section_N924963"
type: "section"
title: "Setting up Accrued Time for an Employee"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Setup for Employees > Setting up Accrued Time for an Employee"
parent: "section_N921632"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924963.html"
anchors: ["procedure_N924987"]
sha256: "aed956277ebd6a5eb5fe961d680bc9da06a7ad47839f366d96ecdd9bdce06c2f"
---

For each employee in payroll, you can set up accrued time by adding sick and vacation payroll items to their record.

You might need to create earning payroll items for accrued time before you can select them for employees. For more information, see [Payroll Items Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930985.html).

Important:

If you use the Time-Off Management feature, see [Updating the Employee Record for Time-Off Management and Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519677675.html).

#### To set up accrued time for each employee: {#procedure_N924987}

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee's name, click **Edit**.
    
3.  Click the **Payroll** subtab, and then the **Accrued Time** subtab.
    
4.  In the **Accrued Time** subtab, do the following:
    
    1.  In the **Sick/Vacation Time** field, a payroll item for sick time, vacation time, or other paid time off (PTO) events.
        
        For example, you might have set up a payroll item called **PTO - Vacation**.
        
    2.  If you're setting up accrued time for this employee for the first time, in the **Accrued Hours** field, enter a beginning balance.
        
        After the beginning balance is set, the system keeps track of this total.
        
    3.  In the **Accrue As** field, select one of the following:
        
        -   **Lump Sums**: Calculate accrual based on total hours for the year. Accrual occurs with the employee's first payroll of the year and does not increase with subsequent payrolls.
            
        -   **Per Pay Period**: Calculate accrual per pay period.
            
        -   **Per Hour Worked**: Calculate accrual per hours worked. This includes overtime if the time was recorded.
            
    4.  In the **Accrual Rate** field, enter the number of hours this employee accrues for the time period set in the **Accrue As** column.
        
        -   If the **Accrue As** field is set to **Lump Sum**, the accrual rate should be the total number of hours per year.
            
        -   If **Accrue As** is set to **Per Pay Period**, the accrual rate should be the number of hours the employee earns per pay period.
            
        -   If **Accrue As** is set to **Per Hour Worked**, the accrual rate should be the amount of time off to accrue for each hour worked. For example, 0.04.
            
    5.  In the **Monetary Rate** field, enter the cost per hour of the accrued time.
        
    6.  To set the total accruals to zero and begin calculations again each calendar year, check the **Reset at Year End** box.
        
        Employees' accrued time is reset when the period ending date is in the new year. Note the following about employees taking time off during a pay period that includes both the previous year and the next. The time is taken from their previous year's balance, and then reset. If an employee's last paid date is blank, the accrued time is not reset.
        
    7.  If your company sets a limit for accrued time, in the **Maximum Hours** field, enter the maximum number of hours that can be accrued.
        
    8.  Click **Add**. Continue adding payroll items as necessary.
        
5.  Click **Save**.
    

### Related Topics

-   [Including an Employee in Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html)
-   [Decreasing Elective Deferral Limits for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162731062157.html)
-   [Setting up Direct Deposit for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N926100.html)
-   [Setting up Earnings for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924353.html)
-   [Setting up Deductions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924665.html)
-   [Setting up Company Contributions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924823.html)
-   [Taxes and Jurisdiction Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556740089.html)
-   [Updating Payroll Items for Multiple Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N925941.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
