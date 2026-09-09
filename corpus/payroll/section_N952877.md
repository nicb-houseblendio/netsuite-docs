---
id: "section_N952877"
type: "section"
title: "Committing Payroll Reversals"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Transactions > Payroll Reversals and Adjustments > Committing Payroll Reversals"
parent: "section_N951824"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952877.html"
anchors: ["procedure_N952903"]
sha256: "f1189361334990c92c06a486bc7f15d488751b8a5c8b9cc5e0c33e5999dde097"
---

Important:

Payroll reversals cannot retrieve funds from employee accounts. You must collect any overpaid amount from an employee.

After you create payroll reversals, you must commit them before you run your next payroll.

Uncommitted reversals do not reduce your liability and may result in overpaying a tax agency. In addition, uncommitted reversals do not show on the Pay Payroll Liabilities page or on liability reports. If you commit a payroll reversal after tax liabilities are paid, unapplied payments may display on the Pay Payroll Liabilities page. Unapplied payments are liability payments not associated with checks.

Note:

Only those user roles that include **Process Payroll** with the **Full** option can commit a payroll. These user roles include Payroll Manager: Full, and Payroll Setup: Full. For more information, see [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html), [Showing Role Permission Differences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292157.html), and [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

The following steps help you commit a payroll reversal that was not previously committed.

#### To commit a payroll reversal: {#procedure_N952903}

1.  Go to _Transactions > Employees > Create Payroll > List_.
    
2.  On the Payroll Batches page, you can add a filter to display payroll batches with a specific status. Those statuses are Ready to Commit, Funding Calculated, and Edited. To filter the Payroll Batches list by status:
    
    1.  Click **Edit View**.
        
    2.  In the **Results** subtab, add **Status** to the list.
        
    3.  In the **Available Filters** subtab, add **Status** to the list. Ensure **Show in Filter Region** and **Show as Multi-Select** are enabled.
        
    4.  Click **Save**.
        
    5.  Click **Filters** to open the Status filter list.
        
    6.  Select **Ready to Commit**, **Funding Calculated**, or **Edited**.
        
3.  Click **Edit** next to an uncommitted payroll reversal.
    
    To quickly locate your reversals, click the **Type** column header to sort the list by type and locate Reverse payroll.
    
4.  On the Payroll Batch page, click **Commit**.
    
5.  Repeat these steps until all reversals have been committed.
    

After all of your reversals are committed, go to _Transactions > Employees > Create Payroll_ to create your next payroll.

### Related Topics

-   [Creating a Payroll Reversal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951968.html)
-   [Creating Payroll Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952992.html)
-   [Payroll Reversals and Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951824.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
