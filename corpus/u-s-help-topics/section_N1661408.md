---
id: "section_N1661408"
type: "section"
title: "Setting Up Bank Records of Customers in the U.S."
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > U.S. Payment Formats > Setting Up Bank Records of Customers in the U.S."
parent: "section_N1659055"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1661408.html"
anchors: ["procedure_3727378958", "procedure_N1661420"]
sha256: "0a18d668b77d08516aa216b605e471622b8d6f04b72cf107561a117e65859533"
---

Set up the bank account details of each customer from whom you will receive direct debit payments. You also need to set up the bank account details of each customer to whom you will send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for direct debit transactions: {#procedure_3727378958}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about adding customer records, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** box, and click **Save**.
    
4.  Click **New Bank Details.**
    
5.  Complete the fields on the Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this bank detail record. |
    | Payment File Format | Select **ACH-PPD**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the 10-digit number that identifies the customer's account in the bank that will receive the payment. |
    | Bank Number | Enter the 9-digit routing number that identifies the customer's bank. |
    
6.  Click **Save**.
    

#### To set up bank details of a customer for refund transactions: {#procedure_N1661420}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this bank detail record. |
    | Payment File Format | Select either **ACH-CCD/PPD** or **ACH-CTX (Free Text)**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter up to 17 digits for the entity's bank account number. |
    | Bank Number | Enter the 9-digit routing number that identifies the customer's bank. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1659433.html)
-   [Setting Up Bank Records of Vendors in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1660722.html)
-   [Setting Up Bank Records of Employees in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1661066.html)
-   [Setting Up Bank Records of Partners in the U.S.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851250354.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
