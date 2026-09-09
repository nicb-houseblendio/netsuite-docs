---
id: "section_N1626422"
type: "section"
title: "Setting Up Bank Records of Customers in Italy"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Payment File Formats > Payment Formats for Countries > Italy Payment Formats > Setting Up Bank Records of Customers in Italy"
parent: "section_N1623115"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1626422.html"
anchors: ["procedure_N1626434", "procedure_N1626686"]
sha256: "0789a99c23ff3ab11bced572f4ce4dc6943129f15a0192d41c673ec927fdf67d"
---

Set up the bank account details of each customer from whom you will receive direct debit payments. You also need to set up the bank account details of each customer to whom you will send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for direct debit transactions: {#procedure_N1626434}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer from whom you want to receive direct debit payments.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the Direct Debit format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **SEPA Direct Debit (CBI)** or **CBI Collections** as the type of file that will be generated for this customer. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Remittance Message | Enter a short message to show in your customer's bank statement every time a direct debit is initiated. |
    | Reference Mandate | Enter the authorization identification or mandate. This information must be supplied by the customer. |
    | IBAN | Enter the customer's International Bank Account Number (IBAN). |
    | Electronic Signature | Enter a digital code or signature for mandates generated electronically. |
    | Issuer | Enter the name of the entity that issued the customer's tax ID. |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    | Billing Sequence Type | This indicates the billing sequence for this mandate. Select one of the following:
    -   **FRST** - This is the first collection of a series of direct debit instructions
    -   **RCUR** - The mandate instructions are used for regular recurrent direct debits
    -   **FNAL** - This is the final collection of a series of direct debits
    -   **OOFF** - The mandate is used only for a single direct debit
    
    Note: Select **FRST** if Original Debtor Agent is selected in the Reference Amended field. |
    | Date of Reference Mandate | Enter the date the mandate was signed by the customer. |
    | Reference Amended | This indicates whether the authorization or mandate was amended or changed since it was originally issued. Select one of the following:
    
    -   **No Changes** - There were no modifications made on the original mandate
    -   **Original Mandate Identification** - The original mandate identification was modified
    -   **Original Debtor Account** - Your customer changed his bank account number
    -   **Original Debtor Agent** - Your customer transferred to another bank
    -   **Original Creditor ID** - Your Creditor ID or company name has been modified after the mandate was issued
    
     |
    | Company Id | Enter the customer's tax identification, or other identification number assigned by an entity. |
    | Original Reference Mandate | Enter the original mandate identification. |
    | Original Debtor's IBAN | Enter the customer's previous IBAN. |
    | Original Creditor ID | Enter your company's previous Creditor ID. |
    | Original Creditor Name | Enter your company's previous company name. |
    
6.  Click **Save**.
    

#### To set up bank details of a customer for refund transactions: {#procedure_N1626686}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **SEPA Credit Transfer (CBI)**, **SEPA Credit Transfer (HSBC)**, or **CBI Payments**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | IBAN | Enter the customer's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    | Issuer | Enter the name of the entity that issued the customer's tax Id. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1623480.html)
-   [Setting Up Bank Records of Employees in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1626074.html)
-   [Setting Up Bank Records of Vendors in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1625724.html)
-   [Setting Up Bank Records of Partners in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851217587.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
