---
id: "section_N1596031"
type: "section"
title: "Setting Up Company Bank Records in Australia"
branch: "australia-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Australia Help Topics > Australia Payment Formats > Setting Up Company Bank Records in Australia"
parent: "section_N1595666"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1596031.html"
anchors: ["procedure_N1596043"]
sha256: "478ac8015eb2ea4b7d0e7602b130ae967cceccb414bde8fee6a7c98f38043429"
---

Note:

For accurate validation and field sourcing, you must create company bank records from the Company Bank Details page. Don't use SuiteScript APIs or CSV Imports to create company bank records.

Set up the bank account records that your company or subsidiaries will be using to send and receive electronic bank payments.

#### To set up company bank details in Australia: {#procedure_N1596043}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the processed electronic bank payment transactions will be posted. Note: The **Subsidiary** and **Currency** fields are automatically filled when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If you don't see a GL bank account in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name to be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they're shown in the Bill Payment Batches list and the Bill Payments form. |
    | EFT Template | Select **ABA**. It's the standard payment file format used by Australian banks for electronic fund transfers. |
    | DD Template | Select **ABA DD**. It's the standard payment file format used by Australian banks for electronic fund transfers. |
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
    
    | Bank Code | Enter the 3-digit alphanumeric code that identifies your company's bank. |
    | --- | --- |
    | Bank Company ID | Enter the 6-digit code that identifies your company in the bank's records. This is assigned by the bank. |
    | BSB Number (Bank) | Enter the 3-digit code that identifies the bank. BSB numbers are codes that identify banks in Australia. |
    | BSB Number (Branch) | Enter the 3-digit numeric code that identifies the bank branch where your company's account is maintained. BSB numbers are codes that identify bank branches in Australia. |
    | Bank Account Number | Enter your company's 9-digit bank account number. |
    | Insert Balancing Line? | Check this box to include a contra record in the payment file that indicates the amount debited from your company's bank account. Check with your bank if this option is required for EFT transactions. |
    | Process Bills Automatically | Check this box if you want to process payment transactions for this bank account in batches. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html). Leave this box clear if you want to process payment transactions for this bank manually. For more information see, [Manually Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666511.html). |
    | Accounts Payable | Select the accounts payable register where the payments will be posted. |
    | Hide Transactions | Check this box if you want to hide the transaction lines on the Bill Payment Batches form when processing payments in batches. For more information, see [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html). Note: This feature is available if **Process Bills Automatically** is enabled or **Marked by Default** is enabled. |
    
6.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab.
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Inactive | Check this box to make a payment batch inactive. When you mark a record as inactive, it isn't shown in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the **Inactive** box for the main batch, bills that do not meet search criteria will not be included in the payment batch. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    
7.  Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
8.  Click **Save** to save the company bank details.
    

To set up approval routing for this bank account, see [Setting Up Approval Routing for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3824128426.html).

### Related Topics

-   [Setting Up Bank Records of Vendors in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1596975.html)
-   [Setting Up Bank Records of Employees in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1597374.html)
-   [Setting Up Bank Records of Customers in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1597766.html)
-   [Setting Up Bank Records of Partners in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851187027.html)
-   [Australia Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1595666.html)
-   [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html)
-   [Shipping Integration with Australia Post](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274389015.html)
-   [Australia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1832106.html)
-   [Setting Up Australia-specific Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540889422.html)
-   [Australia Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540887347.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
