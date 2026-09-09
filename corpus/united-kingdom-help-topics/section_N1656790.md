---
id: "section_N1656790"
type: "section"
title: "Setting Up Company Bank Records in the United Kingdom"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom-specific SuiteApps > United Kingdom Localization > United Kingdom Payment Formats > Setting Up Company Bank Records in the United Kingdom"
parent: "section_156922746724"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1656790.html"
anchors: ["procedure_N1656802"]
sha256: "f556c62517b429131731d673df0b41920e4cb25a2d2d912a1c18ee1b2fd16700"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. You shouldn't create company bank records by using SuiteScript APIs or CSV Imports.

Set up the bank account records that your company or subsidiaries will be using to send and receive electronic bank payments.

#### Setting up company bank details in the United Kingdom: {#procedure_N1656802}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically generated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account isn't available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they are displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select the ETF payment template of your choice. For more information, see [United Kingdom Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156922746724.html). |
    | DD Template | Select the DD payment template of your choice. For more information, see [United Kingdom Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156922746724.html). |
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
    
5.  Complete the fields on the **EFT Template Details** subtab. The fields displayed depend on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | HSBC/SAGE | Enter HSBC or SAGE if there is no Service User Number (SUN) assigned by the bank. |
    | Service User Number | Enter your company's 6-digit Service User Number (SUN). This number is assigned by the bank. |
    | Sort Code | Enter the 6-digit numeric sort code of your bank branch. This code is used by the British banking industry to route money transfers within the country using different clearance organizations. |
    | Account Number | Enter your company's 8-digit bank account number. |
    | Include Total Debit Amount | Check this box to include the total debit amount in the UTL1 record of the payment file. Otherwise, a default value of zero is assigned. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    
6.  Complete the fields on the **DD Template Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | HSBC/SAGE | Enter HSBC or SAGE if there is no Service User Number (SUN) assigned by the bank. |
    | Service User Number | Enter your company's 6-digit Service User Number (SUN). This number is assigned by the bank. |
    | Sort Code | Enter the 6-digit numeric sort code of your bank branch. This code is used by the British banking industry to route money transfers within the country using different clearance organizations. |
    | Account Number | Enter your company's 8-digit bank account number. |
    
7.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Inactive | Check this box if you want to make a payment batch inactive. When you mark a record as inactive, it isn't displayed in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the **Inactive** box for the main batch, bills that don't meet search criteria won't be included in the payment batch. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    
8.  Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
9.  Click **Save** to save the company bank details.
    

If you want to set up approval routing for this bank account, see [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).

### Related Topics

-   [Setting Up Bank Records of Vendors in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1657779.html)
-   [Setting Up Bank Records of Employees in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658141.html)
-   [Setting Up Bank Records of Customers in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658474.html)
-   [Setting Up Bank Records of Partners in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851248105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
