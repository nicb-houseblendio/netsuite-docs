---
id: "section_N1625724"
type: "section"
title: "Setting Up Bank Records of Vendors in Italy"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Payment File Formats > Payment Formats for Countries > Italy Payment Formats > Setting Up Bank Records of Vendors in Italy"
parent: "section_N1623115"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1625724.html"
anchors: ["procedure_N1625736"]
sha256: "dedb7f661287f2cf5b47fbb7d05898a25df803be0a09938da1b224c2835712d5"
---

Set up the bank account records of each vendor to whom you will send electronic bank payments. You can set up multiple bank accounts for each vendor.

#### To set up vendor bank details in Italy: {#procedure_N1625736}

1.  Go to _Lists > Relationships > Vendors_.
    
    For information about adding a vendor, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
2.  Click the Edit link next to the name of the vendor.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page. The fields displayed are dependent on the EFT format selected.
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a unique name for this entity bank detail record. |
    | Payment File Format | Select **CBI Payments** or **SEPA Credit Transfer (CBI)**. |
    | Type | Select whether the bank account is the vendor's primary or secondary bank account. |
    | IBAN | Enter the vendor's International Bank Account Number (IBAN). |
    | BIC | Enter the Business Identifier Code (BIC), also called SWIFT code, of the vendor's bank (eight or 11 characters). |
    | Issuer | Enter the name of the entity that issued the vendor's tax Id. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Setting Up Company Bank Records in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1623480.html)
-   [Setting Up Bank Records of Employees in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1626074.html)
-   [Setting Up Bank Records of Customers in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1626422.html)
-   [Setting Up Bank Records of Partners in Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851217587.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
