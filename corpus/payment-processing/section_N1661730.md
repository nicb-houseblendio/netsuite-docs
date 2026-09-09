---
id: "section_N1661730"
type: "section"
title: "Setting Up Company Bank Records for Positive Pay"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Payment File Formats > Global Payment Formats > Setting Up Company Bank Records for Positive Pay"
parent: "section_N1664266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1661730.html"
anchors: ["procedure_N1661761"]
sha256: "3bd462953824a03dce5c6ce26dc22e1444b1e7f4d1d6b944a6b61ad01061504e"
---

Note:

You must create company bank records from the Company Bank Details page for accurate validation and field sourcing. NetSuite doesn't recommend you to create company bank records by using SuiteScript APIs or CSV Imports.

You need to set up the bank details of your company to generate positive pay file formats.

#### To set up company bank records to use Positive Pay: {#procedure_N1661761}

1.  Go to Payments > Setup > Bank Details > New.
    
2.  Complete the fields on the New Company Bank Details page.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | GL Bank Account | Select the GL account where the issued checks to be included in the Positive Pay file format are posted. Note: The **Subsidiary** and **Currency** fields are automatically populated when a GL Bank Account is selected. Subsidiaries are only available in NetSuite OneWorld. If a GL bank account is not available in the dropdown list, go to _Setup > Accounting > Manage G/L > Chart of Accounts > New_ to create one. For more information, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html). |
    | Legal Name | Enter your company's legal name. This will be used in the electronic bank payment files. |
    | Print Company Name | Enter the company name that should appear on email notifications of payment transactions sent to vendors, employees, and customers. |
    | Marked by Default | Check this box if you want the payment transactions for this bank account automatically checked when they are displayed in the Bill Payment Batches list and the Bill Payments form. |
    | Positive Pay Template | Select **BoA/ML** if your bank uses the Positive Pay file format specifications of Bank of America Merrill Lynch. Select **RBC** if your bank uses the Positive Pay file format specifications of RBC Bank. Select **SVB-CDA** if your bank uses the Positive Pay file format specifications of Silicon Valley Bank for Controlled Disbursement Accounts. |
    | File Cabinet Location ID | Enter the Internal ID of the folder that you created for storing payment format files. For more information, see [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html). |
    | File Name Prefix | (Optional) Enter a prefix for the file number sequence. The prefix is attached to the beginning of each file number whenever this bank is used in creating a payment file. |
    
3.  Click **Save**. Complete the additional bank detail fields.
    
    | Field | Description |
    | --- | --- |
    | Department | Select the department for payments made under this bank account. |
    | Class | Select the class for payments made under this bank account. |
    | Location | Select the location for payments made under this bank account. |
    
    Note:
    
    For each category, you can set up to 50,000 classes, departments or locations. Setting up more than 50,000 for each category may slow down the loading of the dropdown list of categories.
    
4.  On the **Positive Pay Template Details** subtab, enter your company's bank account number.
    
    Note:
    
    Enter a 12-digit account number if your company uses the BoA/ML Positive Pay file format including leading zeroes if the account number has fewer than 12 digits. Enter a 10-digit account number if your company uses the RBC Positive Pay file format including leading zeroes if the account number has fewer than 10 digits.
    
5.  If you want to create multiple payment batches for this bank account, complete the fields on the **Batch Details** subtab:
    
    | Field | Description |
    | --- | --- |
    | Batch Details Name | Enter a name for the payment batch. |
    | Saved Search | Select the search criteria to group the bills and expenses that will be included in the payment batch. |
    | Payment Schedule | Select a payment schedule for when the payment batches should be automatically created and submitted for processing. To set up payment schedules, see [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html). You can leave this field blank and choose to manually trigger the system to create payment batches by clicking **Refresh Batch**. |
    | Email Recipient | Select the employee to whom a notification should be sent whenever payment batches are created per schedule. |
    | Inactive | Check this box if you want to make a payment batch inactive. When you mark a record as inactive, it is not displayed in lists and dropdown fields. However, the record remains in the system for future reference. Note: If you check the **Inactive** box for the main batch, bills that do not meet search criteria will not be included in the payment batch. |
    
6.  Click **Add** to save the payment batch. You can create more payment batches for the bank account.
    
7.  Click **Save** to save the company bank details.
    

### Related Topics

-   [Positive Pay Payment Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4127585994.html)
-   [Setting Up Company Bank Records in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1659433.html)
-   [Setting Up Bank Records of Vendors in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1660722.html)
-   [Setting Up Bank Records of Employees in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1661066.html)
-   [Setting Up Bank Records of Customers in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1661408.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
