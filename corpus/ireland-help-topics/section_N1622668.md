---
id: "section_N1622668"
type: "section"
title: "Setting Up Bank Records of Customers in Ireland"
branch: "ireland-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Ireland Help Topics > Ireland-specific SuiteApps > Ireland Localization > Ireland Payment Formats > Setting Up Bank Records of Customers in Ireland"
parent: "section_157987018221"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1622668.html"
anchors: ["procedure_N1622808"]
sha256: "76087063670327a2972b007fe5e261f69f25a6c3b87c426c224188a5b09daf49"
---

Set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for refund transactions: {#procedure_N1622808}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Entity Bank Details**.
    
5.  Complete the fields on the New Entity Bank Details page. The fields displayed are dependent on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **BACS-Bank of Ireland** or **SEPA Credit Transfer**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Account Number | Enter the customer's 8-digit bank account number. |
    | Sort Code | Enter the 6-digit numeric sort code of the customer's bank. The code is used by the British banking industry to route money transfers within the country using different respective clearance organizations. |
    | IBAN | Enter the customer's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing entity bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1620470.html)
-   [Setting Up Bank Records of Vendors in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1621994.html)
-   [Setting Up Bank Records of Employees in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1622345.html)
-   [Setting Up Bank Records of Partners in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851215287.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
