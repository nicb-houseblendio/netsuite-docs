---
id: "section_N1666511"
type: "section"
title: "Manually Processing Bills and Expenses"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Processing Payments > Processing Bills and Expenses > Manually Processing Bills and Expenses"
parent: "section_N1665255"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html"
anchors: ["procedure_N1666554"]
sha256: "07177a410ccff6e98c613c0dbef8101bafe691746e78e68b4198c6ec45f17aca"
---

You cannot process bills, expenses, and partner and employee commissions in batches if you don't have an active Electronic Bank Payments license. However, you can still process outstanding bills, commissions, journals, and expenses by manually selecting the payment transactions from the bill payments list. Processing includes term or early settlement discounts and bill credit or credit memo transactions.

For OneWorld accounts, if you want to process payments for a vendor's secondary subsidiary, be sure that your role has access to that secondary subsidiary. For more information, see [Setting Up Roles and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1586829.html). If you use the Class, Department, and Location features, be sure to align them with the correct subsidiary. When processing payments, you can select only a class, department or location assigned to subsidiaries that you have access to.

For more information, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html). For more information about multiple subsidiaries, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

Note:

Make sure that the bills and expenses that you want to generate payment files for have previously been entered in NetSuite. For more information, see [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html) and [Enter an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N911232.html).

You can select multiple bills to process. A single payment file is created for all selected transactions.

#### To process bills and expenses manually: {#procedure_N1666554}

1.  Go to Payments > Payment Processing > Bill Payment Processing.
    
    Important:
    
    If the Vendor Payments preference for Approval Routing (Setup > Accounting > Accounting Preferences > Approval Routing) is enabled, you will not be able to manually process vendor bill payments using Electronic Bank Payments SuiteApp. If you want payment batches to go through an approval process before they can be sent to the bank, use the EFT Payment Batch Approval Routing. For more information, see help topic [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).
    
2.  Complete the following fields:
    
    | Field | Description |
    | --- | --- |
    | Bank Account | Select your company bank account where the payment transactions should be posted. The payment file format, maximum number of payments, and subsidiary of the payment file are based on the bank account that you select. |
    | A/P Account | Select the accounts payable register where the payments are posted. Note: An A/P Account that is included in a batch is removed from the selection list. Instead, you should see the A/P account listed in the company bank record along with the enabled **Process Bills Automatically** option. For more information, see the Setting Up Company Bank Records topic for your country or [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). When you select an A/P account, the **Select Transactions** subtab automatically displays the account's list of outstanding bills, expenses, and journal entries. Note: On the Bill Payment Batch page, the list of transactions are displayed on the **Select Transactions** tab. The list does not include bills placed on payment hold. For more information, see [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html). |
    | Date to be processed | This field displays the date when the record is first created. Specify the date when you want the bank to process the payment transaction. |
    | Posting Period | Select the accounting period where the bills payments should be posted. |
    | EFT File Reference Note | Enter notes to display in the header portion of the generated EFT file. |
    | Aggregate by Payee | This box is checked by default to enable you to group payments for a particular vendor, customer, partner or employee into a single payment transaction. Clear this box if you want to create payment transactions for every bill or expense report. Important: To check or clear the **Aggregate by Payee** box by default, go to Payments > Setup > Electronic Payments Preferences. On the General Preference subtab, check or clear the **Aggregate By Payee (EFT)** box. Note: This option is required to process transactions with discounts and credits. |
    | Number of Transactions | This field displays the number of outstanding payment transactions that are marked for processing in the Select Transactions list. |
    | Total Payment Amount | This field displays the total amount of outstanding payment transactions that are marked for processing in the Select Transactions list. Note: In accounts where the bank and base currencies are different, the bank currency is used for the Total Payment Amount. |
    
3.  Select values in the following fields to narrow down the list of outstanding payment transactions for processing:
    
    | Field | Description |
    | --- | --- |
    | Transaction Type | Use this field to narrow down the list of outstanding payment transactions to either bills, expenses, or journal entries. The list of outstanding payment transactions is automatically updated based on the value you select in this field. |
    | Due date from, to | Use this field to narrow down the list of outstanding payment transactions by their due date.
    -   Use the **Due date from** field to list transactions that are due on or later than the specified date.
    -   Use the **Due date to** field to list transactions that are due on or before the specified date.
    -   Use both fields to list transactions that are due within a range of dates.
    
     |
    | Vendor | Use this field to narrow down the list of outstanding payment transactions to bills payable to a particular vendor. The vendor list is displayed when the following criteria is met:
    
    -   Subsidiaries of company bank and primary vendor bank must match.
    -   Company bank and vendor bank file formats must match.
    -   Vendor bank must be primary and active.
    
     |
    | Employee | Use this field to narrow down the list of outstanding payment transactions to expenses payable to a particular employee. |
    | Partner | Use this field to narrow down the list of outstanding commissions payable to a particular partner. |
    | Amount From and Amount To | Use these fields to narrow down the list of outstanding payment transactions by their transaction amount.
    
    -   Use the **Amount From** field to list transactions that are equal or greater than the specified amount.
    -   Use the **Amount To** field to list transactions that are equal or less than the specified amount.
    -   Use both fields to list transactions that are within a range of entered amounts.
    
     |
    | Include All Credits | Use this box to filter and display all credit transactions on the Bill Payments Processing and Invoice Payments Processing pages. Check the **Include All Credits** box to filter all the credit transactions irrespective of the due dates entered in the due date filters. Clear the box to filter the transactions based on the due dates entered in due date filters. This box is enabled when one or both due date filters are filled with values or the box remains disabled. |
    
4.  In the Classification section, select the values on the following fields:
    
    | Fields | Description |
    | --- | --- |
    | Department | Select the department for payments made under this bank account. |
    | Class | Select the class for payments made under this bank account. |
    | Location | Select the location for payments made under this bank account. |
    
    Note:
    
    For each category, you can set up to 50,000 classes, departments or locations. Setting up more than 50,000 for each category may slow down the loading of the dropdown list of categories.
    
    These fields specify department, class, and location values shown on payment records that are created after processing the payment transactions. However, the payment records use the department, class, and location values of the payment transactions, depending on the aggregation settings:
    
    -   If the **Aggregate by Payee** option is enabled, the payment records show the department, class, or location entered in the payment batch, regardless of the department, class, and location values of the individual payment transactions.
        
    -   If the **Aggregate by Payee** option is enabled, and an aggregate by either department, class, or location is used as a second-level aggregation method, the payment records show the department, class, or location of the payment transactions instead of the values entered in the payment batch.
        
    -   If the **Aggregate by Payee** option is disabled, the payment records show the department, class, and location values of the payment transactions instead of the values specified in the payment batch.
        
    
    Additionally, payment records use the department, class, and location values of the payment transactions based on the Allow Per-Line Departments, Allow Per-Line Classes, and Allow Per-Line Location settings saved in the Accounting Preferences:
    
    -   If any of the allow per-line options are enabled, the payment records show the department, class, and location values entered in the payment batch.
        
    -   If any of the allow per-line options are disabled, the payment records show the department, class, and location values of the payment transactions.
        
    
    For more information about NetSuite Accounting Preferences, see [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html).
    
5.  On the **Select Transactions** subtab, in the **Pay** column, check the box for the bills and expenses that you want to process. You can also check credit transactions, if any, to be applied to a bill.
    
    Important:
    
    When applying vendor credits and customer credit memos, be sure to select the bill and bill credit for the same payee. For multi-currency transactions, be sure to select the bill and bill credit for the same payee and in the same currency.
    
    Note:
    
    To display the **Name** column, go to Payments > Setup > Electronic Payments Preferences, click the **General Preference** subtab, and then check the **Include Name in Transaction List** box.
    
    The following columns of the transactions list are automatically updated for your selected transactions:
    
    -   **Payment Amount** - This field is automatically updated with the amount due for the selected transactions. For vendor and customer credit transactions, this amount shows the exact value in the **Amount Remaining** field. You can edit the amount if you want to enter a partial credit.
        
    -   The following columns apply to bills with early payment discounts:
        
        -   **Discount Amount** - This field displays the maximum discount amount that can be applied to the transaction, based on the terms defined on the bill. You can edit the amount to enter a partial discount or remove the discount from the transaction. The discount amount must be an addition of Discount Amount and Payment Amount and cannot be greater than the amount remaining for the transactions.
            
            Discount Amount + Payment Amount <= Amount Remaining.
            
            The payment amount is automatically updated to display the recalculated amount with the applied discount.
            
        -   **Discount Date** - This field displays the last day to apply or use the discount before it expires.
            
    
    In the Payment Information section, the following fields are also automatically updated:
    
    -   **Number of Transactions** - This field displays the total number of bills, expenses, and credits that you selected for payment processing.
        
    -   **Total Payment Amount** - This field displays the sum of the values in the **Payment Amount** column.
        
    -   **Installment Reference Number** - This field displays the installment number which is being paid when the bills are retrieved.
        
    
    Use the following fields and controls to filter the transactions list:
    
    -   **Select Page** - Select a range of pages to display transactions included in those pages.
        
    -   **Transactions Per Page** - Select the number of rows to be displayed per page.
        
    -   Use the **Mark All** or **Unmark All** button to check or clear the box for all transactions in the list.
        
    
    Note:
    
    The Electronic Bank Payments SuiteApp currently processes up to 5,000 open bills at a time. If you are processing more than 5,000 open bills, only the first 5,000 bills are selected for processing.
    
6.  Click the **Exchange Rates** subtab and change the values in the **Exchange Rate** field if you want to use an exchange rate other than the Currency Exchange Rates set up in your NetSuite account. For more information, see [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html).
    
7.  Click **Submit**.
    
    You are redirected to the payment file record on the Payment File Administration page.
    
8.  Click **Refresh** until the value in the **File Processed?** field changes from **Queued** to **Processed**.
    
    When processed, a confirmation message is sent to your email address. The email message confirms that the payment file generation was successful or an error message indicating that the payment file generation failed.
    
9.  Click the download link in the **File Reference** field to save a copy of the payment file to your local drive.
    
    You can electronically send the file format to your bank or upload the file to your bank's electronic payment system.
    

### Related Topics

-   [Processing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665126.html)
-   [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html)
-   [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html)
-   [Adding the Payment Batch Processing Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666182.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
