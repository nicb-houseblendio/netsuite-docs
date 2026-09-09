---
id: "section_N1658141"
type: "section"
title: "Setting Up Bank Records of Employees in the United Kingdom"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom-specific SuiteApps > United Kingdom Localization > United Kingdom Payment Formats > Setting Up Bank Records of Employees in the United Kingdom"
parent: "section_156922746724"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658141.html"
anchors: ["procedure_N1658153"]
sha256: "50e5f96fe6c5b9d17ff54e6c5eca2ffd440784522e4e3ebaf06584b8537a95e9"
---

Set up the bank account details of each employee to whom you'll send electronic bank payments. You can set up multiple bank accounts for each employee.

#### Setting up employee bank details in the United Kingdom: {#procedure_N1658153}

1.  Go to _Lists > Employees > Employees_.
    
    To create a new employee record, see [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html).
    
2.  Click the Edit link next to the name of the employee.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box and then click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields that are displayed depend on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this bank detail record. |
    | Payment File Format | Select **SEPA Credit Transfer (HSBC)** or **BACS** if the employee's bank uses the original variation of the BACS payment file format specification of BACS Payment Schemes Limited. Select **BACS-Albany ALBACS-IP** if the employee's bank uses the variation of the BACS payment file format specification of Albany ePAY Bureau, Barclays Bank, and (BACS Multiple Fixed Length) Lloyds Bank. Select **BACS-Bank of Scotland** if the employee's bank is a branch of Bank of Scotland PLC (BoS). BoS uses a variation of the BACS format where the file headers and footers are omitted. Select **BACSTEL-IP** if the employee's bank uses the internet service variation of BACS. |
    | Type | Select whether the bank account is the employee's primary or secondary bank account. |
    | Sort Code | Enter the 6-digit numeric sort code of the employee's bank. The code is used by the British banking industry to route money transfers within the country using different respective clearance organizations. |
    | Account Number | Enter the employee's 8-digit bank account number. |
    | Account Name | Enter the employee's bank account name. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1656790.html)
-   [Setting Up Bank Records of Vendors in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1657779.html)
-   [Setting Up Bank Records of Customers in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658474.html)
-   [Setting Up Bank Records of Partners in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851248105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
