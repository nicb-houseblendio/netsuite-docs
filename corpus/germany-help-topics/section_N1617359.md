---
id: "section_N1617359"
type: "section"
title: "Setting Up Bank Records of Customers in Germany"
branch: "germany-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Germany Help Topics > Germany-specific SuiteApps > Germany Localization > Germany Electronic Bank Payments > Setting Up Bank Records of Customers in Germany"
parent: "section_1554985535"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617359.html"
anchors: ["procedure_N1617371", "procedure_N1617618"]
sha256: "25fe2430d286e7502580464fa10f23a1eb530a68ac5f65e67e4f897979d44778"
---

Set up the bank account details of each customer from whom you'll receive direct debit payments. You also need to set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for direct debit transactions: {#procedure_N1617371}

1.  Go to _Lists > Relationships > Customers_.
    
    To create a new customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer from whom you want to receive direct debit payments.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** box, and click **Save**.
    
4.  Click **New Entity Bank Details**.
    
5.  Complete the fields on the New Entity Bank Details page. The fields displayed are dependent on the DD format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select one of the following:
    -   **DTAUS DD**
    -   **SEPA Direct Debit (Germany)**
    
     |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customer's bank account number. |
    | Bank Number | Enter the bank number that identifies the customer's bank in Germany. |
    | Original Debtor IBAN | The customer's previous IBAN. |
    | Original Creditor Name | Your company's previous company name. |
    | Original Creditor ID | Your company's previous Creditor ID. |
    | Remittance Message | Enter a short message to show in your customer's bank statement every time a direct debit is initiated. |
    | Reference Mandate | Enter the authorization identification or mandate. This information must be supplied by the customer. |
    | IBAN | This field displays the customer's International Bank Account Number (IBAN) based on the values that you entered in the Bank Account Number and Bank Number fields. |
    | Electronic Signature | Enter a digital code or signature for mandates generated electronically. |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    | Original Reference Mandate | The original mandate identification. |
    | Billing Sequence Type | This indicates the billing sequence for this mandate. Select one of the following:
    
    -   **FRST** - This is the first collection of a series of direct debit instructions.
    -   **RCUR** - The mandate instructions are used for regular recurrent direct debits.
    -   **FNAL** - This is the final collection of a series of direct debits.
    -   **OOFF** - The mandate is used only for a single direct debit.
    
    Note: Select **FRST** if Original Debtor Agent is selected in the Reference Amended field. |
    | Date or Reference Mandate | Enter the date the mandate was signed by the customer. |
    | Reference Amended | This indicates whether the authorization or mandate was amended or changed since it was originally issued. Select one of the following:
    
    -   **No Changes** - There were no modifications made on the original mandate
    -   **Original Mandate Identification** - The original mandate identification was modified.
    -   **Original Debtor Account** - Your customer changed his bank account number.
    -   **Original Debtor Agent** - Your customer transferred to another bank.
    -   **Original Creditor ID** - Your Creditor Id or company name has been modified after the mandate was issued.
    
     |
    
6.  Click **Save**.
    

#### To set up bank details of a customer for refund transactions: {#procedure_N1617618}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
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
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customer's bank account number. |
    | Bank Number | Enter the bank number that identifies the customer's bank in Germany. |
    | Bank Name | Enter the name of the customer's bank. |
    | Payment Description | Enter text that will be displayed on the bank statement to help identify or describe payments to this customer. |
    | IBAN | Enter the customer's International Bank Account Number (IBAN). |
    | Company Country Code | Enter the international code for the country where the bank is based. |
    | Transfer Fee Code | Enter the transfer fee code to identify who accepts responsibility for the transfer fees. Enter one of the following:
    
    -   **00** - Ordering fees are the payer's responsibility and third party fees are the payee's responsibility
    -   **01** - The payer is responsible for all fees
    -   **02** - The payee is responsible for all fees
    
     |
    | Bank BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing entity bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Additional Information

-   [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html)

### Related Topics

-   [Setting Up Company Bank Records in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1614550.html)
-   [Setting Up Bank Records of Vendors in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1616705.html)
-   [Setting Up Bank Records of Employees in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617036.html)
-   [Setting Up Bank Records of Partners in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851207772.html)
-   [Germany Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554985535.html)
-   [Germany Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554981475.html)
-   [Germany Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726737.html)
-   [Setting Up Germany-Specific Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726820.html)
-   [Germany-specific SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158529777788.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
