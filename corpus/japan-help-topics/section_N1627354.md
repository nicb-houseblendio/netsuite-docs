---
id: "section_N1627354"
type: "section"
title: "Setting Up Company Bank Records in Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Payment Formats > Setting Up Company Bank Records in Japan"
parent: "section_N1627002"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1627354.html"
anchors: ["procedure_N1627366"]
sha256: "c277dd6844a72a10a76e261dbff01abfae2bfc66ed81c142d084818959a7a373"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. You shouldn't create company bank records by using SuiteScript APIs or CSV Imports.

Set up the bank account records of your company or its subsidiaries that you will be using to send electronic bank payments.

#### To set up company bank details in Japan: {#procedure_N1627366}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically generated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account isn't available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they are displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select **Zengin** or **Zengin XML**. Zengin is the standard payment file format used by Japanese banks for electronic fund transfers. Note: The Zengin text format can only be used until December 2020, after which, you must use the Zengin XML format. |
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
    
5.  Complete the fields on the **EFT Template Details** subtab.
    
    | Bank Number | Enter the number that identifies the bank in the Japanese banking industry. |
    | --- | --- |
    | Branch Number | Enter the number that identifies the bank branch where your account is maintained. |
    | Account Number | Enter your company's bank account number. |
    | EFT ID | Enter your company's EFT requester ID. This number is assigned by the bank. |
    | Bank Name | Enter the name of your company's bank. |
    | Branch Name | Enter the name of the bank branch where your company's account is maintained. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    
6.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Inactive | Check this box if you want to make a payment batch inactive. When you mark a record as inactive, it isn't displayed in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the **Inactive** box for the main batch, bills that don't meet search criteria won't be included in the payment batch. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    
7.  Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
8.  Click **Save** to save the company bank details.
    

If you want to set up approval routing for this bank account, see [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).

### Related Topics

-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)
-   [Support for Japan Zengin XML Payment Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547540023.html)
-   [Setting Up Bank Records of Vendors in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1628436.html)
-   [Setting Up Bank Records of Employees in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1628890.html)
-   [Setting Up Bank Records of Customers in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1629882.html)
-   [Setting Up Bank Records of Partners in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851223847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
