---
id: "section_N1658474"
type: "section"
title: "Setting Up Bank Records of Customers in the United Kingdom"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom-specific SuiteApps > United Kingdom Localization > United Kingdom Payment Formats > Setting Up Bank Records of Customers in the United Kingdom"
parent: "section_156922746724"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658474.html"
anchors: ["procedure_N1658486", "procedure_N1658733"]
sha256: "ea31030824e4c712cd7541772e4ff7b79d089d3bc3717c2a45b015b4d94f9f64"
---

Set up the bank account details of each customer from whom you'll receive direct debit payments. You also need to set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### Setting up bank details of a customer for direct debit transactions: {#procedure_N1658486}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click Edit next to the name of the customer from whom you want to receive direct debit payments.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** b ox, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed depend on the DD format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this bank detail record. |
    | Payment File Format | Select **BACS DD** if the customer's bank uses the original variation of the BACS payment file format specification of BACS Payment Schemes Limited. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Account Number | Enter the customer's 8-digit bank account number. |
    | Account Name | Enter the customer's bank account name. |
    | Sort Code | Enter the 6-digit numeric sort code of the customer's bank. The code is used by the British banking industry to route money transfers within the country using different respective clearance organizations. |
    
6.  Click **Save**.
    

#### Setting up bank details of a customer for refund transactions: {#procedure_N1658733}

1.  Go to _Lists > Relationships > Customers_.
    
2.  Click Edit next to the name of the customer to whom you want to send refund payments. For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed depend on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this bank detail record. |
    | Payment File Format | Select **SEPA Credit Transfer (HSBC)** or **BACS** if the employee's bank uses the original variation of the BACS payment file format specification of BACS Payment Schemes Limited. Select **BACS-Albany ALBACS-IP** if the employee's bank uses the variation of the BACS payment file format specification of Albany ePAY Bureau, Barclays Bank, and (BACS Multiple Fixed Length) Lloyds Bank. Select **BACS-Bank of Scotland** if the employee's bank is a branch of Bank of Scotland PLC (BoS). BoS uses a variation of the BACS format where the file headers and footers are omitted. Select **BACSTEL-IP** if the customer's bank uses the internet service variation of BACS. |
    | Type | Select whether the bank account is the customer's primary or secondary bank account. |
    | Account Number | Enter the customer's 8-digit bank account number. |
    | Account Name | Enter the customer's bank account name of the customer. |
    | Sort Code | Enter the 6-digit numeric sort code of the customer's bank. The code is used by the British banking industry to route money transfers within the country using different respective clearance organizations. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1656790.html)
-   [Setting Up Bank Records of Vendors in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1657779.html)
-   [Setting Up Bank Records of Employees in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658141.html)
-   [Setting Up Bank Records of Partners in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851248105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
