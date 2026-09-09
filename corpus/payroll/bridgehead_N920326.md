---
id: "bridgehead_N920326"
type: "bridgehead"
title: "General Payroll Preferences"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Preferences > General Payroll Preferences"
parent: "section_N920073"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N920326.html"
anchors: ["subsect_0714031413", "subsect_0714031625", "subsect_0714035042", "subsect_0714035215"]
sha256: "76bfdd13a8489827fc129701f51ec016c282172239ab8e276bb8e81d25625ae4"
---

The following table describes the preferences available on the Preferences subtab of the Set Up Payroll page. This page is located at _Setup > Payroll > Setup Tasks > Set Up Payroll_.

After you set a preference, you must update payroll information. For more information, see [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html).

## General {#subsect_0714031413}

| Field Name | Function |
| --- | --- |
| Calculate Funding | Check this box if you want NetSuite to create a funding transaction. When you check this box, a single transaction for the total payroll run gets posted to your checking account. If you don't check this box, you'll see a separate transaction for each paycheck in your checking account. |
| Expand Account Lists for Payroll Items | Check this box to associate additional general ledger accounts with payroll items. When this box is clear, you can only associate payroll items with their default accounts. Expense accounts for earning payroll items, and liability accounts for deduction payroll items. When you check this box, you get more options:
-   **Deduction payroll item** can be associated with a liability account, asset account, or expense account. If you associate a deduction payroll item with an asset or expense account, that account is credited in the general ledger.
-   **Earning payroll item** can be associated with an expense account, asset account, or liability account. If you associate an earning payroll item with an asset or liability account, that account is debited in the general ledger.

Important: This preference impacts the general ledger. After you check the box, you can only clear the box after all payroll items are associated with their default accounts. For example, deduction payroll items associated with liability accounts. |
| Pay PTO Prior to Pay Period (Days) | Enter the number of days prior to the current pay period to pay personal time off (PTO) for approved time entries. You should enter zero unless you plan to pay employees before the last pay period ends. |
| Pay Earnings Prior to Pay Period (Days) | Enter the number of days before the current pay period when you want to pay earnings that weren't included in the last pay period. You should enter zero unless you plan to pay employees before the last pay period ends. If your employees have been tracking their time using the Time Tracking feature, note the following:

-   If you're adding them to payroll and want to use this preference,, you must enter their last paid date manually on their employee records.
-   Manual entry ensures that the employee's pay is calculated correctly.

For more information, see [Including an Employee in Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921988.html). |
| Payroll Issues Alert Email Addresses | Enter the email addresses for users who'll get alert messages if there are any payroll issues. You can use commas, semi-colons, or spaces to separate multiple addresses. |
| Main Office | Select the name of the workplace that represents the main or home office for your business. NetSuite uses this workplace to calculate taxes for an employee if you haven't picked a workplace on their record. See [Entering Workplace Records for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918520.html). |
| Type of Organization | Select the type of organization that best describes your company: corporation, government agency, LLC (limited liability corporation), partnership, or proprietorship. The selection you make may affect the options available when setting up your payroll. For example, if you select Partnership, you can set up partners with the right tax exemptions. |

## Paychecks {#subsect_0714031625}

| Field Name | Function |
| --- | --- |
| Show Paychecks with Zero Amounts | Check this box if you want to see paychecks for employees who worked zero hours on the Payroll Batch page. |
| Pay Expenses on Paychecks | Check this box if you want to pay approved expense report amounts in NetSuite to employees on their paychecks. You must create an expense payroll item to use this preference. For more information, see [Paying Expenses on Employee Paychecks with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914230.html). |
| Pay Employee Commissions on Paychecks by Default | Check this box if you want to pay approved commission amounts in NetSuite to employees on their paychecks You must create a commission payroll item to use this preference. For more information, see [Payroll Items Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930985.html). |
| Always Classify Individual Paycheck Lines | Check this box if you want the **Classify Individual Paycheck Lines** box to be checked by default on paychecks. When the Classify Individual Paycheck Lines box is checked, you can classify individual paycheck lines by class, department, or location. For more information, see [Classifying Individual Paycheck Lines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543951211.html). |
| Default 'To Be Printed' on Paychecks | Check this box if you want the **To Be Printed** box checked by default when processing individual paychecks or run payroll. |
| Default 'Do Not Accrue Time' on Paychecks | Check this box if you want the **Do Not Accrue Time** box to be checked by default when you process individual paychecks or run payroll. If you check this box, sick and vacation accruals won't process. |
| Default 'Pay Bonuses' on Paychecks | Check this box if you want the **Pay Bonuses** box to be checked by default on payroll batches. If the Pay Bonuses box is checked on payroll batches, bonuses for the pay period are added to paychecks when you calculate the payroll batch. Note: This preference is available only if the Compensation Tracking feature is enabled in your account. For more information, see [Integrating Bonuses with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157488927059.html). |
| Pay Sick/Vacation Time on Paychecks | Check this box if you want the **Pay PTO** box to be checked by default when you process individual paychecks or run payroll. If you don't check this box, sick time and vacation time won't be paid. |
| Show Only Vacation and Sick Payroll Items in PTO Hours | Check this box if you want to limit the payroll items that show up in the PTO Hours subtab of paycheck records to Earning:Sick or Earning:Vacation. These payroll items appear in the PTO Hours subtab if you associate them with time-off pay codes. Paid time off codes include Paid Time Off - Taxable, Sick Pay, Holiday, and Personal. Clear this box if you want to include any payroll item associated to a time-off pay code on the PTO Hours subtab. For example, you might want to include a payroll item for jury duty. |
| Mask Social Security Numbers on Vouchers | Check this box if you want to mask employees' social security numbers on paycheck vouchers. When you check this box, only the last four digits of the social security number show on the voucher (for example, xxx-xx-1234). For vouchers, this preference depends on your permissions and other settings. For example, if Bob has full permission to view social security numbers, they'll still be masked when he views a voucher if you check this box. For more information, see [Working with Employee Social Security Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901259.html). |
| Print Single Copy Voucher | Check this box if you want to include one copy of the paycheck voucher with the paycheck. When this box is clear, taxes and deductions on paychecks may be truncated for employees with numerous tax and deduction line items. Also, NetSuite prints two vouchers when you select vouchers at _Transactions > Management > Print Checks and Forms_. |
| Enable Multi-State Calculation | Check this box if you want to calculate the right taxes for employees who work in different states during a pay period. These taxes include the jurisdiction where the work is done, plus the employee's main office and home jurisdictions. For more information, see [Setting up Taxes for Employees who Work in Different States During a Pay Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4791613456.html). |
| Decrease Elective Deferral Limits and Automatically Calculate Catch-Up | Check this box if you want to do the following:
-   Override annual limits
    -   Decrease the annual elective deferral limit for specific employees on their employee records.
    -   Decrease the annual catch-up over age 50 limit for specific employees on their employee records. Note: The feature for decreasing elective deferral limits feature doesn't apply to 457(b) catch-up deduction codes.If you need to clear or edit limits, do so at the beginning of each calendar year.
-   Automatically calculate standard and higher catch-up contributions for employees who meet the following criteria:
    -   Have a catch-up over age 50 and catch-up age 60 - 63 deduction assigned on their record.
    -   Reach the annual elective deferral limit.
    -   For catch-up over age 50, an employee must be 50 years of age or older by the end of the current calendar year. For catch-up age 60 - 63, an employee must be 60 to 63 years of age by the end of the current calendar year.
-   Automatically spill over catch-up contributions to Roth when Section 402(g) limits are met for employees who meet all of the following criteria:
    
    -   Are age 50 or older.
    -   Have Social Security wages that exceed the annual threshold. For tax year 2025, the threshold is $150,000 for contributions made in 2026. This amount is subject to change.
    
    Note: Automatic Roth spillover is supported only when previous Social Security wage history is available for the employee. If previous Social Security wage history isn't available, the feature doesn't automatically spill over catch-up contributions to Roth. During your initial implementation, monitor employee catch-up contributions to ensure that employees who are required to make Roth catch-up contributions don't contribute to a pre-tax catch-up deduction.

For more information, see the following topics:

-   [Decreasing Elective Deferral Limits for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162731062157.html)
-   [Setting Up Automatic Catch-Up Over Age 50 Calculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162921088440.html)
-   [Setting Up Automatic Catch-Up Age 60 - 63 Calculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0306094149.html)

 |
| Show Payroll Item Descriptions on Summary Tab of Paychecks | Check this box if you want to show payroll item descriptions on the Summary subtab of paychecks. You can add descriptions to payroll item records to give your employees more information about each payroll item. For more information, see [Creating Payroll Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556724572.html). |
| Paychecks Visible to Employees | Choose when paychecks should be visible to employees in the Employee Center. Options are when the payroll batch is committed, on the check date, one day before the check date, or two days before the check date. If you use NetSuite OneWorld, this preference applies to all employees in a subsidiary who get paid with SuitePeople Payroll. If you do not use OneWorld, this preference applies to all employees in your organization who get paid with SuitePeople U.S. Payroll. For more information, see [Specifying When Employees Can View Paychecks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156278676101.html). |

## Reporting {#subsect_0714035042}

| Field Name | Function |
| --- | --- |
| Report Payroll Liabilities By | Choose whether you want to report your payroll liabilities quarterly or year-to-date (YTD). |
| Use Year-to-Date Values on Reports (This option is applicable only in the year that payroll is first implemented.) | Check this box if you want reports to show the YTD values you entered for employees during setup. When you check this box, the values for checks and adjustments entered before the YTD data won't show up on reports. If this box is clear, check and adjustment amounts might make your report data not match the amounts you committed during payroll setup. |

## Self-Service {#subsect_0714035215}

For more information, see [Enabling Employees to Update Direct Deposit Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511534973.html).

| Field Name | Function |
| --- | --- |
| Employees Can View or Change Banking Information | Check this box if you want employees to make changes to their bank accounts for direct deposit. Employees can update their bank account information using their Employee Center roles. |
| Employees Can Choose to be Paid by Check | Check this box if you want employees to change their net payment method from direct deposit to check. Employees use the Employee Center role to update their payment method. This preference is available only if the Employees Can View or Change Banking Information box is also checked. |

### Related Topics

-   [Setting the Subsidiary for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N920116.html)
-   [Setting Up Automatic Catch-Up Over Age 50 Calculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162921088440.html)
-   [Enabling Employees to Update Direct Deposit Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511534973.html)
-   [Specifying When Employees Can View Paychecks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156278676101.html)
-   [Setting Default Accounts for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N921047.html)
-   [Setting Preferences for Jurisdictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N921222.html)
-   [Setting Specific Tax Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N921258.html)
-   [Setting Up Email Alerts for Payroll Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921495.html)
-   [Payroll Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N920073.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
