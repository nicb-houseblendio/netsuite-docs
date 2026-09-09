---
id: "section_N921988"
type: "section"
title: "Including an Employee in Payroll"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Setup for Employees > Including an Employee in Payroll"
parent: "section_N921632"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html"
anchors: ["procedure_N922000"]
sha256: "dfd27f6fb0677be8a8a5a94abb18250e0a7dbea0ffd33066fdf9943d98ec4071"
---

After you enable the Payroll feature, the Payroll subtab appears on employee records. You must enter the required information about this subtab to pay your employees through NetSuite.

#### To include an employee in Payroll: {#procedure_N922000}

1.  Go to _Lists > Employees > Employees_, and do one of the following:
    
    -   To create an employee record, click **New**.
        
    -   To add an existing employee to payroll, click **Edit** next to the employee name.
        
2.  On the **Address** subtab, enter the employee's address. The home address is used to calculate state and local taxes. For more information, see [Entering an Address for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N895137.html).
    
    Note:
    
    You can use the home address along with a workplace address.
    
3.  On the **Human Resources** subtab, enter values in the **Social Security Number**, **Birth Date**, and the **Hire Date** fields.
    
4.  If the employee is newly hired, click the **Medical Insurance** subtab and enter medical insurance information for the employee. For more information, see [Medical Insurance Information for New Hire Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0723111210.html).
    
5.  On the **Payroll** subtab, do the following:
    
    -   Check the **Include in Payroll** box. If you don't check this box, the employee cannot be paid with SuitePeople U.S. Payroll.
        
        If you use NetSuite OneWorld, you must select a **Subsidiary** for the employee that matches the **Subsidiary** defined at _Setup > Payroll > Set Up Payroll_. Otherwise, this box is unavailable. After you select a subsidiary, save the employee record. Then, reopen the record in edit mode to check the **Include in Payroll** box.
        
    -   In the **Compensation Type** field, select **Wage** or **Salary**, depending on whether your company pays this employee an hourly wage or a periodic salary.
        
        Important:
        
        If you use the Compensation Tracking feature and set up Payroll to copy compensation tracking information, enter compensation details on the **Compensation Tracking** subtab. For more information, see [Integrating Employees' Base Pay Information with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1496764441.html).
        
    -   In the **Pay Frequency** field, select how often this employee is paid.
        
    -   In the **Last Paid Date** field, for existing employees, enter or check the last date of the employee's most recent pay period.
        
        This is the most recent date employees were paid or should be paid. For example, if a pay period ends on October 7 but the paycheck is generated on October 10, the last paid date is October 7.
        
        For new employees, leave the Last Paid Date field blank.
        
        If you add an existing employee to payroll for the first time, manually enter the last date of their first pay period. This field updates automatically with the most recent pay-period end date each time you run payroll.
        
        Note:
        
        If this employee uses the Time Tracking feature, you must enter the employee's last paid date. This makes sure their pay is calculated correctly according to the Pay Earnings Prior to Pay Periods (Days) preference in payroll setup. For more information, see [General Payroll Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N920326.html).
        
    -   From the **Workplace** list, select where this employee works.
        
        The workplace determines which taxes the employer and employee need to pay.
        
        Important:
        
        If an employee lives in Washington, D.C. and works in a neighboring state, note the following. You must create a workplace with the same zip code as the employee's home address, but do not assign the workplace to the employee. After you create this workplace, if a reciprocity agreement is checked, employee tax withholding is calculated for only Washington, D.C. If a reciprocity agreement is not checked, withholding is calculated for both jurisdictions.
        
    -   If you set the **Decrease Elective Deferral Limits and Automatically Calculate Catch-Up** preference, you can override the employee's elective deferral limits. For more information, see [Decreasing Elective Deferral Limits for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162731062157.html).
        
6.  Click **Save**.
    

### Related Topics

-   [Setting up Direct Deposit for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N926100.html)
-   [Setting up Earnings for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924353.html)
-   [Setting up Deductions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924665.html)
-   [Setting up Company Contributions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924823.html)
-   [Setting up Accrued Time for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924963.html)
-   [Taxes and Jurisdiction Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556740089.html)
-   [Updating Payroll Items for Multiple Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N925941.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
