---
id: "section_N951476"
type: "section"
title: "Printing Direct Deposit Vouchers"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Transactions > Print Payroll Checks or Vouchers > Printing Direct Deposit Vouchers"
parent: "section_N955656"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951476.html"
anchors: ["procedure_N951499", "bridgehead_N951579"]
sha256: "020f0f4cd0e50cc65a16c856e95764f809f4cfd8e273d9d26f41505d1112bf51"
---

When you process direct deposit payroll transactions, checking the To Be Printed box generates vouchers that detail payment information for that pay period. Do not check this box if you use the Service Printed Checks and Stubs feature and intend the Payroll Service to print checks and stubs.

Direct deposit vouchers should be printed on plain paper or non-negotiable check stock.

#### To print direct deposit vouchers: {#procedure_N951499}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  On the Print Checks and Forms page, click **Direct Deposit Voucher**.
    
3.  In the **Account** field, select an account to display a list of its associated direct deposit transactions.
    
4.  In the displayed list, mark the voucher or vouchers that you want to print.
    
5.  Click **Print**.
    

Direct Deposit Vouchers show the dollar amount of funds transferred into each prenoted employee account. A prenote is a test to ensure that the bank routing information is accurate and the Direct Deposit transmission can be properly completed. Employee accounts are marked Prenoted on the Direct Deposit subtab of the Employee record.

After you print a direct deposit voucher, it disappears from the list. You can reprint a direct deposit voucher by going to _Transactions > Employees > View Individual Paychecks_. Click **Print** next to the paycheck you want to print.

Note:

Before reprinting, make sure the Default Check Type of your printing preference is set to Voucher. If Standard is selected, pay statements for employees with direct deposit will display a zero value instead of the correct amount. For the steps, see [Setting Check Printing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1545526.html).

## Direct Deposit Payroll Transaction Examples {#bridgehead_N951579}

**Example 1**: Post a direct deposit to one prenoted net account.

**Result**: One direct deposit voucher queues to print.

The voucher shows the net amount of the deposit ($1200.00) to the employee's account Wachovia 1234567.

**Example 1 voucher**:

![Screenshot of a Direct Deposit Voucher to one prenoted net account.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/EmployeeManagement/Payroll/voucher1.png)

**Example 2**: Post direct deposits to two accounts - one prenoted savings account and one prenoted net account.

**Result**: One direct deposit voucher queues to print.

The voucher displays the net amount of the deposit ($1200.00) to the employee's two accounts:

-   $200.00 is deposited to savings account Wachovia 987654.
    
-   $1000.00 is deposited to net account Wachovia 1234567.
    

**Example 2 voucher**:

![Screenshot of a Direct Deposit Voucher to one prenoted savings account and one prenoted net account.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/EmployeeManagement/Payroll/voucher2.png)

**Example 3**: Post a direct deposit to one prenoted savings account and one non-prenoted net account.

**Result**: One paycheck queues to print and one prenote test posts for the net account.

As in the below example, the paycheck shows:

-   Net Pay for this period is $1200.00.
    
-   $200.00 is direct deposited to the prenoted savings account Wachovia 987654.
    
-   $1000.00 is the amount on the printed paycheck.
    

**Example 3 paycheck**:

![Screenshot of a Direct Deposit Voucher to one prenoted savings account and one non prenoted net account.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/EmployeeManagement/Payroll/voucher3.png)

### Related Topics

-   [Printing Paychecks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N950744.html)
-   [Print Payroll Checks or Vouchers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N955656.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
