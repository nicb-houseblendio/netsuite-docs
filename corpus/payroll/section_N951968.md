---
id: "section_N951968"
type: "section"
title: "Creating a Payroll Reversal"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Transactions > Payroll Reversals and Adjustments > Creating a Payroll Reversal"
parent: "section_N951824"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951968.html"
anchors: ["procedure_N952007"]
sha256: "19d1fa11da65595d9f7618e933b38d086b570dddcf3576310ab29f91ed1977a7"
---

To reverse disbursements associated with a previously committed paycheck, you should create payroll reversals.

When you submit a payroll reversal, NetSuite creates a journal entry. This journal entry includes transaction lines detailing the reversal of all of the funds from the original paycheck. Reversed paychecks reduce your tax liability. Previously funded but unpaid liabilities can be refunded to you. If some or all of the liabilities incurred by the paycheck have already been paid, you can receive refunds directly from the agencies.

The check date of the paychecks you are reversing determines when a payroll reversal occurs:

-   Check dates in the past or the date that you create the payroll reversal reverse the payroll on the day you create the reversal.
    
-   Check dates in the future reverse the payroll on the same date in the future.
    

Note:

Amounts funded to cover direct deposits and service-printed checks can be refunded if the reversal is made before they are completed.

Important:

Payroll reversals cannot retrieve funds from employee accounts. You must collect any overpaid amount from an employee.

#### To create a payroll reversal: {#procedure_N952007}

1.  Go to _Transactions > Employees >Create Payroll > List_.
    
2.  On the Payroll Batches page, you can add a filter to show only payroll batches that are committed. To filter the Payroll Batches list by committed status:
    
    1.  Click **Customize View**.
        
    2.  In the **Results** subtab, add **Status** to the list.
        
    3.  In the **Available Filters** subtab, add **Status** to the list.
        
    4.  Click **Save**.
        
    5.  In the Status filter list, select **Committed**.
        
3.  Click **View** next to the payroll batch that contains the paycheck to be reversed.
    
4.  On the **Paychecks** subtab, click **View** next to the paycheck to be reversed.
    
5.  Click **Reverse**.
    
    In the case of a funded payroll or a payroll run in a previous quarter, reversing a paycheck incurs fees. If fees apply, consider correcting this payroll with an adjustment to your next standard payroll run. For more information, see [Creating Payroll Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952992.html).
    
6.  On the Voiding Journal page, click **Save**.
    
    Note:
    
    The system generates a journal entry. The Voiding Journal appears on the List of Journal Entries after you save the transaction.
    
    Important:
    
    You must commit all payroll reversals before your next payroll run. For information, see [Committing Payroll Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952877.html).
    
7.  On the Payroll Batch page, click **Commit**.
    

After you reverse a paycheck, NetSuite no longer lists it in the Reconciliation Detail report or on the Reconcile Bank Statement page. In addition, the bank account register does not display the Cleared (Clr) box or link in the Reconciled Date column for the voided paycheck.

### Related Topics

-   [Committing Payroll Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952877.html)
-   [Creating Payroll Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952992.html)
-   [Payroll Reversals and Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951824.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
