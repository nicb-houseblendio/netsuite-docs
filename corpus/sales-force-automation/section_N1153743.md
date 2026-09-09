---
id: "section_N1153743"
type: "section"
title: "Setting Up an Employee for Commission Payments"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Paying Employee Commission > Setting Up an Employee for Commission Payments"
parent: "section_N1153252"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1153743.html"
anchors: ["procedure_N1153787", "procedure_N1153917"]
sha256: "2bbd18ee1b5f66d842a71e5f13936fe6c7ea7f031e30f8365df8bf63194c4fd6"
---

To make commission payments to an employee, you must create a commission earning item. You must then add the item to the record of each employee to whom you want to pay a commission.

Note:

To set up an employee for commission payments, you must use SuitePeople U.S. Payroll to pay your employees. See [Payroll Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N917379.html).

#### To create a commission earning item: {#procedure_N1153787}

1.  Go to _Lists > Employees > Payroll Items > New_.
    
2.  Select **Earning: Commission** from the **Item Type** field.
    
3.  Enter a name for the commission earning item, in the **Item Name** field.
    
4.  Select the expense account to pay the commission.
    
5.  If you use NetSuite OneWorld, select the subsidiary this payroll item relates to.
    
6.  In the **Pay Code** field, select the appropriate pay code. Check the **Withholding** box to determine how the earning is taxed and reported, and whether the item appears on the employee's W-2.
    
7.  Select the report section in which this payroll item should appear on payroll reports.
    
8.  Click **Save**.
    

Next, add the commission earning item to the record of the employees to whom you want to pay a commission.

#### To set up an employee record for commissions: {#procedure_N1153917}

1.  Go to _Lists > Employees > Employees > New (Administrator)_.
    
2.  Click **Edit** next to the employee you want to set up for commission payments.
    
3.  On the employee record, click the **Payroll** subtab.
    
4.  Click the **Earnings** subtab, and then in the **Earnings** field, select the commission earning item you created in the preceding procedure.
    
5.  Click **Add**.
    
6.  Click **Save**.
    
7.  Repeat these steps for each employee you will pay a commission.
    

To pay employee commissions, go to _Transactions > Commissions > Authorize Employee Commissions (Administrator)_.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Paying Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1153252.html)
-   [Creating Payroll Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556724572.html)
-   [Authorizing Employee Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1149753.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
