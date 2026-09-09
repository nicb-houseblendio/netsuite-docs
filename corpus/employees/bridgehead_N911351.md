---
id: "bridgehead_N911351"
type: "bridgehead"
title: "Entering an Expense Report in the Employee Center"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Expense Reports and Purchase Requests > Expense Reporting > Enter an Expense Report > Entering an Expense Report in the Employee Center"
parent: "section_N911232"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N911351.html"
anchors: []
sha256: "9773742b44237abde37df0f8c0d5d3e8636e53df09aabd7d61bfb610e497a06a"
---

Usually, employees enter expense reports when they are logged in with the Employee Center role. Employees can enter expenses when logged in with a role other than Employee Center if they have the Create level of the Expense Reports permission. If approval routing is set up, all expense reports must be entered through the Employee Center to maintain the hierarchy of approval routing.

#### To enter an expense report when logged in with the Employee Center role:

1.  On the Employee Center Home page, in the **Home Links** portlet, click the **Enter Expense Reports** link.
    
    If you use NetSuite OneWorld, notice that the **Subsidiary** field is automatically populated with your subsidiary.
    
2.  NetSuite inserts today's date as the date of this expense report. You can optionally enter another date.
    
    The **Expenses Total and Amount** field values are calculated based on the amounts entered for expense line items.
    
    There's a summary box in the top corner that shows real-time totals for expenses, non-reimbursable and reimbursable expenses, any advances, and the total reimbursable amount.
    
3.  Enter an advance that should be applied to any reimbursement for these expenses.
    
4.  Enter the purpose of these expenses.
    
5.  If your company uses foreign currency expense reports, in the **Currency** field, select the currency in which you want your reimbursement to be paid.
    
    Note:
    
    Currencies must first be set up on the employee record. Only currencies defined on the employee record are available for selection in this field.
    
6.  If you use Multiple Currencies, check the **Use Multi Currency** box to show the Foreign Amount, Currency, and Exchange Rate fields for each line item. These fields let you enter expenses in foreign currencies that are reimbursed in the base currency. This is true unless an alternate currency is selected in the **Currency** field.
    
    This box is checked by default if you have enabled the **Use Multicurrency Expense Reports** preference on the General subtab at Home > Set Preferences. You can clear the box to hide Multi Currency fields on individual expense reports. Any expenses entered when Multi Currency fields are hidden are automatically saved in the base currency.
    
    Important:
    
    Exchange rates and converted amounts displayed on expense lines are provided as estimates. Reimbursement amounts are based on rates at the time of reimbursement.
    
7.  If your company tracks them, review the default values entered for **Department**, **Class**, and **Location** to edit as necessary.
    
    Note:
    
    Any department, class, or location selected in the body of the expense report doesn't automatically transfer to the line item fields for each expense. For this information to appear on the GL Impact for each line item you must select the appropriate information for each line item. You can also customize your forms with a custom script to automate this process. For more information, see [SuiteScript 2.x Scripting Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623184.html).
    
    If you enter intercompany expenses, the department, class, or location must be available to the subsidiary associated with the selected customer. Otherwise, an attempt to generate intercompany adjustments for the expenses will result in errors.
    
8.  If you use the American Express integration, on the **Expenses** subtab, click **Imported Expenses** to select your corporate card expense transactions.
    
9.  On the **Expenses** subtab, complete line items for expenses:
    
    1.  The **Ref No.** field is automatically populated with 1 for the first line item on this expense report. You may update this number and each new line item will use the next successive number. Line item reference numbers are helpful when referencing receipts and individual expenses.
        
        Note:
        
        If you use the **Combine Detail Items on Expense Reports** preference, line items are grouped by category, not by entry order. This preference is located at Setup > Accounting > Accounting Preferences > Time & Expenses. For more information, see [Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391368.html#bridgehead_N1391559).
        
    2.  In the **Date** column, enter the date the expense was incurred.
        
    3.  Select an expense category.
        
        If you use NetSuite OneWorld, an expense category is available to only those subsidiaries assigned to the account linked with the expense category. To use intercompany expense transactions, set up expense categories linked to expense accounts that are available to all subsidiaries for use in these transactions. For intercompany expense transactions, users can't save expense lines unless they contain expense categories available to both the employee subsidiary and customer subsidiary. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
        
    4.  If you selected a category that requires a rate, you'll see quantity and rate fields. Enter the quantity for this expense.
        
    5.  If a rate isn't automatically populated, enter the rate for this expense category. The amount is automatically calculated from the rate and quantity.
        
        Note:
        
        If you use multi-currencies, the foreign amount field is used to calculate expense report totals.
        
    6.  If this expense was incurred in a foreign currency, select the currency, and then enter the foreign currency amount.
        
        If you do system-generated adjustments for intercompany expenses, the currency used for those adjustments is always the base currency of the employee's subsidiary. It may not match the currency recorded. For more information, see [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html).
        
    7.  If it isn't automatically calculated, enter the exchange rate applicable for this expense. (Be aware that any automatically calculated rate is provided as an estimate. The rate at the time of reimbursement is used to calculate the reimbursement amount.)
        
    8.  In the **Amount** column, enter the amount of the expense.
        
        If you entered a foreign currency amount for this expense, the expense is automatically converted to your base currency amount in the **Amount** column. This amount is provided as an estimate. It may not match the reimbursement amount that is calculated based on the exchange rate at the time of reimbursement.
        
        If this expense required a rate, the amount is calculated after a quantity and rate are entered.
        
    9.  Optionally, you can enter a memo, department, class, or location to apply only to this line item.
        
        If you enter intercompany expenses, the department, class, or location must be available to the subsidiary associated with the selected customer. Otherwise, an attempt to generate intercompany adjustments for the expenses will result in errors.
        
    10.  If this item is billable to a customer or project, select it from the **Customer** list, and then check the **Billable** box.
         
         Warning:
         
         Checking the **Billable** box without selecting a customer will generate an error. You must select a customer if the **Billable** box is checked.
         
         If you use NetSuite OneWorld, the Intercompany Time and Expense feature, and the related **Intercompany Expenses** accounting preference, note the following. The feature and the preference determine whether you can select a customer or project with a subsidiary different from yours. If the feature isn't enabled, or if the preference is set to **Disallow**, you can't enter intercompany expenses. Instead, you can select only those customers or projects with the same subsidiary to which you are assigned. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).
         
    11.  You can attach a receipt to each line item. In the **Attach File** column, select **List** to select your receipt from the **File Cabinet** or **New** to upload a new receipt. You can attach the same receipt to multiple line items.
         
    12.  If the receipt for this item is being provided, check the **Receipt** box.
         
    13.  If your company uses non-reimbursable expenses, and this item isn't reimbursable, check the **Non-reimbursable** box. For more information, see [Non-reimbursable Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N912353.html).
         
    14.  Click **Add**.
         
10.  Continue adding expense line items.
     
     Note:
     
     Similar line items on expense reports may be combined if your company has enabled the Combine Detail Items on Expense Reports preference. For more information, see [Projects Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3769284587.html).
     
11.  When you're finished, save the expense report.
     
     Warning:
     
     If your company uses expense report policies, you may receive a warning if one or more of your expense lines are over the allowed amounts. Depending on how the expense report policies are set up, you may be able to submit your expense report without changing the entered expenses. Any expense lines that are a violation of defined policies are highlighted in red. Click **Show Policies** to see details of any policy violations.
     
     You have the following choices:
     
     -   **Submit, Submit & New, or Submit & Print** - to save the report and identify it as complete after you have entered all information.
         
         After an expense report is marked complete, you can no longer make changes to it.
         
     -   **Complete Later** - to save an incomplete form without submitting it. The information is saved, but the form isn't submitted for approval.
         

Important:

Only expense reports that are submitted as complete enter the queue for supervisor or accounting approval.

### Related Topics

-   [Entering an Expense Report with a Role other than Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N911711.html)
-   [Enter an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N911232.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
