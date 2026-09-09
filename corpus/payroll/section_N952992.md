---
id: "section_N952992"
type: "section"
title: "Creating Payroll Adjustments"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Transactions > Payroll Reversals and Adjustments > Creating Payroll Adjustments"
parent: "section_N951824"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952992.html"
anchors: ["procedure_N953052"]
sha256: "fe0af9b673b8750dea413f9eb3787c9e18787bf5eb2ad1eb419eb7403e37ea5e"
---

To make changes to previously committed paychecks, you should create payroll adjustments. These adjustments can be either positive or negative, depending on the situation.

Payroll adjustments never directly affect company disbursement (bank) accounts or employee accounts. Instead, adjustments balance expenses recorded on your company's accounting ledgers. You must collect incorrect payments directly from employees.

Note:

Only those user roles that include **Process Payroll** with the **Full** option can commit a payroll. These user roles include Payroll Manager: Full, and Payroll Setup: Full. For more information, see [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html), [Showing Role Permission Differences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292157.html), and [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

**NetSuite automatically funds any increase in liabilities from your Payroll Funding Account and files amendments with tax agencies.**

To reverse disbursements associated with a previously committed paycheck, you should create a payroll reversal. For more information, see [Creating a Payroll Reversal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951968.html).

#### To create a payroll adjustment: {#procedure_N953052}

1.  Go to _Transactions > Employees > Create Payroll Adjustment_.
    
2.  In the **Payee** field, select the employee for whom you are entering the adjustment.
    
3.  If you track departments, classes, or locations, select the appropriate information for those fields.
    
4.  In the **Pay Period Ending** field, select the date for the pay period in which these funds were originally disbursed.
    
5.  In the **Post Date** field, enter the date of the payroll that includes the adjustment.
    
6.  In the **Posting Period** field, select the fiscal period to which NetSuite must post the adjustment.
    
    Note:
    
    You cannot post to a locked accounting period.
    
7.  If you have a NetSuite OneWorld account, select a subsidiary from the list in the **Subsidiary** field.
    
8.  Enter the amount of the adjustment. This amount can be either positive or negative.
    
9.  Enter a memo for this adjustment.
    
10.  Select an account to use to fund this transaction.
     
     You must use the **Payroll Funding Account** you selected on the Set Up Payroll page.
     
11.  On the **Earnings**, **Withholdings**, **Deductions**, and **Company Contributions** subtabs, enter amounts for the payroll items related to the adjustment.
     
     Note:
     
     If you need to reduce a value, enter a negative amount.
     
     NetSuite automatically checks the corresponding box.
     
     In the **Amount** field, NetSuite calculates the total for the adjustment based on the amounts entered.
     
12.  Click **Save**.
     
     NetSuite calculates the taxes associated with this adjustment and updates the employee's payroll history.
     
13.  Click **Commit** to commit the payroll batch.
     

To review a list of payroll adjustments, on the Payroll Adjustment page, click List. On the list, click the View or Edit links to review individual adjustment records.

### Related Topics

-   [Creating a Payroll Reversal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951968.html)
-   [Committing Payroll Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952877.html)
-   [Payroll Reversals and Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951824.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
