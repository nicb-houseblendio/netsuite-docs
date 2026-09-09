---
id: "section_N1647643"
type: "section"
title: "Setting Up Bank Records of Customers in Singapore"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Payment Formats > Setting Up Bank Records of Customers in Singapore"
parent: "section_N1642722"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647643.html"
anchors: ["procedure_3851123366", "procedure_N1647902"]
sha256: "a6bab344f67c512d5d0d0dd9820e73512cad33226ec4ecd0cca37d92fa6868d3"
---

Set up the bank account details of each customer from whom you will receive direct debit payments and to whom you will send refund payments. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for direct debit transactions: {#procedure_3851123366}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer from whom you want to receive direct debit payments.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the selected DD Template. The following table lists the common fields displayed, you may disregard those that are not displayed.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | DD Template | Select any of the following Direct Debit (DD) payment file formats to use when receiving payments from this customer:
    -   **DBS-IDEAL DD**
    -   **UoB - BIB-IBG DD**.
    
    DBS - IDEAL is the standard payment file format used by Singapore banks for direct deposit transactions. UoB - BIB-IBG is included in the nationwide electronic payment platform in Singapore. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customer's bank account number. |
    | Bank Account Name | Enter the customer's bank account name. |
    | Bank Number | Enter the 4-digit numeric code that identifies the customer's bank. |
    | Branch Number | Enter the 3-digit numeric code that identifies the bank branch where the customer's account is maintained. |
    | Bank Account Payment Description | Enter text that will be displayed on the bank statement to help identify or describe payments from this customer. |
    | Reference | Enter additional text that will be displayed on the bank statement to help identify or describe payments from this customer. |
    
6.  Click **Save**.
    

#### To set up bank details of a customer for refund transactions: {#procedure_N1647902}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the selected Payment File Format. The following table lists the common fields displayed, you may disregard those that are not displayed.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | EFT Template | Select any of the following Electronic Fund Transfer (EFT) payment file formats to use when sending payments to this customer:
    -   **DBS Singapore Ideal 3.0 Universal File Format Domestic Transfer**
    -   **DBS Singapore Ideal 3.0 Universal File Format International Transfer**
    -   **DBS - IDEAL specifications of DBS Bank Limited**
    -   **UoB - BIB-IBG specifications of United Overseas Bank Limited**
    -   **ISO 20022 of HSBC**
    
    Note: To use international transfer payment formats, you must have an active license for advanced Electronic Bank Payments and you must install the NetSuite SuiteApps License Client SuiteApp in your account. With active license for advanced Electronic Bank Payments, domestic and cross-border templates are available and you can edit the template as needed. If you use the free version of Electronic Bank Payments, only domestic templates are available and you can't edit the template, but you can edit the PFA output file. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Account Name/Bank Account Name | Enter the customer's bank account name. |
    | Bank Number/Bank Code | Enter the 4-digit numeric code that identifies the customer's bank. |
    | Branch Number/Branch Code | Enter the 3-digit numeric code that identifies the branch where the customer's account is maintained. |
    | Account Number/Bank Account Number | Enter the customer's bank account number.
    
    -   For DBS Singapore Ideal 3.0 Universal File Format Domestic Transfer - maximum of 34 digits
    -   For DBS Singapore Ideal 3.0 Universal File Format International Transfer - maximum of 34 digits
    -   For DBS - IDEAL - 11 digits
    -   For UoB - BIB-IBG - 11 digits
    -   For HSBC ISO 20022 - 7-12 digits
    
     |
    | Bank Name | Enter the name of the customer's bank. |
    | Street Name | Enter the street name of the customer's address. |
    | Building Number | Enter the building number of the customer's address. |
    | Post Code | Enter the post code of the customer's address. |
    | Town Name | Enter the town name of the customer's address. |
    | Country Subdivision | Enter the country subdivision of the customer's address. |
    | Address Line | Enter any additional details of the customer's address. |
    | Purpose Code | Enter the Purpose Code that specifies the reason for the payment. Note: Refer to your bank's website for the list of Purpose Codes. |
    | Charge Bearer | Select who will pay the charges for processing the payment transaction:
    
    -   "DEBT" - Debtor will pay all charges
    -   "CRED" - Creditor will pay all charges
    -   "SHAR" - Debtor and Creditor will pay their own charges
    
     |
    | Service Level | Enter the bank's supported electronic fund transfer service type. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Setting Up Company Bank Records in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1645419.html)
-   [Setting Up Bank Records of Vendors in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1646764.html)
-   [Setting Up Bank Records of Employees in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647136.html)
-   [Setting Up Bank Records of Partners in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851239814.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
