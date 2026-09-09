---
id: "section_N953245"
type: "section"
title: "Recording Third-Party Sick Pay Payments"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Transactions > Recording Third-Party Sick Pay Payments"
parent: "chapter_N945815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N953245.html"
anchors: ["procedure_N953431"]
sha256: "45dd25b7487d4a1b5a3ab1bb543651b46d6b9220620bfe03169b9a2d2d089e45"
---

Many companies provide short and long-term disability benefits to their employees. Generally, companies purchase these benefit plans from third-party providers that administer the benefits, such as insurance companies.

The third-party provider:

-   Makes payments to employees with disabilities
    
-   Withholds Federal taxes:
    
    -   Income
        
    -   FICA (Federal Insurance Contribution Act)
        
    -   Medicare
        
    -   FUTA (Federal Unemployment Tax Act)
        
-   Reports data to companies as required to prepare employees' annual W-2 forms
    

By creating Third-Party Sick Pay payroll items, you can enter the data that you receive from the third-party provider into SuitePeople U.S. Payroll. This ensures that employees receive the appropriate payments and W-2 information.

If an employee elects to receive non-taxable disability payments, NetSuite reports these payments on the employee's W-2, but does not withhold taxes. If an employee elects to receive taxable disability payments, the third-party provider withholds income tax, FICA, and Medicare contributions from the employee's payments.

The following guidelines can help you process Third-Party Sick Pay:

-   Enter the Third-Party Sick Pay taxable gross, federal income tax (if withheld), employee social security, and Medicare.
    
-   Do not enter any amount in the Taxable Wage Base and Taxed Wage Base fields.
    
-   Do not enter any employer taxes.
    
-   Do not enter any state or local taxes.
    
-   Process each employee's benefit check as a separate adjustment. You cannot process all employees' checks at the same time.
    
-   Process these entries as adjustments. Process Third-Party Sick Pay adjustments separate from other entries.
    
-   Do not process third-party sick pay adjustments with your regular payroll. Your payroll will not process with this error condition.
    
-   Do not pay employees third-party sick pay with a check or direct deposit. The employee has already received the money from the third party payer.
    
-   **Do not process any other types of earnings or deduction code entries with your Third-Party Sick Pay adjustments.**
    

Additional notes:

-   To properly report the information, including the adjustment on Form 941 line 7b, you must follow processing instructions for third-party sick pay.
    
-   If you enter any amount in the Taxable Wage Base and Taxed Wage Base fields, note the following. After you commit the payroll adjustment, the Social Security and Medicare tax amount fields have a value of zero.
    

Note:

Only user roles that include **Process Payroll** with the **Full** option can commit a payroll batch. These user roles include Payroll Manager: Full, and Payroll Setup: Full. For more information, see [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html), [Showing Role Permission Differences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292157.html), and [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

#### To record third-party sick pay payments: {#procedure_N953431}

1.  Create two payroll earning items: Third-Party Sick Pay Taxable and Third-Party Sick Pay Non-Taxable.
    
    You can use the most appropriate **Payroll Item Type**, such as **Earning: Salary** or **Earning:Wage**. For more information, see [Creating Payroll Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556724572.html).
    
2.  Assign a third-party sick pay payroll earning item to the employee who receives the sick pay.
    
    Refer to [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html).
    
3.  On the Payroll Adjustment page, on **Earnings** subtab, create a payroll adjustment using a third-party sick pay payroll earning item.
    
    On the **Withholding** subtab enter amounts for:
    
    -   Employee's portion of Social Security
        
    -   Federal tax withholding
        
    -   Medicare employee portion
        
    
    For more information, refer to [Creating Payroll Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N952992.html).
    
4.  Save the payroll adjustment.
    
    NetSuite calculates the required tax amounts.
    
5.  To submit the adjustment payroll for processing, on the Payroll Batch page, click **Commit**.
    
    For more information, refer to [Committing a Payroll Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4791611139.html).
    

### Related Topics

-   [Processing Payroll Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N947159.html)
-   [Searching for Paychecks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N950964.html)
-   [Payroll Dashboard Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544802669.html)
-   [Print Payroll Checks or Vouchers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N955656.html)
-   [Payroll Reversals and Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N951824.html)
-   [Payroll Transaction Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N953616.html)
-   [Making Payroll Liability Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N954201.html)
-   [Complete Quarterly or Yearly Payroll Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N954521.html)
-   [Allocating Paycheck Expenses to Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N955773.html)
-   [Payroll Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N945815.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
