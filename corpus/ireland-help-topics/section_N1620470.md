---
id: "section_N1620470"
type: "section"
title: "Setting Up Company Bank Records in Ireland"
branch: "ireland-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Ireland Help Topics > Ireland-specific SuiteApps > Ireland Localization > Ireland Payment Formats > Setting Up Company Bank Records in Ireland"
parent: "section_157987018221"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1620470.html"
anchors: ["procedure_N1620482"]
sha256: "ea9e8164833abdb733a117dbba030a7da8e4ce1b41f1845801bf4b014c54a758"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. You shouldn't create company bank records by using SuiteScript APIs or CSV Imports.

Set up bank account records that your company or subsidiaries will use to send and receive electronic bank payments.

#### To set up company bank details in Ireland: {#procedure_N1620482}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are filled automatically after you select a GL Bank Account. Subsidiaries are only available in NetSuite OneWorld. If there's no GL bank account available in the list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they're displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select **BACS-Bank of Ireland**, **SEPA Credit Transfer (HSBC)**, or **SEPA Credit Transfer (Bank of Ireland)**. |
    | File Cabinet Location ID | Enter the internal ID of the folder that you created for storing payment format files. For more information, see [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html). |
    | File Name Prefix | If the EFT file format for this record is SEPA Credit Transfer (Bank of Ireland), enter **PAIN001**. The use of this file name prefix is only required for SEPA Credit Transfer (Bank of Ireland). The prefix goes at the start of each file number whenever you use this bank to create a payment file. If the EFT file format is BACS-Bank of Ireland, the file name prefix is optional. |
    
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
    
    | Field | Description |
    | --- | --- |
    | Company Name | Enter your company's name. |
    | Identification Number | Enter your company's tax identification or other number assigned by an entity to identify your company. |
    | IBAN | Enter your company's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of your company's bank (eight or 11 characters). |
    | Sort Code | Enter the 6-digit numeric sort code of your bank branch. This code is used by the British banking industry to route money transfers within the country using different clearance organizations. |
    | Account Number | Enter your company's 8-digit bank account number. |
    | Authorized ID No. | Enter your company's 6-digit, alphanumeric issuer number. This number is assigned by the bank. |
    | HSBC Connect Id | Enter your company's HSBC Connect Id. |
    | Country | Select the country where your company is located. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if Process Bills Automatically is enabled or Marked by Default is enabled. |
    
6.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Inactive | Check this box if you want to make a payment batch inactive. When you mark a record as inactive, it's not displayed in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the Inactive box for the main batch, bills that don't meet search criteria won't be included in the payment batch. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    
7.  Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
8.  Click **Save** to save the company bank details.
    

If you want to set up approval routing for this bank account, see [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).

### Related Topics

-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)
-   [Setting Up Bank Records of Vendors in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1621994.html)
-   [Setting Up Bank Records of Employees in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1622345.html)
-   [Setting Up Bank Records of Customers in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1622668.html)
-   [Setting Up Bank Records of Partners in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851215287.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
