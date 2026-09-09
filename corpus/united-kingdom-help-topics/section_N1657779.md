---
id: "section_N1657779"
type: "section"
title: "Setting Up Bank Records of Vendors in the United Kingdom"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom-specific SuiteApps > United Kingdom Localization > United Kingdom Payment Formats > Setting Up Bank Records of Vendors in the United Kingdom"
parent: "section_156922746724"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1657779.html"
anchors: ["procedure_N1657791"]
sha256: "b432d59e57619011ae3f4d56ff03930e0e57b747b6a89018df243e7618fafc8a"
---

Set up the bank account records of each vendor to whom you'll send electronic bank payments. You can set up multiple bank accounts for each vendor.

#### Setting up vendor bank details in the United Kingdom: {#procedure_N1657791}

1.  Go to _Lists > Relationships > Vendors_.
    
    For information about adding a vendor, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
2.  Click the Edit link next to the name of the vendor.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed depend on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this bank detail record. |
    | Payment File Format | Select **SEPA Credit Transfer (HSBC)** or **BACS** if the vendor's bank uses the original variation of the BACS payment file format specification of BACS Payment Schemes Limited. Select **BACS-Albany ALBACS-IP** if the vendor's bank uses the variation of the BACS payment file format specification of Albany ePAY Bureau, Barclays Bank, and (BACS Multiple Fixed Length) Lloyds Bank. Select **BACS-Bank of Scotland** if the vendor's bank is a branch of Bank of Scotland PLC (BoS). BoS uses a variation of the BACS format where the file headers and footers are omitted. Select **BACSTEL-IP** if the vendor's bank uses the internet service variation of BACS. |
    | Type | Select whether the bank account is the vendor's primary or secondary bank account. |
    | Sort Code | Enter the 6-digit numeric sort code of the vendor's bank. The code is used by the British banking industry to route money transfers within the country using different respective clearance organizations. |
    | Account Number | Enter the vendor's 8-digit bank account number. |
    | Account Name | Enter the vendor's bank account name. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Setting Up Company Bank Records in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1656790.html)
-   [Setting Up Bank Records of Employees in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658141.html)
-   [Setting Up Bank Records of Customers in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1658474.html)
-   [Setting Up Bank Records of Partners in the United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851248105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
