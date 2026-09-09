---
id: "section_N1595275"
type: "section"
title: "Setting Up Bank Records of Customers in Austria"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Payment File Formats > Payment Formats for Countries > Austria Payment Formats > Setting Up Bank Records of Customers in Austria"
parent: "section_N1592839"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1595275.html"
anchors: ["procedure_N1595287"]
sha256: "451761bac15aeff5a1f2271e619aae341e85dae6f697a5102ad449da810e1fcb"
---

Set up the bank account details of each customer where customer refunds are sent. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for refund transactions: {#procedure_N1595287}

1.  Go to _Lists > Relationships > Customers_.
    
    For information on creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **SEPA Credit Transfer (Austria)** or **SEPA Credit Transfer (HSBC)**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | IBAN | Enter the customer's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html)
-   [Setting Up Company Bank Records in Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1593207.html)
-   [Setting Up Bank Records of Vendors in Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1594516.html)
-   [Setting Up Bank Records of Employees in Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1594900.html)
-   [Setting Up Bank Records of Partners in Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851092659.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
