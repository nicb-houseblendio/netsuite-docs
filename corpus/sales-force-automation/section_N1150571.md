---
id: "section_N1150571"
type: "section"
title: "Authorizing Individual Employee Commissions"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Authorizing Employee Commission > Authorizing Individual Employee Commissions"
parent: "section_N1149753"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1150571.html"
anchors: ["procedure_N1150618"]
sha256: "00fa67175fe68523896d04549ebd43365cfb9d0fdc57d27d656c309b9528a693"
---

After a commission amount is generated from a sale that meets the commission criteria, it must be authorized by a supervisor.

Authorization verifies the commission amount, creates a commission payable transaction, and may also give accounting approval to cut a payment check.

#### To authorize individual commission transactions: {#procedure_N1150618}

1.  Go to _Transactions > Commissions > Individual Employee Commission (Administrator)_.
    
2.  In the **Employee** field, select the sales rep who will receive the commission.
    
    The **Supervisor** field displays the employee's assigned supervisor.
    
3.  If you pay commissions on payroll, select the commission earning item in the **Commission Item** field.
    
    Set up commission earning items at _Lists > Employees > Payroll Items > New_.
    
4.  In the **Date Eligible** field, enter a date to filter commission transactions by the date they became eligible.
    
    You can use this date filter to show only the transactions for the month you authorize commission.
    
    This date defaults to the most recent date for eligible transactions.
    
    For example, if you have a commission eligibility period of 15 days and today's date is February 28, the **Date Eligible** field defaults to February 13. Only transactions that are eligible on the date you authorize commissions are shown.
    
5.  Accept or enter the date in the **Date** field.
    
6.  If you pay commissions as an expense, select an account for this commission in the **Expense Account** field.
    
7.  In the **Memo** field, enter a memo for this transaction.
    
8.  If you use the Accounting Approval preference, and you can grant accounting approval, check the **Accounting Approval** box to approve payment of this commission.
    
9.  Select a department, class, or location, if you track them.
    
10.  Accept or enter the commission number in the **Commission #** field.
     
     To permit the transaction number to be modified, go to _Setup > Company > Setup Tasks > Auto-Generated Numbers_. Check the **Override** box on the **Transactions** subtab next to **Commission**.
     
11.  Choose the amounts to include on the commission transaction:
     
     -   Check the box next to the commission to include a commission on the **By Transaction** subtab
         
     -   Check the box next to the commission to include a commission on the **By Period** subtab
         
     
     The following columns appear on the **By Transaction** and **By Period** subtabs:
     
     -   **Date Eligible** - The date the commission is eligible, based on the terms of the schedule plus the offset preference
         
         This column appears only on the **By Transaction** subtab.
         
         For example, an order closed on 6/1/2019 has an eligibility schedule based on billings, and the order is invoiced on 6/15/2019. The eligible date is 6/15/2019. If the offset is 5 days, then the eligible date is 6/20/2019.
         
     -   **Calculated Commission** - The amount calculated by the schedule, which is the total payable amount
         
     -   **Previously Authorized** - The amount previously authorized
         
         In view mode, this is the total amount authorized including this transaction
         
     -   **Eligible Amount** - The total eligible amount after the triggering event occurs (billing or collection)
         
         Note:
         
         This amount may differ from the calculated commissions column. For example, if a schedule is based on collections and only half of the payment is received, the eligible amount is half of the calculated amount.
         
     -   **Amount** - The amount authorized by this transaction
         
         -   To enter a commission amount manually, click the **Other Commissions** subtab. Complete the **Memo** and **Amount** fields for the commission
             
             The **Exchange Rate** column displays the currency exchange rate on the date this commission is authorized. The **Foreign Currency Amount** column displays the related commission amount.
             
         -   Click **Add**
             
12.  Click **Save**.
     

The Process Status page displays the status of the commission authorization process while the process runs. To view this page, go to Transactions > Commissions > Authorize Employee Commissions > Status. Information that displays includes the submission ID, process type, the status of the commission payment, and percent complete. It also displays any processing errors, the date created, and the name of the creator. If the status is **Complete**, click the link to open the Processed Commissions page. On this page you can obtain the name of the employee receiving the commission, status, and transaction number. You can also obtain currency, amount in foreign currency, amount in base currency, and any error messages. If you click the **Transaction Number** link, you can access the individual commission record.

Note:

You cannot authorize commissions for employees whose commissions are currently being authorized.

The next step depends upon your set preference to use accounting approval for commissions and to pay commissions. You can require separate accounting approval. You can choose either to pay commissions to employees on their paychecks, or pay commissions on a separate check.

Sales managers with accounting approval permissions can both authorize and approve a commission transaction at the same time.

After you authorize a commission transaction, one of the following occurs:

-   **With Accounting Approval and Use Payroll both off** - The commission appears as a payable transaction at Transactions > Pay Bills.
    
-   **With Accounting Approval and Use Payroll both on** - The commission appears in the accounting approval queue.
    
-   **With Accounting Approval on and Use Payroll off** - The commission appears in the accounting approval queue.
    
-   **With Accounting Approval off and Use Payroll on** - The commission appears as a payment on the employee's paycheck at Transactions > Process Payroll.
    

To set your preference to require separate accounting approval on commissions, go to _Setup > Sales > Sales Management > Commissions (Administrator)_. On the General subtab, check the Require Accounting Approval box, and then click Save.

-   To pay commissions on paychecks, you must use SuitePeople U.S. Payroll. For more information, see [SuitePeople U.S. Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1538679887.html).
    
    Next, go to _Setup > Payroll > Setup Tasks > Set Up Payroll (Administrator)_. On the Preferences subtab, check the Pay Commissions on Paychecks by Default box. Click Save.
    
-   If you do not pay commissions on paychecks, approved commission amounts generate a commission payable transaction. Go to _Transactions > Payables > Pay Bills (Administrator)_.
    

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Authorizing Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1149753.html)
-   [Authorizing Employee Commission in Bulk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1150000.html)
-   [Viewing the Status of Authorized Employee Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3802855281.html)
-   [Approving and Rejecting Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1151300.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
