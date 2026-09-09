---
id: "section_N926100"
type: "section"
title: "Setting up Direct Deposit for an Employee"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Setup for Employees > Setting up Direct Deposit for an Employee"
parent: "section_N921632"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N926100.html"
anchors: ["procedure_N926127"]
sha256: "6aaba38b5ffba36be7fd4135903565d7a46d18857ab73c15eb1ac5734e6d25ec"
---

You can set up direct deposit for employees by entering their bank account information about their records. You can also have employees set up their own direct deposit information. For more details, see [Enabling Employees to Update Direct Deposit Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511534973.html).

#### To set up direct deposit for an employee: {#procedure_N926127}

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee that you want to set up for direct deposit, click **Edit**.
    
3.  On the employee record, click the **ACH/Direct Deposit** subtab.
    
4.  Check the **Use Direct Deposit** box.
    
5.  In the **Accounts** table, add bank accounts for the employee:
    
    1.  Check the **Net Account** box to indicate that the net paycheck balance should be deposited in this account.
        
        For example, an employee's check amount is net pay of $1,200.00. The employee record lists two direct deposit accounts, one **Savings** account showing an amount of $200.00, and one Net account. The transaction will show a deposit of $200.00 into the savings account, and the balance, $1,000.00, is deposited into the Net account.
        
        For more examples of Direct Deposit payroll transactions, see [Printing Direct Deposit Vouchers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951476.html).
        
    2.  If the account is a savings account, check the **Savings Account** box.
        
    3.  To run a prenote test transmission on the account, clear the **Prenoted** box.
        
        To process direct deposit transactions to this account without a prenote test, check the **Prenoted** box. You should run a prenote test for each account.
        
    4.  In the **Bank Name** column, enter the name of the employee's bank name.
        
        You can enter up to 31 characters in this field.
        
    5.  In the **Routing Number** column, enter the 9-digit routing number for the employee's bank account.
        
        Note:
        
        SuitePeople U.S. Payroll doesn't support international direct deposit yet. You may consider using pay cards to pay employees with international bank accounts. Be aware that international transit numbers may require a specific number pattern. For example, Canadian transit numbers are regulated by the Canadian Payments Association. The number pattern for Electronic Fund Transactions (EFT) is 0YYYXXXXX. The first four digits represent the transit number where YYY is an Institution Number. The last five digits represent the Branch Number. The last digit of the Branch Number, with few exceptions, indicates the geographical location of the branch.
        
    6.  In the **Account Number** column, enter the employee's bank account number.
        
        You can enter up to 20 characters in this field.
        
    7.  In the **Amount** field, enter how much should go into this bank account.
        
        For example, an employee requests that $200.00 from every paycheck is deposited into their savings account. Enter 200 in the amount field next to the savings account information.
        
        If the account is the **Net Account**, leave this field blank.
        
    8.  To save the bank account on the employee record, click **Add**.
        
        Repeat this process to add multiple accounts for this employee.
        
6.  Click **Save**.
    

If a direct deposit to an employee's account fails and the error cannot be resolved, note the following. NetSuite changes the paycheck from direct deposit to Employer Paid and refunds the amount that initially funded the employee's direct deposit. The refund does not trigger a correcting journal entry. For this reason, when your company receives the refund, you must make a manual journal entry in your Payroll Funding Account. For more information, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).

### Related Topics

-   [Including an Employee in Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html)
-   [Decreasing Elective Deferral Limits for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162731062157.html)
-   [Setting up Earnings for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924353.html)
-   [Setting up Deductions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924665.html)
-   [Setting up Company Contributions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924823.html)
-   [Setting up Accrued Time for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924963.html)
-   [Taxes and Jurisdiction Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556740089.html)
-   [Updating Payroll Items for Multiple Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N925941.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
