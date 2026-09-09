---
id: "section_N1614550"
type: "section"
title: "Setting Up Company Bank Records in Germany"
branch: "germany-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Germany Help Topics > Germany-specific SuiteApps > Germany Localization > Germany Electronic Bank Payments > Setting Up Company Bank Records in Germany"
parent: "section_1554985535"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1614550.html"
anchors: ["procedure_N1614562"]
sha256: "fc33c5f95ee349686e22ade329759dc0c7e7cd9820bf78d43e43ce5c1f37daa7"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. You shouldn't create company bank records by using SuiteScript APIs or CSV Imports.

Set up the bank account records that your company or subsidiaries will be using to send and receive electronic bank payments.

#### To set up company bank details in Germany: {#procedure_N1614562}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically generated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account isn't available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they're displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select one of the following:
    -   **DTAUS**
    -   **DTAZV**
    -   **SEPA Credit Transfer (ABN AMRO)**
    -   **SEPA Credit Transfer (Austria)**
    -   **SEPA Credit Transfer (Germany)**
    -   **SEPA Credit Transfer (HSBC)**
    
     |
    | DD Template | Select **DTAUS DD** or **SEPA Direct Debit (Germany)**. Note: The SEPA Direct Debit (Germany) template can process up to 3,000 transactions in a single payment run. |
    | File Cabinet Location ID | Enter the internal ID of the folder that you created in [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html). |
    | File Name Prefix | If the EFT file format for this record is DTAZV, enter **DTAZV\_**. The use of this file prefix is required only for DTAZV. The prefix is attached to the beginning of each file number whenever this bank is used in creating a payment file. If the EFT file format is DTAUS or SEPA Credit Transfer, the use of a file name prefix is optional. |
    
3.  Click **Save**.
    
4.  Complete the additional bank detail fields.
    
    | Field | Description |
    | --- | --- |
    | Department | Select the department for payments made under this bank account. |
    | Class | Select the class for payments made under this bank account. |
    | Location | Select the location for payments made under this bank account. |
    
    Note:
    
    For each category, you can set up to 50,000 classes, departments or locations. Setting up more than 50,000 for each category may slow down the loading of the dropdown list of categories.
    
5.  Complete the fields on the **EFT Template Details** subtab. The fields displayed are dependent on the EFT format selected.
    
    Important:
    
    When using the DTAUS format, the details you enter are automatically converted to capital characters to comply with bank specifications.
    
    Note:
    
    The **EFT Template Details** subtab isn't displayed if you did not select a value in the **EFT Template** field.
    
    | Field | Description |
    | --- | --- |
    | Bank Number (BLZ) | Enter the BLZ code of your company's bank. BLZ (Bankleitzahl) is a bank identifier numbering system used in Germany. |
    | Account Number/Bank Account Number | Enter your company's bank account number. |
    | IBAN | This field displays your company's International Bank Account Number (IBAN). This number is sourced from the values that you supplied in the Bank Number and Account Number fields. |
    | Company Name | Enter the name of your company. |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of your company's bank (eight or 11 characters). |
    | Bank Code | Enter the 8-digit identification code of your company's bank. |
    | Bank Street Address | Enter the street address of your company's bank. |
    | Bank City/Town Address | Enter the city or town address of your company's bank. |
    | Bank Account Name | Enter your company's bank account name. |
    | HSBC Connect Id | Enter your company's HSBC Connect Id. |
    | Country | Select the country where your company is located. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    
6.  Complete the fields on the **DD Template Details** subtab. The fields displayed are dependent on the DD format selected.
    
    Note:
    
    The **DD Template Details** subtab isn't displayed if you did not select a value in the **DD Template** field.
    
    | Field | Description |
    | --- | --- |
    | Bank Number (BLZ) | Enter the BLZ code of your company's bank. BLZ (Bankleitzahl) is a bank identifier numbering system used in Germany. |
    | Account Number | Enter your company's bank account number. You can provide separate bank accounts for payments and direct debit transactions. |
    | IBAN | This field displays your company's International Bank Account Number (IBAN). This number is sourced from the values that you supplied in the Bank Number and Account Number fields. |
    | Company Name | Enter the name of your company. |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of your company's bank (eight or 11 characters). |
    | Creditor Id | Enter your company's Creditor Identification number issued by your bank. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    
7.  If you want to create multiple payment batches for this bank account, complete the following fields on the **Batch Details** subtab.
    
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

-   [Setting Up Bank Records of Vendors in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1616705.html)
-   [Setting Up Bank Records of Employees in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617036.html)
-   [Setting Up Bank Records of Customers in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617359.html)
-   [Setting Up Bank Records of Partners in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851207772.html)
-   [Germany Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554985535.html)
-   [Germany Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554981475.html)
-   [Germany Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726737.html)
-   [Setting Up Germany-Specific Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726820.html)
-   [Germany-specific SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158529777788.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
