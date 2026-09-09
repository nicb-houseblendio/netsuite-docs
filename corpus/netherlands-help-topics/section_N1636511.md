---
id: "section_N1636511"
type: "section"
title: "Setting Up Company Bank Records in the Netherlands"
branch: "netherlands-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Netherlands Help Topics > Netherlands-Specific SuiteApp > Netherlands Localization > Netherlands Payment Formats > Setting Up Company Bank Records in the Netherlands"
parent: "section_N1636146"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636511.html"
anchors: ["procedure_N1636523"]
sha256: "3a62ea8731ca954407ac9e4425b04cd1107de2c20fd91df11bb2f5dd5e04c783"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. It's not a best practice to create company bank records by using SuiteScript APIs or CSV Imports.

Set up the bank account records that your company or subsidiaries will be using to send and receive electronic bank payments.

#### To set up company bank details in the Netherlands: {#procedure_N1636523}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically generated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account isn't available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they're displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select **Equens-ClieOp**, **Equens-ClieOp (ING Bank)**, **SEPA Credit Transfer (HSBC)**, or **SEPA Credit Transfer (Netherlands)**. Important: Select **Equens-ClieOp (ING Bank)** if you're setting up your company's account in a bank that belongs to the ING Group. Select **Equens-ClieOp** to set up your company's account in other Dutch banks. ING banks support variant B of the ClieOp format. Other Dutch banks support variant C. |
    | DD Template | Select **SEPA Direct Debit (ABN AMRO)**. Note: The SEPA Direct Debit (ABN AMRO) template can process up to 3,000 transactions in a single payment run. |
    | File Cabinet Location ID | Enter the internal ID of the folder that you created for storing payment format files. For more information, see [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html). |
    | File Name Prefix | (Optional) Enter a prefix for the file number sequence. The prefix is attached to the beginning of each file number whenever this bank is used in creating a payment file. |
    
3.  Click **Save**.
    
4.  Complete the additional bank detail fields..
    
    | Field | Description |
    | --- | --- |
    | Department | Select the department for payments made under this bank account. |
    | Class | Select the class for payments made under this bank account. |
    | Location | Select the location for payments made under this bank account. |
    
    Note:
    
    For each category, you can set up to 50,000 classes, departments or locations. Setting up more than 50,000 for each category may slow down the loading of the dropdown list of categories.
    
5.  If you selected an EFT template, complete the applicable fields on the **EFT Template Details** subtab. The fields displayed are dependent on the EFT format selected.
    
    Note:
    
    The **EFT Template Details** subtab isn't displayed if you did not select a value in the EFT Template field.
    
    | Field | Description |
    | --- | --- |
    | Account Number | Enter the 9-digit number that identifies your company's account in the bank. |
    | Sender Identification | Enter information to identify your company as the sender of the payment. |
    | IBAN | Enter your company's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of your company's bank (eight or 11 characters). |
    | Company Id | Enter the code the bank uses to identify your company. This is assigned by the bank. |
    | Issuer | Enter the code the bank uses to identify fund transfers from your company. This is assigned by the bank. |
    | Address Line 1 | Enter the street address of your company's bank. |
    | Address Line 2 | Enter the building, city, or town address of your company's bank. |
    | Company Name | Enter your company's name. |
    | HSBC Connect Id | Enter your company's HSBC Connect Id. |
    | Country | Select the country where your company is located. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    
6.  If you selected **SEPA Direct Debit (ABN AMRO)** in the DD template, complete the applicable fields on the **DD Template Details (SEPA Direct Debit (ABN AMRO))** subtab.
    
    Note:
    
    The **DD Template Details** subtab isn't displayed if you didn't select a value in the DD Template field.
    
    | Field | Description |
    | --- | --- |
    | IBAN | Enter your company's International Bank Account Number (IBAN). |
    | Company Name | Enter your company's name. |
    | Creditor ID | Enter your company's Creditor Identification number issued by your bank. |
    | BIC | Enter your Bank Identifier Code/Swift Code (8 or 11 characters), which is used to identify banks worldwide. |
    
7.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Inactive | Check this box if you want to make a payment batch inactive. When you mark a record as inactive, it's not displayed in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the **Inactive** box for the main batch, bills that don't meet search criteria won't be included in the payment batch. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    
8.  Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
9.  Click **Save** to save the company bank details.
    

If you want to set up approval routing for this bank account, see [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).

### Additional Information

-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)

### Related Topics

-   [Setting Up Bank Records of Vendors in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1638884.html)
-   [Setting Up Bank Records of Employees in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1639339.html)
-   [Setting Up Bank Records of Customers in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1639791.html)
-   [Setting Up Bank Records of Partners in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851230281.html)
-   [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html)
-   [Netherlands Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636146.html)
-   [Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1585433.html)
-   [EMEA Localization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157122959910.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
