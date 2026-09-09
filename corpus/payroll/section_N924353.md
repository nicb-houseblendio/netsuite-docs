---
id: "section_N924353"
type: "section"
title: "Setting up Earnings for an Employee"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Setup for Employees > Setting up Earnings for an Employee"
parent: "section_N921632"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924353.html"
anchors: ["procedure_N924380", "procedure_0819012756"]
sha256: "c2f2f0e91b47d60ee7029047aa7dd7c79630b322a7e7f4c35e85cbe5aeda9f4f"
---

For each employee in Payroll, you can add earning payroll items to their record. These payroll items help figure out the employee's gross pay.

Before you set up earnings for an employee, make sure you've created earning payroll items. For information, see [Creating Payroll Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556724572.html).

Important:

If you use the Compensation Tracking feature and set up Payroll to copy compensation tracking information, enter compensation details on the **Compensation Tracking** subtab. For more information, see [Integrating Employees' Base Pay Information with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1496764441.html).

Also, make sure the primary payroll item has a rate (not a multiplier), isn't based on another payroll item, and is either Earning:Salary or Earning:Wage.

#### To set up earnings information for an employee: {#procedure_N924380}

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee's name, click **Edit**.
    
3.  Click the **Payroll** subtab, and then the **Earnings** subtab.
    
4.  In the **Earning** field, choose one of the payroll items you set up for earnings.
    
    For example, you may have set up a payroll item called **Regular Hourly Wages**.
    
    An employee shouldn't have both wage and salary items at the same time. If you previously selected a wage item for the employee, the wage item must be inactivated to add a salary payroll item.
    
5.  In the **Rate** field, enter the rate for this type of earning.
    
    For example, if you are setting up wages for an employee, you might enter 22.00 for an employee earning $22 per hour. If you are setting up annual salary for an employee, you might enter 45000.00 for an employee earning $45,000 per year.
    
6.  If this payroll item is the employee's main pay item, check the **Primary** box. The Primary box has the following uses:
    
    -   You can use the **Primary** attribute to filter records for reporting and search purposes. This lets you obtain lists of employee salaries and wages, without the clutter of information from other earning payroll items. The following related fields are available as search filters and displayed as search results: **Primary Earning Type**, **Primary Earning Item**, and **Primary Earning Amount**.
        
    -   If you use the Compensation Tracking feature, and you set up Payroll to copy compensation tracking information, note the following. The Compensation Tracking feature uses the Primary box to determine which payroll item to automatically update. Make sure that:
        
        -   The primary payroll item has a rate (not a multiplier)
            
        -   Is not derived from another payroll item
            
        -   Has an item type of either Earning:Salary or Earning:Wage
            
        
        For more information, see [Integrating Employees' Base Pay Information with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1496764441.html).
        
7.  In the **Default Hours** field, enter the default number of hours this person is paid for this earning type. To create an additional pay using the rate and default hours, check the **Default** box.
    
    -   If you select a payroll item with the type Earning:Salary, the system calculates the amount even if you leave the **Default Hours** field blank. This is also true if you enter 0 (zero).
        
    -   If you select a payroll item with the type Earning:Wage, the hours entered in time tracking are used to calculate earnings. In addition, checking **Default** will add an earning amount equal to default hours multiplied by rate, regardless of hours entered by time tracking.
        
    -   If you select a payroll item and you leave the **Default Hours** field blank or enter zero, then the earning type is not calculated.
        
8.  To prevent the use of this item for this employee, check the **Inactive** box.
    
9.  If this item is to appear on the paycheck every time you run payroll, check the **Default** box. This additional pay is not calculated if you leave the **Default Hours** field blank or enter zero.
    
10.  Enter the **Effective Date** and **Expiration Date** for the payroll item. These dates are checked against the payroll period ending date to determine which payroll items are affected.
     
11.  Click **Add**.
     
12.  Add more earning items as needed.
     
13.  Click **Save**.
     

You can also set up a one-time earning item for an employee.

#### To set up a one-time earning item for an employee: {#procedure_0819012756}

1.  Go to _Transactions > Employees > Create Payroll > List_.
    
2.  Click **Edit** on the paycheck batch that includes the employee you want to add the one-time earning item for.
    
3.  On the **Complete** subtab, click the **Paychecks** subtab.
    
4.  Click **Edit** on the name of the person for you want to add the one-time earning item for.
    
5.  On the **Earnings** subtab, from the dropdown list, select the earning item.
    
6.  Click **Add**.
    
7.  Click **Save**.
    
    Note:
    
    Make sure you recalculate the payroll batch after making these changes.
    

### Related Topics

-   [Including an Employee in Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html)
-   [Decreasing Elective Deferral Limits for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162731062157.html)
-   [Setting up Direct Deposit for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N926100.html)
-   [Setting up Deductions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924665.html)
-   [Setting up Company Contributions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924823.html)
-   [Setting up Accrued Time for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924963.html)
-   [Taxes and Jurisdiction Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556740089.html)
-   [Updating Payroll Items for Multiple Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N925941.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
