---
id: "section_N1609094"
type: "section"
title: "Setting Up Company Bank Records in Canada"
branch: "canada-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Canada Help Topics > Canada Payment Formats > Setting Up Company Bank Records in Canada"
parent: "section_156941355409"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1609094.html"
anchors: ["procedure_N1609106"]
sha256: "daababcb514aa091cf9b3cfa30732b1933d06e4572eddc76b58b81c1f78bc349"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. You should not create company bank records by using SuiteScript APIs or CSV Imports.

Set up the bank account records that your company or subsidiaries will be using to send and receive electronic bank payments.

#### To set up company bank details in Canada: {#procedure_N1609106}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically generated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account isn't available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they are displayed in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select **CPA-005**. |
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
    
    | Field | Description |
    | --- | --- |
    | Financial Institution Number | Enter the number that identifies the bank in the Financial Institutions Directory, which is maintained by the Canadian Payment Association. |
    | Branch Transit Number | Enter the routing number of the bank branch where your company's account is maintained. Bank branch routing numbers of Canadian financial institutions are listed in the Financial Institutions Directory of the Canadian Payment Association. |
    | Account Number | Enter your company's bank account number (maximum of 12 digits). |
    | Client Number | Enter the 10-digit number that identifies your company as a client of the bank. The first six numbers is assigned by the bank and the last 4 numbers is assigned by your company and can be used to indicate a subsidiary or division. |
    | Data Center | Enter the number of the bank processing center where the payment file will be processed. This information should be provided by the bank. |
    | Statement Name | Enter a name for electronic bank payment transactions made with this bank. |
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
-   [Setting Up Bank Records of Vendors in Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1610148.html)
-   [Setting Up Bank Records of Employees in Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1610495.html)
-   [Setting Up Bank Records of Customers in Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1610834.html)
-   [Setting Up Bank Records of Partners in Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851201197.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
