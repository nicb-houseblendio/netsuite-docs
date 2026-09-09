---
id: "section_N1646764"
type: "section"
title: "Setting Up Bank Records of Vendors in Singapore"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Payment Formats > Setting Up Bank Records of Vendors in Singapore"
parent: "section_N1642722"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1646764.html"
anchors: ["procedure_N1646776"]
sha256: "c24954ae85ef3c0fe5a3da178a26baea1df155e7795a3be300420111b4118ec8"
---

Set up the bank account records of each vendor to whom you will send electronic bank payments. You can set up multiple bank accounts for each vendor.

#### To set up vendor bank details in Singapore: {#procedure_N1646776}

1.  Go to _Lists > Relationships > Vendors_.
    
    For information about adding a vendor, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
2.  Click the Edit link next to the name of the vendor with a Singapore subsidiary.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the selected Payment File Format. The following table lists the common fields displayed, you may disregard those that are not displayed.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | EFT Template | Select any of the following Electronic Fund Transfer (EFT) payment file formats to use when sending payments to the vendor:
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
    | Type | Select whether the bank account is the vendor's primary or secondary bank account. |
    | Account Number/Bank Account Number | Enter the vendor's bank account number.
    
    -   For DBS Singapore Ideal 3.0 Universal File Format Domestic Transfer - maximum of 34 digits
    -   For DBS Singapore Ideal 3.0 Universal File Format International Transfer - maximum of 34 digits
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
    -   For Beneficiaries who are using HSBC, OCBC or State Bank of India Accounts, the 3-Digit Bank Code is added to the Beneficiary Account Number as a prefix.
    
     |
    | Account Name/Bank Account Name | Enter the vendor's bank account name. |
    | Bank Number/Bank Code | The 4-digit number that identifies the vendor's bank. |
    | Branch Number/Branch Code | Enter the 3-digit number that identifies the bank branch where the vendor's account is maintained. |
    | Bank Name | Enter the name of the vendor's bank. |
    | Street Name | Enter the street name of the vendor's address. |
    | Building Number | Enter the building number of the vendor's address. |
    | Post Code | Enter the post code of the vendor's address. |
    | Town Name | Enter the town name of the vendor's address. |
    | Country Subdivision | Enter the country subdivision of the vendor's address. |
    | Address Line | Enter any additional details of the vendor's address. |
    | Purpose Code | Enter the Purpose Code that specifies the reason for the payment. Note: Refer to your bank's website for the list of Purpose Codes. |
    | Charge Bearer | Select who will pay the charges for processing the payment transaction.
    
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
-   [Setting Up Bank Records of Employees in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647136.html)
-   [Setting Up Bank Records of Customers in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647643.html)
-   [Setting Up Bank Records of Partners in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851239814.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
