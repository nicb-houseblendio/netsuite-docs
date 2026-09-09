---
id: "section_N1597766"
type: "section"
title: "Setting Up Bank Records of Customers in Australia"
branch: "australia-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Australia Help Topics > Australia Payment Formats > Setting Up Bank Records of Customers in Australia"
parent: "section_N1595666"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1597766.html"
anchors: ["procedure_3903097201", "procedure_N1597778"]
sha256: "f25af4a943e6b7f66cd51720d9187b96a9cc5740a4ea23216a5eea9fd83c2ada"
---

Set up the bank account details of each customer from whom you'll receive direct debit payments. Set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for direct debit transactions: {#procedure_3903097201}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit link next to the name of the customer from whom you want to receive direct debit payments.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **ABA DD**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customer's bank account number. |
    | Bank Account Name | Enter the customer's bank account name. |
    | Bank Number | Enter the 3-digit code that identifies the customer's bank. |
    | Branch Number | Enter the 3-digit code that identifies the bank branch where the customer's account is maintained. |
    | Bank Account Payment Description | Enter text that should be displayed in the customer's bank statement. |
    
6.  Click **Save**.
    

#### To set up bank details of a customer for refund transactions: {#procedure_N1597778}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **ABA**. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customers bank account number. |
    | Bank Account Name | Enter the customer's bank account name. |
    | Bank Number | Enter the 3-digit code that identifies the customer's bank. |
    | Branch Number | Enter the 3-digit code that identifies the bank branch where the customer's account is maintained. |
    | Bank Account Payment Description | Enter text that should be displayed in the customer's bank statement. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1596031.html)
-   [Setting Up Bank Records of Vendors in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1596975.html)
-   [Setting Up Bank Records of Employees in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1597374.html)
-   [Setting Up Bank Records of Partners in Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851187027.html)
-   [Australia Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1595666.html)
-   [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html)
-   [Shipping Integration with Australia Post](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274389015.html)
-   [Australia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1832106.html)
-   [Setting Up Australia-specific Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540889422.html)
-   [Australia Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540887347.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
