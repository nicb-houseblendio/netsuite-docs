---
id: "section_N924516"
type: "section"
title: "Employee Tax Withholdings and Allowances"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Payroll Setup for Employees > Taxes and Jurisdiction Setup for Employees > Employee Tax Withholdings and Allowances"
parent: "section_1556740089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N924516.html"
anchors: ["subsect_157349136431", "subsect_157349139990", "subsect_157565702031", "subsect_157349143006"]
sha256: "8857396e7e38e6509eccf91f463d77a294fd522133d8909375125239d3a37826"
---

After you include an employee in payroll and update payroll information, SuitePeople U.S. Payroll uses the home address and workplace to create a list of applicable tax items for the employee. These tax items appear on the Taxes subtab, under the Payroll subtab of the employee record.

For each employee, you should do the following:

-   Check the tax rates
    
-   Add additional withholding information based on the information that employees submit in federal Form W-4 or in state-specific tax forms
    

Learn how to set up tax withholdings and allowances in the following topics:

-   [Entering Form W-4 (2020 version) Information for an Employee](#subsect_157349136431)
    
-   [Entering Legacy Form W-4 Information for an Employee](#subsect_157349139990)
    
-   [Reverting to the 2019 Version of Form W-4](#subsect_157565702031)
    
-   [Setting Up Other Tax Withholdings and Allowances](#subsect_157349143006)
    

To learn more about the taxes applicable for employees in each state in the U.S., you can visit the [IRS website](https://www.irs.gov/businesses).

## Entering Form W-4 (2020 version) Information for an Employee {#subsect_157349136431}

Important:

The 2020 version of Form W-4 is available as of January 1, 2020.

U.S. employees are required to complete Form W-4 and submit it to their employers. NetSuite uses the information from the Form W-4 to calculate the appropriate amount of federal taxes to withhold from paychecks. Some states also use Form W-4 for state tax withholdings. For more information about Form W-4, visit the [IRS website](https://www.irs.gov/forms-pubs/about-form-w-4).

#### To enter Form W-4 information for an employee:

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee's name, click **Edit**.
    
3.  Click the **Payroll** subtab, and then click the **Taxes** subtab.
    
4.  In the row containing federal withholding, or, if applicable, state withholding, in the **Tax Form** column, click **W-4**.
    
5.  Enter the employee's information in the form:
    
    -   If the employee has indicated that they are exempt from tax withholding, check the **Exempt** box.
        
        If you check this box, the other fields on the form, with the exception of the Filing Status field, are no longer editable.
        
    -   From the **Filing Status** list, select the employee's filing status.
        
    -   If the employee has checked box 2(c) on Form W-4, check the **Multiple Jobs or Spouse Works** box.
        
    -   In the **Dependents Total Amount** field, enter the amount from box 3 on the employee's Form W-4.
        
    -   In the **Other Income** field, enter the amount from box 4(a) on the employee's Form W-4.
        
    -   In the **Deductions** field, enter the amount from box 4(b) on the employee's Form W-4.
        
    -   In the **Extra Withholding Per Pay Period** field, enter the amount from box 4(c) on the employee's Form W-4.
        
        Note:
        
        If you enter an amount in this field, the **Override Amount** field on the Taxes subtab automatically populates with the same amount. The **Tax Override Method** field also changes to Adjusted Amount.
        
6.  Click **Save**.
    

After you enter Form W-4 information, make sure that you update payroll information. For more information, see [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html).

## Entering Legacy Form W-4 Information for an Employee {#subsect_157349139990}

You may be setting up taxes for employees who submitted the legacy version (the version used from 2019 or earlier) of Form W-4. If this is the case, use the following procedure to enter their Form W-4 information.

As of January 1, 2020, employees should submit the 2020 version of Form W-4 in the following scenarios:

-   The employee is new to the company.
    
-   The employee is updating their withholdings. This can be due to a life event, such as marriage or having a child.
    

For more information, see [Entering Form W-4 (2020 version) Information for an Employee](#subsect_157349136431).

#### To enter legacy Form W-4 information for an employee:

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee's name, click **Edit**.
    
3.  Click the **Payroll** subtab, and then click the **Taxes** subtab.
    
4.  In the federal withholding row, enter the information from Form W-4.
    
5.  Click **Save**.
    

After you enter Form W-4 information, make sure that you update payroll information. For more information, see [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html).

## Reverting to the 2019 Version of Form W-4 {#subsect_157565702031}

If you accidentally updated an employee to the Form W-4 2020 version, you may have to revert to the 2019 version of Form W-4. You can revert the form only if the 2019 version of the form immediately precedes the current version of the form. If you make additional changes to the 2020 version of the form, you cannot revert to the 2019 version.

#### To revert to the 2019 version of Form W-4:

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee's name, click **Edit**.
    
3.  Click the **Payroll** subtab, and then click the **Taxes** subtab.
    
4.  In the row containing federal withholding, in the **Tax Form** column, click **W-4**.
    
5.  At the top of the form, click **Revert**.
    
6.  In the confirmation message, to confirm that you want to revert the form, click **Revert**.
    

## Setting Up Other Tax Withholdings and Allowances {#subsect_157349143006}

You may need to set up state withholdings and allowances for your employees.

#### To set up tax withholdings and allowances for an employee:

1.  Go to _Lists > Employees > Employees_.
    
2.  Next to the employee's name, click **Edit**.
    
3.  Click the **Payroll** subtab, and then click the **Taxes** subtab.
    
4.  For the applicable tax items, complete the following:
    
    -   In the **Filing Status** column, verify that the selected status for each tax item is correct. This information is available on the employee's tax forms.
        
    -   If the employee qualifies as exempt for any of the listed taxes, check the **Exempt** box for the tax item.
        
    
    -   In the **Exemptions/Allowances** column, enter the number of exemptions or allowances for the employee for each tax item.
        
    -   To apply a tax override method to a tax item, from the **Override Method** list, select a method, and then enter an override amount. For more information, see [Tax Override Methods for Employee Withholding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N925327.html).
        
5.  Click **Save**.
    

After you enter Form W-4 information, make sure that you update payroll information. For more information, see [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html).

### Related Topics

-   [Verifying the Jurisdictions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921903.html)
-   [Selecting Status Exemptions for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549401872.html)
-   [Setting up Taxes for Employees who Work in Different States During a Pay Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4791613456.html)
-   [Adding Standard Occupational Classification Codes for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1506349052.html)
-   [Setting up California VDI for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529938339.html)
-   [Paid Family and Medical Leave Contributions for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0113124114.html)
-   [Setting up Payroll for Expatriate Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4099382383.html)
-   [Taxes and Jurisdiction Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1556740089.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
