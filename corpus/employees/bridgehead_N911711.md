---
id: "bridgehead_N911711"
type: "bridgehead"
title: "Entering an Expense Report with a Role other than Employee Center"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Expense Reports and Purchase Requests > Expense Reporting > Enter an Expense Report > Entering an Expense Report with a Role other than Employee Center"
parent: "section_N911232"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N911711.html"
anchors: []
sha256: "5369c9250ab1d23f401876ddd7e975d348b2d1f727d1eb908057d281df2282ab"
---

Expense reports can be entered by employees when logged in with roles other than the Employee Center. This gives employees the ease of using a single role to handle all of their business tasks. It also enables employees to enter expense reports on behalf on another employee if they have the necessary permissions.

Note:

There is an automated internal system logic for selecting likely ideal value for your account based on the previous usage.

#### To enter an expense report when logged in with a role other than Employee Center:

1.  Go to _Transactions > Employees > Enter Expense Reports_.
    
2.  Select a form to use.
    
3.  In the **Exp. Rept. #** field, NetSuite increases the largest expense report number by one.
    
    You can type another number it you want to. The next expense number will revert to the standard pattern. You can enter a maximum of 45 characters in this field.
    
4.  Select the employee who incurred these expenses.
    
    If you use NetSuite OneWorld, notice that the **Subsidiary** field is automatically populated with the subsidiary associated with the employee.
    
5.  Select an account for this expense. This field is only available if you have checked the **Accounting Approval** box on this form or if you're editing a previously approved expense report.
    
    The **Expenses and Total Amount** field values are calculated based on the amounts entered for expense line items.
    
    There's a summary box in the top corner that shows real-time totals for expenses, non-reimbursable and reimbursable expenses, any advances, and the total reimbursable amount
    
6.  If your company uses foreign currency expense reports, in the **Currency** field, select the currency in which you want the reimbursement to be paid. The Exchange Rate field automatically shows the current exchange rate for your selected currency.
    
    Note:
    
    Currencies must first be set up on the employee record. Only currencies defined on the employee record are available for selection in this field.
    
7.  Enter any advance that should be applied to any reimbursement for these expenses.
    
8.  Enter the purpose of this expense.
    
9.  NetSuite inserts today's date as the date of this expense report. You can optionally enter another date.
    
    Note that a posting period based on the current date is displayed. This period is subject to change until accounting approval of the expense report. If approval occurs after this displayed period has closed, the expense report is posted to the first open period.
    
10.  If available, enter the due date of the expense report.
     
11.  Review the setting for the **Complete** box, and clear it if you intend to make changes to this expense report later.
     
     Only complete reports are submitted for approval and processing. Be aware that after an expense report is marked complete, you can no longer make changes to it.
     
12.  If you have the appropriate authority, check the **Supervisor Approval**, **Accounting Approval**, or both boxes.
     
     Note:
     
     If you have multiple payable accounts, after the **Account Approval** box has been checked the **Account** field automatically populates with the default payable account. You may change this account if necessary. For more information, see [Time & Expenses Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391368.html). If you use NetSuite OneWorld, see [Set Subsidiary Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156717451103.html).
     
13.  Click the **Expenses** subtab.
     
14.  If you use Multiple Currencies, check the **Use Multi Currency** box to show the **Foreign Amount**, **Currency**, and **Exchange Rate** fields for each line item. These fields let you enter expenses in foreign currencies to be reimbursed in the base currency. This is true unless an alternate currency is selected in the **Currency** field.
     
     This box is checked by default if you use the **Use Multicurrency Expense Reports** preference on the **General** subtab at Home > Set Preferences. You can clear the box to hide Multi Currency fields on individual expense reports. Any expenses entered when Multi Currency fields are hidden are automatically saved in the base currency.
     
     Important:
     
     Exchange rates and converted amounts displayed on expense lines are provided as estimates. Reimbursement amounts are based on rates at the time of reimbursement.
     
15.  If you use the American Express integration, on the **Expenses** subtab, click **Imported Expenses** to select your corporate card expense transactions.
     
16.  On the **Expenses** subtab, complete line items for expenses:
     
     1.  The **Ref No.** field is automatically populated with 1 for the first line item on this expense report. You may update this number and each new line item will use the next successive number. Line item reference numbers are helpful when referencing receipts and individual expenses.
         
         Note:
         
         If you use the **Combine Detail Items on Expense Reports** preference, line items on expense reports are grouped by category and aren't listed in the order they were entered. This preference is located at Setup > Accounting > Accounting Preferences > Time & Expenses. For more information, see [Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391368.html#bridgehead_N1391559).
         
     2.  In the **Date** column, enter the date the expense was incurred.
         
     3.  Select an expense category.
         
         If you use NetSuite OneWorld, an expense category is available to only those subsidiaries assigned to the account linked with the expense category. To use intercompany expense transactions, set up expense categories linked to expense accounts that are available to all subsidiaries for use in these transactions. For intercompany expense transactions, users can't save expense lines unless they contain expense categories available to both the employee subsidiary and customer subsidiary. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
         
     4.  If you selected a category that requires a rate, quantity and rate fields appear. Enter the quantity for this expense.
         
     5.  If a rate isn't automatically populated, enter the rate for this expense category. The amount is automatically calculated from the rate and quantity.
         
         Note:
         
         If you use multi-currencies, the foreign amount field is used to calculate expense report totals.
         
     6.  If this expense was incurred in a foreign currency, select the currency, and enter the foreign currency amount.
         
         If you do system-generated adjustments for intercompany expenses, the currency used for those adjustments is always the base currency of the employee's subsidiary. For more information, see [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html).
         
     7.  If it isn't automatically calculated, enter the exchange rate applicable for this expense. (Be aware that any automatically calculated rate is provided as an approximation. The rate at the time of reimbursement is used to calculate the reimbursement amount.)
         
     8.  In the **Amount** column, enter the amount of the expense.
         
         If you entered a foreign currency amount for this expense, the expense is automatically converted to your base currency amount in the **Amount** column. This amount is an estimate, and may not match the reimbursement amount calculated based on the exchange rate at the time of reimbursement.
         
         If this expense required a rate, the amount is calculated a quantity and rate are entered.
         
     9.  Optionally, you can enter a memo, department, class, or location to apply only to this line item.
         
         If you enter intercompany expenses, the department, class, or location must be available to the subsidiary associated with the selected customer. Otherwise, an attempt to generate intercompany adjustments for the expenses will result in errors.
         
     10.  If this item is billable to a customer or project, select it from the **Customer** list and check the **Billable** box.
          
          Warning:
          
          Checking the **Billable** box without selecting a customer will generate an error. You must select a customer if the **Billable** box is checked.
          
          Note:
          
          If you use NetSuite OneWorld and you have shared customer records with multiple subsidiaries, you can choose any customer assigned to the default subsidiary. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
          
          If you use NetSuite OneWorld, the Intercompany Time and Expense feature, and the related **Intercompany Expenses** accounting preference, note the following. The feature and the preference determine whether you can select a customer or project with a subsidiary different from yours. If the feature isn't enabled, or if the preference is set to **Disallow**, you can't enter intercompany expenses. Instead, you can select only those customers or projects with the same subsidiary to which you are assigned. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
          
     11.  You can attach a receipt to each line item. In the **Attach File** column, select **List** to select your receipt from the **File Cabinet** or **New** to upload a new receipt. You can attach the same receipt to multiple line items.
          
     12.  If the receipt for this item is being provided, check the **Receipt** box.
          
     13.  If your company uses non-reimbursable expenses, and this item isn't reimbursable, check the **Non-reimbursable** box. For more information, see [Non-reimbursable Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N912353.html).
          
     14.  Click **Add**.
          
17.  Continue adding expense line items.
     
     Note:
     
     Similar line items on expense reports may be combined if your company has enabled the Combine Detail Items on Expense Reports preference. For more information, see [Projects Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3769284587.html).
     
18.  When you're done, save the expense report.
     
     Warning:
     
     If your company uses expense report policies, you may receive a warning if one or more of your expense lines are over the allowed amounts. Depending on how the expense report policies are set up, you may be able to submit your expense report without changing the entered expenses. Any expense lines that are a violation of defined policies are highlighted in red. Click **Show Policies** to see details of any policy violations.
     

Important:

Only expense reports that are submitted as complete enter the queue for supervisor or accounting approval.

### Related Topics

-   [Entering an Expense Report in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N911351.html)
-   [Enter an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N911232.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
