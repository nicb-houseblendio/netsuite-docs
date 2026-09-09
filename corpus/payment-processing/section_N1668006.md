---
id: "section_N1668006"
type: "section"
title: "Processing Payments from Customers"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Processing Payments > Processing Payments from Customers"
parent: "section_N1665126"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1668006.html"
anchors: ["procedure_N1668036"]
sha256: "2fa6ae9119727f09179553e51f9ab3e9da3f0bf859657e94f50b3e1e74cec92f"
---

You can select multiple invoices to process. Payment instructions for all selected invoices are included in a single payment file format. This includes processing of term or early settlement discounts and bill credit or credit memo transactions.

#### To select invoices to process: {#procedure_N1668036}

1.  Go to Payments > Payment Processing > Invoice Payment Processing.
    
2.  Complete the following fields:
    
    | Field | Description |
    | --- | --- |
    | Bank Account | Select your company bank account where the payment transactions should be posted. Note: Only bank accounts on which you have not enabled the Process Bills Automatically option appears on this list. For more information, refer to the Setting Up Company Bank Records topic for your country. The **Select Transactions** subtab is automatically updated with a list of outstanding bills, expenses, and journal entries from that bank account. The payment file format, maximum number of payments, and subsidiary of the payment file are based on the bank account that you select. |
    | A/R Account | Select the accounts receivable register where the payments should be posted. |
    | Date to be processed | Specify the date when you want the bank to process the payment transaction. |
    | Posting Period | Select the accounting period where the bills payments should be posted. |
    | Direct Debit file reference note | Enter notes to display in the Direct Debit file. |
    | Direct Debit Type | For SEPA Direct Debit templates. Select the direct debit type:
    -   **B2B** - SEPA B2B (business to business) direct debit
    -   **CORE** - For SEPA core direct debit
    -   **COR1** - SEPA core direct debit with reduced execution time cycle by one day
    
     |
    | Aggregate by Payee | The option lets you group payments for a particular vendor, customer, partner or employee into a single payment transaction. Disable this option if you want to create payment transactions for every bill or expense report. Important: To check or clear the **Aggregate by Payee** box by default, go to Payments > Setup > Electronic Payments Preferences, click the General Preference subtab, and then check or clear the **Aggregate By Payee (DD)** box. Note: This option is required to process discounts and credit transactions. |
    | Number of Transactions | This field displays the number of outstanding payment transactions that are marked for processing in the Select Transactions list. |
    | Total Payment Amount | This field displays the total amount of outstanding payment transactions that are marked for processing in the Select Transactions list. |
    
3.  Use the following fields to narrow down the list of outstanding payment transactions for processing:
    
    | Field | Description |
    | --- | --- |
    | Transaction Type | Use this field to narrow down the list of outstanding payment transactions to invoices or journals. The list of outstanding payment transactions is automatically updated based on the value you select in this field. |
    | Due date from, to | Use these field to narrow down the list of outstanding payment transactions by their due date.
    -   Use the **Due date from** field to list transactions that are due on or later than the specified date.
    -   Use the **Due date to** field to list transactions that are due on or before the specified date.
    -   Use both fields to list transactions that are due within a range of dates.
    
     |
    | Amount From and Amount To | Use these fields to narrow down the list of outstanding payment transactions by their transaction amount.
    
    -   Use the **Amount From** field to list transactions that are equal or greater than the specified amount.
    -   Use the **Amount To** field to list transactions that are equal or less than the specified amount.
    -   Use both fields to list transactions that are within a range of entered amounts.
    
     |
    | Customer | Use this field to narrow down the list of outstanding payment transactions to invoices that are payable to a particular customer. The customers list is displayed when the following criteria is met for Bank Payment Details (Debit and Credit):
    
    -   When a subsidiary is not attached to a Customer Entity Bank:
        -   Subsidiaries of company bank and primary customer must match.
        -   File formats of company bank and customer entity bank must match.
        -   Customer entity bank must be primary and active.
    -   When a subsidiary is attached to a Customer Entity Bank:
        -   Subsidiaries of company bank and primary customer must match.
        -   File formats of company bank and customer entity bank must match.
        -   Customer entity bank must be primary and active.
    
     |
    | Department Filter | Use this field to narrow down the list of invoices or journals to those that originated from a specific department. |
    | Class Filter | Use this field to narrow down the list of invoices or journals to those that originated from a specific class. |
    | Location | Use this field to narrow down the list of invoices or journals to those that originated from a specific location. |
    
4.  In the Classification section, complete the following fields:
    
    | Field | Description |
    | --- | --- |
    | Department | Select the department for payments made under this bank account. |
    | Class | Select the class for payments made under this bank account. |
    | Location | Select the location for payments made under this bank account. |
    
    Note:
    
    For each category, you can set up to 50,000 classes, departments or locations. Setting up more than 50,000 for each category may slow down the loading of the dropdown list of categories.
    
5.  On the **Select Transactions** subtab, in the **Pay** column, check the box for the invoices that you want to process. You can also check the credit transactions, if any, to be applied to an invoice.
    
    Important:
    
    When applying customer credit memos, be sure to select the invoice and credit memo for the same payee. For multi-currency transactions, be sure to select the invoice and credit memo for the same payee and in the same currency.
    
    Note:
    
    To display the **Name** column, go to Payments > Setup > Electronic Payments Preferences, click the **General Preference** subtab, and check the **Include Name in Transaction List** box.
    
    The following columns of the transactions list are automatically updated for your selected transactions:
    
    -   **Payment Amount** - This field is automatically updated with the invoice amount due for the selected transaction. For credit transactions, this amount shows the exact value from the **Amount Remaining** field. You can edit the amount if you want to enter a partial credit.
        
    -   The following columns apply to invoices with early payment discounts:
        
        -   **Discount Amount** - This field displays the maximum discount amount that can be applied to the transaction, based on the terms defined on the bill. You can edit the amount to enter a partial discount or remove the discount from the transaction. The discount amount must be an addition of Discount Amount and Payment Amount and cannot be greater than the amount remaining for the transactions.
            
            Discount Amount + Payment Amount <= Amount Remaining.
            
            The payment amount is automatically updated to display the recalculated amount with the applied discount.
            
        -   **Discount Date** - This field displays the last day to use or apply the discount before it expires.
            
    
    In the Payment Information section, the following fields are also automatically updated:
    
    -   **Number of Transactions** - This field displays the total number of invoice and credit transactions that you selected for payment processing.
        
    -   **Total Payment Amount** - This field displays the sum of the values in the **Payment Amount** column or the sum of customer payments.
        
    
    Use the following fields and controls to filter the transactions list:
    
    -   **Select Page** - Select a range of pages to display transactions included in those pages.
        
    -   **Transactions Per Page** - Select the number of rows to be displayed per page.
        
    -   Use the **Mark All** or **Unmark All** button to check or clear the box for all transactions in the list.
        
    
    Note:
    
    The Electronic Bank Payments SuiteApp currently processes up to 5,000 open invoices at a time, with the exception of transactions using SEPA Direct Debit. Transactions using SEPA Direct Debit currently processes 3,000 open invoices at a time. If you are processing more than 5,000 open invoices or more than 3,000 open SEPA Direct Debit invoices, only the first 5,000 or 3,000 invoices are selected for processing.
    
6.  Click **Submit**. You are redirected to the payment file record on the Payment File Administration form.
    
7.  Click **Refresh** until the value in the **File Processed?** field changes from **Queued** to **Processed**.
    
    After the payment is processed, a confirmation message is sent to your email address. The email message confirms that the payment file generation was successful or an error message indicating that the payment file generation failed.
    
8.  Click the download link in the **File Reference** field to save a copy of the payment file to your local drive.
    
9.  You can electronically send the file format to your or upload the file to your bank's electronic payment system.
    

### Related Topics

-   [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html)
-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
