---
id: "section_N924665"
type: "section"
title: "Setting up Deductions for an Employee"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Setup for Employees > Setting up Deductions for an Employee"
parent: "section_N921632"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924665.html"
anchors: ["procedure_N924689", "section_4775099652"]
sha256: "545886f9afd46dc6e9509fb8fe69450e291d04a34812f6f59277f414fbfa5a27"
---

For each employee included in payroll, you can add deduction payroll items to their record.

You might need to create payroll deduction items before you can select them for employees. For information, see [Payroll Items Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930985.html).

#### To set up deductions for an employee: {#procedure_N924689}

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the employee's name.
    
3.  Click the **Payroll** subtab, then click the **Deductions** subtab.
    
4.  In the **Deductions** field, choose one of the payroll items you set up for deductions.
    
    For example, you might have a payroll item called 401(k).
    
5.  In the **Rate** field, enter the deduction per pay period for this individual as a dollar amount or percentage.
    
    For example, you might enter 60 for sixty dollars or 15% for fifteen percent.
    
6.  In the **Limit** field, enter a limit if one applies.
    
    For example, you could enter 10,500 as the annual limit for the employee's 401(k) deductions.
    
7.  Click **Add**.
    
8.  Add more deduction items as needed.
    
9.  Click **Save**.
    

## Setting up Negative Deductions for an Employee {#section_4775099652}

To fix an incorrect deduction on a previous paycheck, use a negative deduction to add it back to an employee's earnings. A negative deduction automatically calculates the taxes. The negative deduction feature complies with all federal, state, and local taxable wage rules. This feature works if it doesn't create a negative paycheck. If needed, enter a negative amount on the Create Payroll page and review it before you commit the payroll batch.

Tip:

If you need to adjust a pre-tax deduction from a previous quarter, make an adjustment instead of using a negative deduction.

Negative deductions can be used for these pre-tax deductions:

-   Cafeteria Contribution - FSA: Adopt. Assist
    
-   Cafeteria Contribution - FSA: Dependent Care
    
-   Cafeteria Contribution - FSA: Health Care
    
-   Cafeteria Contribution - POP
    
-   Cafeteria Contribution - Medial Care Premiums
    
-   Commuter Check
    
-   401(K) Contribution
    
-   401(K) Catch-up
    
-   403(b) Contribution
    
-   403(b) Catch-up - After the Age Limit
    
-   403(b) Catch-up - With 15 Years of Service
    
-   Government Employee Deferred - 457(b)
    
-   Government EE 457(b) - Catch-Up Standard
    
-   SEP Contribution - 408(k)(6)
    
-   SEP 408(k)(6) - Catch-Up
    
-   Simple 408(p) Contribution
    
-   Simple 408(p) Catch-Up
    

Negative deductions should not be used for the Cafeteria Contribution - HSA pretax deduction.

#### To set up a negative deduction for an employee:

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the employee's name.
    
3.  Click the **Payroll** subtab, then click the **Deductions** subtab.
    
4.  In the **Deductions** field, choose from a list of payroll items that are set up for negative deduction.
    
    Note:
    
    If you allocate the negative deduction as a pretax deduction the system adds the amount to the taxable wage base. If you allocate it as an after-tax deduction the system treats it as an additional earning item with no tax implications.
    
5.  In the **Rate** field, enter the negative deduction for the pay period as a dollar amount or percentage.
    
6.  Enter the effective and expiration dates for the payroll item. The system checks these dates against the payroll period end date to see which items are affected.
    
7.  Click **Add**.
    
8.  Click **Save**.
    

When you create a payroll batch, the negative deduction is calculated as a reimbursement.

### Related Topics

-   [Including an Employee in Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html)
-   [Decreasing Elective Deferral Limits for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162731062157.html)
-   [Setting up Direct Deposit for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N926100.html)
-   [Setting up Earnings for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924353.html)
-   [Setting up Company Contributions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924823.html)
-   [Setting up Accrued Time for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924963.html)
-   [Taxes and Jurisdiction Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556740089.html)
-   [Updating Payroll Items for Multiple Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N925941.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
