---
id: "section_N1150000"
type: "section"
title: "Authorizing Employee Commission in Bulk"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Authorizing Employee Commission > Authorizing Employee Commission in Bulk"
parent: "section_N1149753"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1150000.html"
anchors: ["procedure_N1150052"]
sha256: "3bc4c9b9e207999b4b8275c989fba27fe4c7d6e93dfe1b3c28a5f98f39a1c1da"
---

After you assign a commission plan to an employee, NetSuite generates a commission amount when a sales transaction is created that meets the commission criteria. After NetSuite generates a commission amount, it must be authorized by a supervisor.

Authorization verifies the commission amount, creates a commission payable transaction, and may also give accounting approval to cut a payment check.

Bulk employee commission transactions source department, class, and location from employee records.

#### To authorize bulk commission transactions: {#procedure_N1150052}

1.  Go to _Transactions > Commissions > Authorize Employee Commissions (Administrator)_.
    
    The Authorize Commissions page displays a list of commission transactions pending authorization.
    
    Sales managers see only commissions for their subordinate sales reps.
    
2.  In the **Pay Commissions Using** field, select whether you want to pay commission through payroll or through accounts payable.
    
3.  Enter or pick a date. NetSuite inserts today's date by default for this commission, but you can change it. The date you enter determines the range in which this transaction appears on the Accounts Payable Register.
    
4.  Select the period to which you want these commission transactions to post.
    
5.  Check the **Accounting Approval** box to give accounting approval for these commission transactions.
    
    Commission transactions with accounting approval can be paid through checks.
    
6.  In the **Account** field, select the account to which you want these commission transactions to post.
    
    This field appears only if you are paying the commission through accounts payable.
    
    The balance for this account is shown in the **Balance** field.
    
7.  Select the expense account used by these commission transactions.
    
    This field appears only if you are paying the commission through accounts payable.
    
8.  In the **Date Eligible** field, enter a date to filter commission transactions by the date they became eligible.
    
    You can use this date filter to show only the transactions for the month you authorize commission.
    
    This date defaults to the most recent date for eligible transactions.
    
    For example, if you have a commission eligibility period of 15 days and today's date is February 28, the **Date Eligible** field defaults to February 13. Only transactions that are eligible on the date you authorize commissions are shown.
    
9.  In the **Sales Rep** field, enter the name of a sales rep to filter the commission transactions for the particular rep.
    
10.  In the **Select** column, check the box next to one or more commission amounts to authorize, or click **Mark All**.
     
11.  Check the **Accounting Approval** box (if available) to approve and authorize commissions at the same time.
     
12.  Click **Authorize**.
     

The Process Status page displays the status of the commission authorization process while the process runs. To view this page, go to Transactions > Commissions > Authorize Employee Commissions > Status. Information that displays includes the submission ID, process type, the status of the commission payment, and percent complete. It also displays any processing errors, the date created, and the name of the creator. If the status is **Complete**, click the link to open the Processed Commissions page. On this page you can obtain the name of the employee receiving the commission, status, and transaction number. You can also obtain currency, amount in foreign currency, amount in base currency, and any error messages. If you click the **Transaction Number** link, you can access the individual commission record.

Note:

You cannot authorize commissions for employees whose commissions are currently being authorized.

The next step depends upon your set preference to use accounting approval for commissions and to pay commissions. You can require separate accounting approval. You can choose either to pay commissions to employees on their paychecks, or pay commissions on a separate check.

Sales managers with accounting approval permissions can both authorize and approve a commission transaction at the same time.

After you authorize a commission transaction, one of the following occurs:

-   **With Accounting Approval and Use Payroll both off** - The commission appears as a payable transaction at Transactions > Payables > Pay Bills.
    
-   **With Accounting Approval and Use Payroll both on** - The commission appears in the accounting approval queue.
    
-   **With Accounting Approval on and Use Payroll off** - The commission appears in the accounting approval queue.
    
-   **With Accounting Approval off and Use Payroll on** - The commission appears as a payment on the employee's paycheck at Transactions > Process Payroll.
    

To set your preference to require separate accounting approval on commissions, go to _Setup > Sales > Sales Management > Commissions (Administrator)_. Check the **Require Accounting Approval of Employee Commissions** box, and then click **Save**.

-   To pay commissions on paychecks, you must use SuitePeople U.S. Payroll. For more information, see [SuitePeople U.S. Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1538679887.html).
    
    Next, go to _Setup > Payroll > Setup Tasks > Set Up Payroll (Administrator)_. On the Preferences subtab, check the Pay Commissions on Paychecks by Default box. Click Save.
    
-   If you do not pay commissions on paychecks, approved commission amounts generate a commission payable transaction. Go to _Transactions > Payables > Pay Bills (Administrator)_.
    

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Authorizing Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1149753.html)
-   [Authorizing Individual Employee Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1150571.html)
-   [Viewing the Status of Authorized Employee Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3802855281.html)
-   [Approving and Rejecting Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1151300.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
