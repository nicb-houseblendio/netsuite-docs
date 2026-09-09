---
id: "section_N914230"
type: "section"
title: "Paying Expenses on Employee Paychecks with Payroll"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Expense Reports and Purchase Requests > Expense Reporting > Paying Expenses on Employee Paychecks with Payroll"
parent: "section_N907845"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914230.html"
anchors: ["bridgehead_N914326", "bridgehead_N914370", "bridgehead_N914500", "subsect_1528472193", "bridgehead_N914587"]
sha256: "4288a743f77ec06fe72b7e69f1a708965f92c19f4fc622140428b92b3bb3be5b"
---

If you use SuitePeople U.S. Payroll, you can choose to pay employees' expenses on their regular paychecks instead of paying them through accounts payable. When you use SuitePeople U.S. Payroll to pay expenses, you pay the full amount of the expense report. You can partially pay an expense report, or pay an expense report on a date other than the regular pay date. To do this, pay expenses by accounts payable. To pay expenses by accounts payable, go to Transactions > Pay Bills.

To pay expenses on employee paychecks, complete the following tasks:

1.  [Setting the Pay Expenses on Paychecks Preference](#bridgehead_N914326)
    
2.  [Creating an Earning:Expense Payroll Item](#bridgehead_N914370)
    
3.  [Adding an Expense Payroll Item to an Employee Record](#bridgehead_N914500)
    
4.  [Updating Payroll Information](#subsect_1528472193)
    
5.  [Creating a Payroll Batch that Uses the Pay Expenses Option](#bridgehead_N914587)
    

Note:

When you pay expenses on employee paychecks, note the following. In the general ledger, the default payable account for expense reports is debited, and the payroll funding account is credited. For more information about default payable accounts, see [Setting Default Payable Accounts for non-OneWorld Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913502.html#subsect_1528469712).

## Setting the Pay Expenses on Paychecks Preference {#bridgehead_N914326}

#### To set the Pay Expenses On Paychecks preference:

1.  Go to _Setup > Payroll > Set Up Payroll_.
    
2.  Check the **Pay Expenses on Paychecks** box.
    
3.  Click **Save**.
    

After you enable the preference, you need to create a new payroll item.

## Creating an Earning:Expense Payroll Item {#bridgehead_N914370}

#### To create or edit an Earning:Expense payroll item:

1.  Go to _Lists > Employees > Payroll Items_.
    
    -   To create a new payroll item, click New.
        
    -   To edit an existing payroll item, click **Edit** next to the payroll item you want to edit.
        
2.  If you have a NetSuite OneWorld account, select a subsidiary from the **Subsidiary** list.
    
3.  From the **Item Type** list, select **Earning:Expense**.
    
4.  In the **Item Name** field, enter a name for the earning item.
    
5.  From the **Expense Account** list, choose any expense account. The expense account that you choose here doesn't determine the expense account that is debited for the reimbursement.
    
6.  From the **Pay Code** list, select **Nontaxable Reimbursement**.
    
7.  If necessary, select a **Report Section**.
    
8.  Click **Save**.
    

Earning:Expense items don't affect an employee's gross pay. They're added to the net pay. In addition, expense items don't appear on the employee's W-2.

Next, you need to add the expense payroll item to the employee record.

## Adding an Expense Payroll Item to an Employee Record {#bridgehead_N914500}

#### To add an expense payroll item to an employee record:

1.  Go to Lists > Employees > Employees.
    
2.  Click **Edit** next to the employee name.
    
3.  On the employee record click the **Payroll** subtab.
    
4.  Click the **Earnings** subtab.
    
5.  From the **Earnings** list, select the expense payroll item.
    
6.  Click **Add**.
    
7.  Click **Save**.
    

Add the expense payroll item to all employee records. For more information, see [Including an Employee in Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html).

When an employee submits an expense report and it's approved, you can now pay the expense report when you process payroll.

## Updating Payroll Information {#subsect_1528472193}

After you create the Earning:Expense payroll item and add the item to employee records, you must update payroll information. For more information, see [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html).

## Creating a Payroll Batch that Uses the Pay Expenses Option {#bridgehead_N914587}

After you complete the tasks above, you can pay the expense in a payroll batch.

#### To pay expenses on checks in a payroll batch:

1.  Go to Transactions > Employees > Create Payroll.
    
2.  Create the payroll batch. For more information, see [Creating a Payroll Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N947366.html).
    
3.  On the Payroll Run page, verify that the **Pay Expenses** box is checked.
    
4.  Verify that the employees you want to pay are included in the payroll.
    
5.  Click **Calculate**.
    
6.  When the calculation is complete, on the **Complete** subtab, click **View** next to a paycheck.
    
7.  Click the **Expenses** subtab.
    
8.  Verify that the expense appears on the paycheck.
    

After you have verified the information for the payroll batch, you can commit it. For more information, see [Committing a Payroll Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4791611139.html).

### Related Topics

-   [Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908140.html)
-   [Employee Access to Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908637.html)
-   [Enter an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N911232.html)
-   [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html)
-   [Editing an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550694498.html)
-   [Deleting an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746063133.html)
-   [Rejecting an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751910971.html)
-   [Corporate Card Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531259544.html)
-   [Reviewing Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913094.html)
-   [Giving Accounting Approval for Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913502.html)
-   [Giving an Employee Access to Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914882.html)
-   [Notifying a Supervisor or Approver About Required Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N910874.html)
-   [Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907845.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
