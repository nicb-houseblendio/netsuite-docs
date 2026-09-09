---
id: "section_N1629882"
type: "section"
title: "Setting Up Bank Records of Customers in Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Payment Formats > Setting Up Bank Records of Customers in Japan"
parent: "section_N1627002"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1629882.html"
anchors: ["procedure_N1629894"]
sha256: "a005ad18226da0f96c2f2f40166dad410388082c7a3e73434be7b145c44fa569"
---

Set up the bank account details of each customer to whom you will send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for refund transactions: {#procedure_N1629894}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | Payment File Format | Select **Zengin** or **Zengin XML**. Zengin is the standard payment file format used by Japanese banks for electronic fund transfers. Note: The Zengin text format can only be used until December 2020, after which, you must use the Zengin XML format. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Bank Account Number | Enter the customer's bank account number. This number shouldn't exceed seven characters. |
    | Bank Account Name | Enter the customer's bank account name. |
    | Bank Number | Enter the 4-digit number that identifies the customer's bank. |
    | Bank Name | Enter the name of the customer's bank. |
    | Branch Number | Enter the 3-digit number that identifies the bank branch where the customer's account is maintained. |
    | Branch Name | Enter the name of the branch. |
    | Account Type | Select whether the customer's bank account is an ordinary or checking account. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Support for Japan Zengin XML Payment Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547540023.html)
-   [Setting Up Company Bank Records in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1627354.html)
-   [Setting Up Bank Records of Vendors in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1628436.html)
-   [Setting Up Bank Records of Customers in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1629882.html)
-   [Setting Up Bank Records of Partners in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851223847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
