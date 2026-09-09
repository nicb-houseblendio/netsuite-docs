---
id: "bridgehead_N938756"
type: "bridgehead"
title: "Fringe Benefit Earning Pay Codes"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Items Setup > Standard Pay Codes > Fringe Benefit Earning Pay Codes"
parent: "section_N935979"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N938756.html"
anchors: []
sha256: "6e58de003b244d4a13b172ace720bbb883e695a6df86e5950c1839a62549134c"
---

In most cases, these codes are additions to earnings for taxation purposes. They account for payments made to employees outside of the payroll system. They are also used for company assets such as vehicles that have value to the employee.

Note:

Fringe earnings on a paycheck must be offset by a deduction with the same amount. You must create a matching deduction to ensure the employee receives no additional cash on the paycheck. To offset a fringe earning code, use a deduction code based on the Fringe Benefits Offset type.

| **Code Name** | **Description** | **Additional Information** | FIT Taxable | FICA Taxable | W-2 box |
| --- | --- | --- | --- | --- | --- |
| Advances - Non-Loans | Code for any advance where repayment is not expected | These are non-loan payments that were made to the employee and need to be reported as taxable income. | Y | Y | box 1, 3, 5 |
| Aggregate Deferrals Under Section 83i Elections | This code should be used to record the aggregate deferrals under Section 83(i) elections as of the close of the calendar year. | Use the pay code Aggregate Deferrals Under Section 83i Elections (Offset) to remove the net effect of the deferrals. | N | N | box 12 Code HH |
| Cost of Employer-Sponsored Health Coverage | Code for health care contributions made by employer Use the Fringe Benefits Offset deduction code to remove the net pay effect of these contributions |  | N | N | box 12 Code DD |
| Cost of Employer-Sponsored Health Coverage (Offset) |  |  |  |  |  |
| Health Care Premiums: Domestic Partner/Civil Union/Same-Sex Marriage (Employer) | For employer contribution for health insurance | Federal law requires that premiums for health insurance for domestic partners is taxable. This code adds the employer contribution to the earnings for taxation. An automatic deduction ensures that the employee is not paid for this amount. | Y | Y | box 1, 3, 5, and 14 |
| HSA (Employer Contribution) | Employer contribution to the Employees Health Spending Account | Paid into a qualified plan. Some states tax these contributions. Set up a matching deduction to ensure the employee is not paid for this amount. Note: This amount is not considered for calculation of base wages for 401(k) contributions. | N | N | box 12 Code W |
| Moving Expenses - Qualified | This code records qualified moving expenses. Used when expenses for an employee's relocation are paid by the employer directly to service providers. The money is already paid to the third party. Therefore, the check should include an offsetting deduction so this amount does NOT increase check's net payment. | These are expenses that were paid to the employee, but not through payroll. These qualified expenses do not affect net pay and are fully reportable and taxable. | Y | Y | Box 12, Code P no longer supported for this pay code Box 1, 3 and 5 |
| Non-Cash Compensation | This records taxable non-cash compensation | This code tracks non-cash compensation, received by the employee, for which value needs to be added to the employee's earnings for taxation purposes. Code is fully taxable. | Y | Y | box 1, 3, 5 |
| Non-Qualified Stock Option | This records non-qualified stock options and is W-2 reportable and taxable. | This code tracks non-qualified stock options, exercised by the employee, for which value needs to be added to the employee's earnings for taxation purposes. Code is fully taxable. | Y | Y | box 1, 3, 5, and box 12 Code V |
| Third Party Sick Pay - Taxable |  | For a sick pay plan, that the employee contributed to, that is paid by a third party. This code does not affect earnings or net pay. An automatic deduction ensures that the employee is not paid for this amount. |  |  | box 1, 3, 5 |
| Third Party Sick Pay - Nontaxable | This code records nontaxable sick pay | This code tracks sick pay plans that employees contribute to and is paid by a third party. This code does not effect earnings or net pay. It enables the amount to be recorded in W-2 box 12 Code J. | N | N | box 12 Code J |
| Group-Term Life Insurance over $50,000 | This records the value of group term life. The IRS determines the standard amount and provides a table for computing the value of the insurance that is in excess of the standard. This code records the value of the excess in regular earnings and reports the value in W-2 box 12 Code C. (Box 1, 3, and 5 of W-2) | You must manually create a matching deduction to ensure the employee receives no additional cash on the paycheck. Set up a matching deduction to ensure the employee is not paid for this amount. For details on creating deductions, see [Creating Payroll Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556724572.html). | N | Y | box 1, 3, 5, and box 12 Code C |
| Tips | This records tips paid directly by customers to the employee. | These payments are added to earnings and are fully taxable. | Y | Y | box 1, 3, 5 |
| Unsubstantiated Reimbursements | Reimbursements for expenses that do not meet the federal rules for exclusion from taxation | These are reimbursements that were previously paid and now determined to be unsubstantiated. They are added to earnings and are fully taxable. | Y | Y | box 1, 3, 5, and 14 |
| Health Ins Employer Pd--2% Shrhldrs | This code is used to set the amount paid by an employer to cover health insurance premiums of an employee of an s-corporation. This employee must be a 2%+ shareholder of the company. | These employer payments are taxed at supplemental rates and if combined with regular earnings, taxed at regular rates. | Y |  | box 1, 14 |
| Non Taxable Fringe Benefit | This code should be used carefully. Use only when the payroll administrator cannot match a benefit on hand with any of fringe code types available in the system. | Because it cannot be matched, it cannot be taxed properly and this code is never taxed. It is up to an employee to report it correctly on personal tax returns. If the amount is large and the benefit taxable, the employee could be liable for an estimated tax payment during the tax year. |  |  |  |
| QSEHRA Coverage | Code for QSEHRA contributions made by employer Use the Fringe Benefits Offset deduction code to remove the net pay effect of these contributions | QSEHRA allows eligible employers to pay or reimburse medical care expenses of eligible employees after the employees provide proof of coverage. | N | N | box 12, code FF |
| QSEHRA Coverage (Offset) |  |  |  |  |  |

### Related Topics

-   [Taxable Earning Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N936321.html)
-   [Other Earning Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N938073.html)
-   [Miscellaneous Pre-Tax Employee Deduction Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N941176.html)
-   [Pension Plan Contribution Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N941423.html)
-   [Education Plan Contribution Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N942422.html)
-   [Cafeteria Plan Contribution Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N942579.html)
-   [After-Tax Deduction Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N942962.html)
-   [Employer Contribution Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N944033.html)
-   [Standard Pay Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N935979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
