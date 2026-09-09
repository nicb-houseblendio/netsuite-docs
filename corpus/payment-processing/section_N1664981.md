---
id: "section_N1664981"
type: "section"
title: "Setting Up Bank Records of Customers for J.P. Morgan Freeform GMT Payments"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Payment File Formats > Global Payment Formats > J.P. Morgan Freeform GMT Payment Format > Setting Up Bank Records of Customers for J.P. Morgan Freeform GMT Payments"
parent: "section_4122407314"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1664981.html"
anchors: ["procedure_N1665003"]
sha256: "b0efb6a6b3e89884d14155ecae47c38053baca743878c00969ef8ce10e9f13a0"
---

Set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for refund transactions for J.P. Morgan Freeform GMT payments: {#procedure_N1665003}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Entity Bank Details**.
    
5.  Complete the fields on the New Entity Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **J.P. Morgan Freeform GMT**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Account Number | Enter the customer's bank account number. |
    | Swift ID/BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the customer's bank (eight or 11 characters). |
    | Bank Name | Enter the name of the customer's bank. |
    | Bank Address 1 | Enter the street address of the customer's bank. |
    | Bank Address 2 | Enter the city or state where the customer's bank is located. |
    | IBAN | Required if country is Lebanon or Saudi Arabia. Enter the customer's International Bank Account Number (IBAN). |
    
6.  Click **Save**.
    

### Related Topics

-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)
-   [Setting Up Company Bank Records for J.P. Morgan Freeform GMT Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1664376.html)
-   [Setting Up Bank Records of Vendors for J.P. Morgan Freeform GMT Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1664682.html)
-   [Setting Up Bank Records of Employees for J.P. Morgan Freeform GMT Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1664834.html)
-   [Setting up Bank Records of Partners for J.P. Morgan Freeform GMT Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3854647220.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
