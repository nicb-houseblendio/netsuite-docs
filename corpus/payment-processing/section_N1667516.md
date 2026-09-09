---
id: "section_N1667516"
type: "section"
title: "Processing Customer Refunds"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Processing Payments > Processing Customer Refunds"
parent: "section_N1665126"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1667516.html"
anchors: ["procedure_N1667547"]
sha256: "3e1a26e8e1e77c30b6afef1f8142b7c0b2961e34e841f51952a469c141fd4070"
---

Perform these steps to generate payment files for customer refund payments.

You can select multiple customer refunds to process. Payment instructions for all selected customer refunds are included in a single payment file.

Note:

Make sure that the customer refund records that you are generating payment files for have previously been entered in NetSuite before performing this task. For more information, see [Refunding an Open Balance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313840.html).

Note:

When processing a customer refund, you must select the mode of payment on the customer payment record. If you check the **For Electronic Bank Payment (Direct Debit)** box, the **Check#** field and other payment options are automatically cleared in the customer refund when you save the record.

The **Check#** or **To EFT** fields are automatically filled depending on the default setting on the customer record. When selecting a refund method, you can change the **Check#** or **To EFT** fields manually.

When you change the account number, the system clears the default setting. The **To EFT** box is cleared and the **Check#** field value is automatically filled.

#### To pay customer refunds: {#procedure_N1667547}

1.  Go to Payments > Payment Processing > Customer Refund Payments.
    
2.  Complete the following fields:
    
    | Field | Description |
    | --- | --- |
    | Bank Account | Select your company bank account where the customer refund payments are posted. For information about setting up company bank account records, see [Setting Up Bank Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590309.html). The payment file format, maximum number of payments, and subsidiary of the payment file are based on the bank account that you select. |
    | Date from | Limit the list of customer refunds to only those approved on a particular date or later. To limit the customer refunds to those approved within a range of dates, enter values for both **Date from** and **Date to** fields. |
    | Date to | Limit the list of customer refunds to only those approved on a particular date or earlier. To limit the customer refunds to those approved within a range of dates, enter values for both **Date from** and **Date to** fields. |
    | Amount From and Amount To | Use these fields to narrow down the list of outstanding payment transactions by their transaction amount.
    -   Use the **Amount From** field to list transactions that are equal or greater than the specified amount.
    -   Use the **Amount To** field to list transactions that are equal or less than the specified amount.
    -   Use both fields to list transactions that are within a range of entered amounts.
    
     |
    | Customer | Narrow down the list of customer refunds to process to a particular customer. The customers list is displayed when the following criteria is met for Bank Payment Details (Debit and Credit):
    
    -   When a subsidiary is not attached to a Customer Entity Bank:
        -   Subsidiaries of company bank and primary customer must match.
        -   File formats of company bank and customer entity bank must match.
        -   Customer entity bank must be primary and active.
    -   When a subsidiary is attached to a Customer Entity Bank:
        -   Subsidiaries of company bank and primary customer must match.
        -   File formats of company bank and customer entity bank must match.
        -   Customer entity bank must be primary and active.
    
     |
    | Date to be Processed | Specify the date when you want the Electronic Bank Payments SuiteApp to generate the payment files for the selected transactions. |
    | EFT File Reference Note | Enter notes to display in the header portion of the generated payment file. |
    
    Note:
    
    The Select Transactions list shows customer refunds. Customer refunds that are not included are those that have check numbers, those that are marked To be Printed, and those that were voided. To display the **Name** column, go to Payments > Setup > Electronic Payments Preferences, click the **General Preference** subtab, and check the **Include Name in Transaction List** box.
    
3.  On the **Select Transactions** subtab, in the **Pay** column, check the box for the customer refund transactions that you want to process.
    
    In the Payment Information section, the following fields are automatically updated:
    
    -   **Number of Transactions** - This field displays the total number of customer refund transactions that you selected for payment processing.
        
    -   **Total Payment Amount** - This field displays the sum of the values in the **Payment Amount** column or the sum of customer refunds.
        
    
    Use the following fields and controls to filter the transactions list:
    
    -   **Select Page** - Select a range of pages to display transactions included in those pages.
        
    -   **Transactions Per Page** - Select the number of rows to be displayed per page.
        
    -   Use the **Mark All** or **Unmark All** button to check or clear the box for all transactions in the list.
        
    
    Note:
    
    The Electronic Bank Payments SuiteApp currently processes up to 5,000 open customer refunds at a time. If you are processing more than 5,000 open bills, you can first process the first 5,000 bills before processing the remaining bills.
    
4.  Click **Submit**. You are redirected to the payment file record on the Payment File Administration form.
    
5.  Click **Refresh** until the value in the **File Processed?** field changes from **Queued** to **Processed**.
    
    When processed, a confirmation message is sent to your email address. The email message confirms that the payment file generation was successful or an error message indicating that the payment file generation failed.
    
6.  Click the download link in the **File Reference** field to save a copy of the payment file to your local drive.
    
    You can electronically send the file format to your bank or upload the file to your bank's electronic payment system.
    

### Related Topics

-   [Processing Payments from Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1668006.html)
-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
