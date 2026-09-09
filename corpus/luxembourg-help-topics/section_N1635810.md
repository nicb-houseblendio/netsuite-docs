---
id: "section_N1635810"
type: "section"
title: "Setting Up Bank Records of Customers in Luxembourg"
branch: "luxembourg-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Luxembourg Help Topics > Luxembourg Payment Formats > Setting Up Bank Records of Customers in Luxembourg"
parent: "section_156864104822"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1635810.html"
anchors: ["procedure_N1635822"]
sha256: "885708249d5f7970eebd168f305ae9f1aaa6250d98621038f5adf479caba8724"
---

Set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for refund transactions: {#procedure_N1635822}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed depend on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **ABBL VIR 2000**, **SEPA Credit Transfer (HSBC)**, or **SEPA Credit Transfer (Luxembourg)**. |
    | Type | Select whether the bank account is your customer's primary or secondary bank account. |
    | IBAN | Enter the customer's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in Luxembourg](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1630676.html)
-   [Setting Up Bank Records of Vendors in Luxembourg](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1635095.html)
-   [Setting Up Bank Records of Employees in Luxembourg](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1635453.html)
-   [Setting Up Bank Records of Partners in Luxembourg](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851227075.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
