---
id: "section_N1645419"
type: "section"
title: "Setting Up Company Bank Records in Singapore"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Payment Formats > Setting Up Company Bank Records in Singapore"
parent: "section_N1642722"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1645419.html"
anchors: ["procedure_N1645431"]
sha256: "646d1846fb21fd99debad0b27c31060146777749e7483a8bbf57e67794e9430f"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. You should not create company bank records by using SuiteScript APIs or CSV Imports.

Set up the bank account records that your company or subsidiaries will be using to send and receive electronic bank payments.

#### To set up company bank details in Singapore: {#procedure_N1645431}

1.  Go to Payments > Setup > Company Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically generated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account is not available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they are displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select any of the following Electronic Fund Transfer (EFT) payment file formats to use when making payments through this bank:
    -   **DBS Singapore Ideal 3.0 Universal File Format Domestic Transfer**
    -   **DBS Singapore Ideal 3.0 Universal File Format International Transfer**
    -   **DBS - IDEAL specifications of DBS Bank Limited**
    -   **UoB - BIB-IBG specifications of United Overseas Bank Limited**
    -   **ISO 20022 of HSBC**
    -   **Citibank Singapore XML Domestic Transfer**
    -   **Citibank Singapore XML International Transfer**
    -   **Citibank Singapore XML GIRO**
    -   **HSBC Singapore pain.001.001.03 Low and High Value Domestic Payments**
    -   **JP Morgan Singapore pain.001.001.03 Low and High Value Domestic Payments**
    -   **OCBC Singapore GIRO and FAST Payments**
    -   **Standard Chartered Bank Singapore iPayment CSV GIRO and Domestic Payments**
    -   **UOB Singapore pain.001.001.03 GIRO, FAST and Domestic Payments**
    
    Note: To use international transfer payment formats, you must have an active license for advanced Electronic Bank Payments and you must install the NetSuite SuiteApps License Client SuiteApp in your account. With active license for advanced Electronic Bank Payments, domestic and cross-border templates are available and you can edit the template as needed. If you use the free version of Electronic Bank Payments, only domestic templates are available and you can't edit the template, but you can edit the PFA output file. |
    | DD Template | Select any of the following Direct Debit (DD) payment file formats to use when receiving payments through this bank:
    
    -   **DBS-IDEAL DD**
    -   **UoB - BIB-IBG DD**
    
     |
    | File Cabinet Location ID | Enter the internal ID of the folder that you created for storing payment format files. For more information, see [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html). |
    | File Name Prefix | (Optional) Enter a prefix for the file number sequence. The prefix is attached to the beginning of each file number whenever this bank is used in creating a payment file. |
    
3.  Click **Save**.
    
4.  Complete the additional bank detail fields.
    
    | Field | Description |
    | --- | --- |
    | Department | Select the department for payments made under this bank account. |
    | Class | Select the class for payments made under this bank account. |
    | Location | Select the location for payments made under this bank account. |
    
    Note:
    
    For each category, you can set up to 50,000 classes, departments or locations. Setting up more than 50,000 for each category may slow down the loading of the dropdown list of categories.
    
5.  Complete the fields on the **EFT Template Details (Bank Template Name)** subtab. The fields displayed are dependent on the selected EFT Template. The following table lists the common fields displayed, you may disregard those that are not displayed.
    
    Note:
    
    The **EFT Template Details** subtab is not displayed if you didn't select a value in the **EFT Template** field.
    
    | Field | Description |
    | --- | --- |
    | Account Number/Bank Account Number | Enter your company's bank account number.
    -   For DBS Singapore Ideal 3.0 Universal File Format Domestic Transfer - maximum of 35 digits
    -   For DBS Singapore Ideal 3.0 Universal File Format International Transfer - maximum of 35 digits
    -   For DBS - IDEAL - 11 digits
    -   For UoB - BIB-IBG - 11 digits
    -   For HSBC ISO 20022 - 7-12 digits
    -   For Citibank Singapore XML Domestic Transfer - maximum of 34 digits
    -   For Citibank Singapore XML International Transfer - maximum of 34 digits
    -   For Citibank Singapore XML GIRO - maximum of 34 digits
    -   For HSBC Singapore pain.001.001.03 Low and High Value Domestic Payments - maximum of 34 digits
    -   For JP Morgan Singapore pain.001.001.03 Low and High Value Domestic Payments - maximum of 34 digits
    -   For OCBC Singapore GIRO and FAST Payments - maximum of 34 digits
    -   For Standard Chartered Bank Singapore iPayment CSV GIRO and Domestic Payments - maximum of 34 digits
    -   For UOB Singapore pain.001.001.03 GIRO, FAST and Domestic Payments - maximum of 34 digits
    
     |
    | Authorization Code | (For HSBC ISO 20022) Enter the authorization code for your payment files, as provided by the bank. Acceptable values include **AUTH**, **FSUM**, and **FDET**. |
    | Sender's Company ID | Enter the 8-digit number that the bank uses to identify your company. |
    | Bank Number/Bank Code | Enter the 4-digit identification code of your company's bank. |
    | Customer/EFT ID | (For HSBC ISO 20022) Enter your company's HSBC Connect ID. |
    | Country | Select the country where your company's bank is located. |
    | Swift/BIC Code | Enter the Business Identifier Code (BIC), also called SWIFT code, of your company's bank. |
    | Branch Number | Enter the identification code of the bank branch where your company's account is maintained (maximum of 3 digits). |
    | Sender's Name | Enter your company's legal name. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    | Address | Enter the address of your company's bank; either structured (Street, Building Number, Postcode, Town, Country SubDivision, Country) or unstructured address, which must exist in the bank's Ordering Party Library. |
    
6.  Complete the fields on the **DD Template Details** subtab. The fields displayed are dependent on the DD format selected. The following table lists the common fields displayed, you may disregard those that are not displayed.
    
    Note:
    
    The **DD Template Details** subtab is not displayed if you didn't select a value in the DD Template field.
    
    | Field | Description |
    | --- | --- |
    | Bank Number | Enter the number that identifies the company's bank. |
    | Branch Number | Enter the number that identifies the bank branch where your company's account is maintained. |
    | Bank Account Number | Enter your company's bank account number. |
    | Sender's Company ID | Enter the 8-digit number that the bank uses to identify your company. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    
7.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Inactive | Check this box if you want to make a payment batch inactive. When you mark a record as inactive, it is not displayed in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the **Inactive** box for the main batch, bills that don't meet search criteria will not be included in the payment batch. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    
    Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
8.  Click **Save** to save the company bank details.
    

If you want to set up approval routing for this bank account, see [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).

### Related Topics

-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)
-   [Setting Up Bank Records of Vendors in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1646764.html)
-   [Setting Up Bank Records of Customers in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647643.html)
-   [Setting Up Bank Records of Employees in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647136.html)
-   [Setting Up Bank Records of Partners in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851239814.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
