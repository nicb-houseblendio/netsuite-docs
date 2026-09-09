---
id: "section_N1122601"
type: "section"
title: "Commission Preferences"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Commission Preferences"
parent: "chapter_N1122333"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1122601.html"
anchors: []
sha256: "69a9433a6665f6d03c5ab73ad5b341c532ab7c94d4b4bae620a6df7df502b707"
---

An administrator can set the following company commissions preferences at _Setup > Sales > Sales Management > Commissions (Administrator)_:

-   **Commissions Paid By Default On** - Select when commissions are eligible to be paid:
    
    -   **Billings/Bookings** - When the sales transaction is invoiced. In the case of commission based on alternate sales amounts (ASA), when sales orders are booked and approved.
        
    -   **Collections** - When payment is received partially at billing/booking and partially upon receipt of payment.
        
    
    Note:
    
    If you change this preference it does not affect existing schedules. For more information, see [Commission Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html).
    
    Note:
    
    Customer payments and deposits do count as collections at the time they are applied to the invoice, regardless of the application date. The date of the invoice determines whether it is in plan, regardless of the payment date. The payment date (for collections eligibility) affects when the commission is eligible to be paid, regardless if it is backdated.
    
-   **Allow Overwrite in Schedules** - Check this box if you want to overwrite commission schedules when commissions become eligible.
    
    If you do not check this box, the **Eligible Amount** field on commission schedules is read-only. It shows the eligibility selected in the **Commissions Paid By Default On** field.
    
-   **Default ASA Collections Eligibility Type** - Select how to define the default commission eligibility option on ASA-based schedules:
    
    -   **First In** - Select this option to consider the amount paid on an order as fulfilling the ASA of a transaction. This option ensures commission eligibility.
        
    -   **Percent of Order** - Select this option if you want the alternate sales amount, collections-based commission schedules, to determine eligibility of calculated commissions. Commissions are based on the proportion of cash collected against the sales order amount, rather than the ASA total.
        
    -   **Whichever Is Greater** - Select this option to use the greater of the two preceding amounts when NetSuite determines commission eligibility.
        
    -   **Whichever Is Less** - Select this option to use the lesser of the two preceding amounts when NetSuite determines commission eligibility.
        
    
    For example, a sales order is entered in the amount of $1,000. The alternate sales amount for the order is $500. The sales rep on the order receives commission of 10% of ASA, which makes the calculated commission on the order $50. A payment of $400 is received on the order.
    
    **First In** - The $400 payment counts toward the ASA, which makes 80% ($400/$500), or $40, eligible for commission payment.
    
    **Percent of Order** - The $400 payment is 40% of the order total; so 40% or $20, of the calculated commission is eligible.
    
    **Whichever Is Greater** - Forty dollars is eligible because counting the payment toward the ASA gives a greater eligible amount.
    
    **Whichever Is Less** - Twenty dollars is eligible because counting the payment as a percentage of the order total gives a smaller eligible amount.
    
    For more information, see [Basing Commission on ASA](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050405.html).
    
-   **Commission Eligibility Period** - Enter the number of days to wait after the sale is made or billed before NetSuite pays commission to sales reps.
    
-   **Calculate Commissions on Shipping Items** - Check this box to include shipping costs when NetSuite calculates a transaction's commission amount. Note that this setting works differently depending on the basis for the commission:
    
    -   If the basis for the commission is Inventory Total Profit, NetSuite bases the commission on the gross profit. It does not base the commission on the profit minus the shipping costs.
        
    -   If the basis for the commission is Sales, NetSuite bases the commission on the transaction amount.
        
    
    Note:
    
    When you check this box, NetSuite applies this preference to new transactions. NetSuite does not change commission amounts on previously entered transactions.
    
-   **Require Accounting Approval of Employee Commissions** - Check this box to require your accounting department to approve employee commissions and payments.
    
    Note:
    
    NetSuite requires supervisor authorization of commissions, regardless if you use this preference.
    
-   **Require Accounting Approval of Partner Commissions** - Check this box to require your accounting department to approve partner commissions and payments.
    
-   **Maximum Commission Brackets** - Enter the maximum number of brackets to include in commissions schedules.
    
    Warning:
    
    If you decrease this number after you create commission schedules, you may lose columns of data in the existing schedules.
    
-   **Default Employee Commissions Expense Account** - Select the default expense account to which you want employee commission payments to post.
    
    You can select a different account on the commission transaction.
    
    Do not fill this field if you do not want a default account.
    
-   **Default Partner Commissions Expense Account** - Select the default expense account to which you want partner commission payments to post.
    
    You can select a different account on the commission transaction.
    
    Do not flil this field if you do not want a default account.
    

An administrator can choose how the sales effective date is set on refunds and credit memos. Go to _Setup > Sales > Preferences > Sales Preferences (Administrator)_. Check the **Default Sales Effective Date to Linked Sales Effective Date** box , and then click **Save**.

You can choose to pay commissions on your employees regular paychecks if you use SuitePeople U.S. Payroll. To set this preference, go to _Setup > Payroll > Setup Tasks > Set Up Payroll (Administrator)_. Check the **Pay Employee Commissions on Paychecks by Default** box, and then click **Save**.

Company commission preferences apply to everyone with access to your NetSuite account.

Important:

Sales transaction pages such as Sales Order, Invoice, Credit Memo, Cash Sales, Cash Refunds, and Return Authorizations have an Exclude Commissions box. If a user checks this box, NetSuite excludes the transaction and its subordinate transactions from inclusion in all commission calculations. For example, a user checks this box on a sales order. NetSuite excludes the sales order and subsequent invoice from all commission calculations for all sales people.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Employee Commission Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146679.html)
-   [Authorizing Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1149753.html)
-   [Approving and Rejecting Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1151300.html)
-   [Paying Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1153252.html)
-   [Commission Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1154636.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
