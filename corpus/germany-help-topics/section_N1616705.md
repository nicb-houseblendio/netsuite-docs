---
id: "section_N1616705"
type: "section"
title: "Setting Up Bank Records of Vendors in Germany"
branch: "germany-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Germany Help Topics > Germany-specific SuiteApps > Germany Localization > Germany Electronic Bank Payments > Setting Up Bank Records of Vendors in Germany"
parent: "section_1554985535"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1616705.html"
anchors: ["procedure_N1616717"]
sha256: "7e9163a56bef58094df06129266d77832223d9f4daad013dc4324dd2327aad3e"
---

Set up the bank account records of each vendor to whom you'll send electronic bank payments. You can set up multiple bank accounts for each vendor.

#### To set up vendor bank details in Germany: {#procedure_N1616717}

1.  Go to _Lists > Relationships > Vendors_.
    
    For information about adding a vendor, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
2.  Click the Edit link next to the name of the vendor.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box, and click **Save**.
    
4.  Click **New Entity Bank Details**.
    
5.  Complete the fields on the New Entity Bank Details page. The fields displayed are dependent on the EFT format selected. For specific formats, take note of the following:
    
    -   For the DTAZV format, the Bank Account Number and Country Code are disabled when you provide the IBAN.
        
    -   For the DTAUS format, the details you enter are automatically converted to capital characters when generating the payment file.
        
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select one of the following:
    -   **DTAUS**
    -   **DTAZV**
    -   **SEPA Credit Transfer (ABN AMRO)**
    -   **SEPA Credit Transfer (Austria)**
    -   **SEPA Credit Transfer (Germany)**
    -   **SEPA Credit Transfer (HSBC)**
    
     |
    | Type | Select whether the bank account is the vendor's primary or secondary bank account. |
    | Bank Number | Enter the bank number that identifies the vendor's bank in Germany. |
    | Account Number/Bank Account Number | Enter the vendor's bank account number. |
    | Bank Name | Enter the name of the vendor's bank. |
    | Payment Description | Enter text that will be displayed on the bank statement to help identify or describe payments to this vendor. |
    | IBAN | Enter the vendor's International Bank Account Number (IBAN). |
    | Company Country Code | Enter the international code assigned to the country where the bank is based. |
    | Transfer Fee Code | Enter the transfer fee code to identify who accepts responsibility for the transfer fees. Enter one of the following:
    
    -   **00** - Ordering fees are the payer's responsibility and third party fees are the payee's responsibility
    -   **01** - The payer is responsible for all fees
    -   **02** - The payee is responsible for all fees
    
     |
    | Bank BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the vendor's bank (eight or 11 characters). |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing entity bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Additional Information

-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)

### Related Topics

-   [Setting Up Company Bank Records in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1614550.html)
-   [Setting Up Bank Records of Employees in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617036.html)
-   [Setting Up Bank Records of Customers in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617359.html)
-   [Setting Up Bank Records of Partners in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851207772.html)
-   [Germany Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554985535.html)
-   [Germany Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554981475.html)
-   [Germany Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726737.html)
-   [Setting Up Germany-Specific Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726820.html)
-   [Germany-specific SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158529777788.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
