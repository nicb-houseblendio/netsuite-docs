---
id: "section_N1642399"
type: "section"
title: "Setting Up Bank Records of Customers in New Zealand"
branch: "new-zealand-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > New Zealand Help Topics > New Zealand Payment Formats > Setting Up Bank Records of Customers in New Zealand"
parent: "section_N1640223"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1642399.html"
anchors: ["procedure_N1642411"]
sha256: "5594c45dc870dce4b87e8de45a25a21b26bb26dc32c132800d0c671f84f69b36"
---

Set up the bank account details of each customer to whom you will send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for refund transactions: {#procedure_N1642411}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the selected EFT format.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **ANZ** to generate payment files for this customer in the format required by ANZ New Zealand. Select **ASB** to generate payment files for this customer in the format required by ASB Bank. Select **BNZ** to generate payment files for this customer in the format required by the Bank of New Zealand. Select **Westpac-DeskBank** to generate payment files for this vendor in the format required by Westpac Banking Corporation. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customer's bank account number (15 - 16 digits). |
    | Bank Account Name | Enter the customer's bank account name. |
    
    | Payment Description | Enter a maximum of 12 characters for the bank payment description to be displayed in the bank statement. |
    | --- | --- |
    | Payment Reference | Enter a maximum of 12 characters for the payment reference details to be displayed in the bank statement. |
    | Payment Code | Enter a maximum of 12 characters for the payment code to be displayed in the bank statement. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Bank Records of Partners in New Zealand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851237339.html)
-   [Setting Up Company Bank Records in New Zealand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1640758.html)
-   [Setting Up Bank Records of Vendors in New Zealand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1641714.html)
-   [Setting Up Bank Records of Employees in New Zealand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1642061.html)
-   [New Zealand Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1640223.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
