---
id: "section_N944846"
type: "section"
title: "Running Test Payroll Batches"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Running Test Payroll Batches"
parent: "chapter_N917379"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N944846.html"
anchors: ["procedure_N944909"]
sha256: "58fc365ffaa5a8e155a0d5f478327afa9880936675cfc587dc0e21a54d850d33"
---

Running test payroll batches helps you to verify that SuitePeople U.S. Payroll correctly calculates the payroll information that you set up for each employee.

Your payroll setup is not complete until you do the following:

1.  Enter Year To Date (YTD) information OR select the option indicating you have no YTD information to report.
    
2.  Run at least one test payroll.
    

You can run as many test payroll batches as you like. Test payroll batches do not affect your current data and are deleted from the system when you turn off Payroll Test Mode in your account.

#### To run a test payroll batch: {#procedure_N944909}

1.  Go to _Setup > Payroll > Set Up Payroll_.
    
2.  If you have a NetSuite OneWorld account, select a subsidiary from the list in the **Subsidiary** field.
    
    For more information, see [Payroll Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275739.html).
    
3.  Ensure that the **Run Payroll in Test Mode** box is checked. Click **Save**.
    
4.  Go to _Transactions > Employees > Create Payroll_.
    
5.  If you have a NetSuite OneWorld account, select a subsidiary from the list in the **Subsidiary** field.
    
6.  In the **Pay Frequency** field, select the range that describes how often you pay the employees you want to include in this payroll.
    
    Note:
    
    The frequency you select in this field filters the list of employees on this page who are included in the payroll run.
    
7.  In the **Period Ending** field, accept or change the last date of the payroll period.
    
    This date is based on the last paid date and pay frequency entered on the employee record.
    
8.  Click **Create**.
    
9.  Select the employees to include in the payroll batch:
    
    1.  In the **Workplace** field, select a workplace to filter the list.
        
        For details about workplace records, see [Entering Workplace Records for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918520.html).
        
    2.  In the **Department** field, select a department.
        
        For details about department records, see [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html).
        
    3.  In the **Class** field, select a class.
        
        For details about class records, see [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html).
        
    4.  In the **Select** column, check the boxes next to the employees you want to include in the payroll batch. Click **Mark All** to select all employees in the list.
        
10.  Click **Save**.
     
11.  In the **Check Date** field, accept or change the posting date of the paychecks.
     
     Note:
     
     This date cannot be a previous date, a weekend, or a bank holiday. To enter a check for today's date, you must check the **To Be Printed** box and locally print the check. SuitePeople U.S. Payroll cannot process direct deposits or service-printed checks on the same day.
     
12.  Check or clear the following boxes:
     
     1.  To save the checks and direct deposit vouchers in a queue for printing later, check the **To Be Printed** box.
         
         Important:
         
         If you do not check this box, paychecks and direct deposit vouchers are not printed for this payroll. To print checks and vouchers later, you must individually access and print each transaction. If you use the Service Printed Checks and Stubs feature, do not check this box. To print the checks yourself for this payroll run only, check this box. By default, this box is not checked for future payrolls.
         
     2.  To pay approved commission amounts, from NetSuite Commissions, on the paychecks included in this run, check the **Pay Commissions** box.
         
     3.  To pay approved expense amounts (from NetSuite) on the paychecks included in this run, check the **Pay Expenses** box.
         
         You must set up an expense payroll item to use this preference. For more information, see [Creating Payroll Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556724572.html).
         
     4.  If you do not want to accrue vacation or sick time on the paychecks included in this run, check the **Do Not Accrue Time** box.
         
     5.  To pay PTO on the paychecks included in this run, check the **Pay PTO** box.
         
13.  Verify the hours and amounts shown for the earning items listed.
     
14.  To run your test payroll and view the checks created on the Payroll Batch page, click **Calculate**.
     
15.  On the Payroll Batch page, on the **Complete** tab, click **View** next to an employee's name to view the details on their paycheck.
     
     If you need to make changes, click **Edit** to change any payroll related information about the paycheck record.
     
16.  Compare and verify employee withholding and deduction calculations with your most recent payroll run.
     

If you discover errors during your test payroll runs, go to _Lists > Employees > Employees_ to make the necessary changes to employee records. Then, to go to _Transactions > Employees > Create Payroll_ to rerun your test payroll.

If you make changes, you may be required to update your payroll information before running another test payroll. To update your payroll information, go to _Setup > Payroll > Update Payroll Information_.

When you complete your test runs, turn off the test mode so that you can run payrolls. For more information, see [Turning Off Payroll Test Mode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N945490.html).

### Related Topics

-   [Enabling Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N917966.html)
-   [Entering Company Information for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918232.html)
-   [Entering Workplace Records for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918520.html)
-   [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html)
-   [Payroll Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N920073.html)
-   [Retirement Plan Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162558111263.html)
-   [Payroll Items Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930985.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)
-   [Setting up Year-To-Date Information From Your Previous Payroll System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N944369.html)
-   [Entering a Payroll Start Date](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N945629.html)
-   [Payroll Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N917379.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
