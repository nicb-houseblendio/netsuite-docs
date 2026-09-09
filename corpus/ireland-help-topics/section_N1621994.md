---
id: "section_N1621994"
type: "section"
title: "Setting Up Bank Records of Vendors in Ireland"
branch: "ireland-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Ireland Help Topics > Ireland-specific SuiteApps > Ireland Localization > Ireland Payment Formats > Setting Up Bank Records of Vendors in Ireland"
parent: "section_157987018221"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1621994.html"
anchors: ["procedure_N1622006"]
sha256: "89dc225d7620a1eb65fc6aa43ee3b9364786441f7322e4c90927773f6eb2b50e"
---

Set up the bank account records of each vendor to whom you'll send electronic bank payments. You can set up multiple bank accounts for each vendor.

#### To set up vendor bank details in Ireland: {#procedure_N1622006}

1.  Go to _Lists > Relationships > Vendors_.
    
    For information about adding a vendor, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
2.  Click the Edit link next to the name of the vendor.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the New Bank Details page. The fields displayed are dependent on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **BACS-Bank of Ireland**, **SEPA Credit Transfer (HSBC)**, or **SEPA Credit Transfer (Bank of Ireland)**. |
    | Type | Select whether the bank account is the vendor's primary or secondary bank account. |
    | Sort Code | Enter the 6-digit numeric sort code of the vendor's bank. The code is used by the British banking industry to route money transfers within the country using different respective clearance organizations. |
    | Account Number | Enter the vendor's 8-digit bank account number. |
    | IBAN | Enter the vendor's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the vendor's bank (eight or 11 characters). |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Setting Up Company Bank Records in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1620470.html)
-   [Setting Up Bank Records of Employees in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1622345.html)
-   [Setting Up Bank Records of Customers in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1622668.html)
-   [Setting Up Bank Records of Partners in Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851215287.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
