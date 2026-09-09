---
id: "section_N1153252"
type: "section"
title: "Paying Employee Commission"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Paying Employee Commission"
parent: "chapter_N1122333"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1153252.html"
anchors: ["bridgehead_N1153261", "procedure_N1153376", "subsect_98115355533", "procedure_N1153473", "procedure_N1153603"]
sha256: "8feaaed4c16ead2846f79a7d90d08aafd04b5dc389fa7680e500dcd3fe225cd0"
---

This topic details two methods for paying employee commission.

## Commission Payment Methods {#bridgehead_N1153261}

You can choose one of two methods to pay commissions to employees:

-   On paychecks, commission payments show on the check stub as a payroll earning item.
    
    To pay commissions on paychecks, you must use SuitePeople U.S. Payroll to pay your employees. See [Payroll Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N917379.html).
    
-   On payable checks, NetSuite treats commission payments as an accounts payable transaction.
    

If you use SuitePeople U.S. Payroll, you set your preferences to pay commissions on paychecks.

#### To pay commissions on paychecks: {#procedure_N1153376}

1.  Go to _Setup > Payroll > Setup Tasks > Set Up Payroll (Administrator)_.
    
2.  In the Paychecks section, check the **Pay Employee Commissions on Paychecks by Default** box.
    
    Note:
    
    If you do not check this box, commissions are paid on a separate check as accounts payable transactions. To pay commission through payable checks, first create a journal entry for the payment, and then process the payment. You can process the payment at _Transactions > Payables > Pay Bills_.
    
3.  Click **Save**.
    
    Now you can pay approved commissions at _Transactions > Employees > Create Payroll_.
    
    Important:
    
    You can change the state of the **Pay Employee Commissions on Paychecks by Default** box. However, the method to pay existing commissions transactions depends on the preference state at the time the commission is authorized, not at payment processing.
    
    For example, you check the Pay Employee Commissions on Paychecks by Default box. Then, commission transaction #1 is created and pending authorization. Before you authorize commission #1, you clear the box. Then, commission #2 is created. After you authorize each commission, you pay both commissions on a check separate from the employee's paycheck.
    

## Paying Commissions using Accounts Payable {#subsect_98115355533}

#### To create a bill credit for the commissions payable: {#procedure_N1153473}

1.  Go to _Transactions > Financial > Make Journal Entries (Administrator)_.
    
2.  Choose the posting period and date you want this journal entry to apply to.
    
3.  On the **Lines** subtab, in the **Account** column, select the payables account to pay this commission.
    
4.  In the **Debit** column, enter the commission amount.
    
5.  In the **Name** column, enter the name of the sales rep.
    
6.  Select the appropriate department in the **Department** column.
    
7.  Click **Add**.
    
8.  In the **Account** column, select the bank account for this payment.
    
9.  Click **Add**.
    
10.  Click **Save**.
     

Make a note of the journal entry reference number.

#### To offset the bill credit to commission and process the commission payment: {#procedure_N1153603}

1.  Go to _Transactions > Financial > Make Journal Entries (Administrator)_.
    
2.  Choose the posting period.
    
3.  Select the payable account for this commission.
    
4.  Choose the bank account for this payment.
    
5.  Check the box in the **Pay** column next to the commissions payable.
    
6.  Check the box in the **Pay** column next to the Bill Credit that corresponds to the commissions payable.
    
7.  Click **Save**.
    

NetSuite processes the commission payment and you can print the check for the sales rep.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Setting Up an Employee for Commission Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1153743.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Employee Commission Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146679.html)
-   [Authorizing Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1149753.html)
-   [Commission Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1154636.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
