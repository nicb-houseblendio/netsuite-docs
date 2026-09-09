---
id: "section_N1628436"
type: "section"
title: "Setting Up Bank Records of Vendors in Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Payment Formats > Setting Up Bank Records of Vendors in Japan"
parent: "section_N1627002"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1628436.html"
anchors: ["procedure_N1628448"]
sha256: "afa62de5cdb80135440e92df5b4d67102b1162aef7edb3367595b42d46fce4ec"
---

Set up the bank account records of each vendor to whom you will send electronic bank payments. You can set up multiple bank accounts for each vendor.

#### To set up vendor bank details in Japan: {#procedure_N1628448}

1.  Go to _Lists > Relationships > Vendors_.
    
    For information about adding a vendor, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
2.  Click the Edit link next to the name of the vendor.
    
3.  On the **Bank Payment Details** subtab, check the **EFT Bill Payment** box, and click **Save**.
    
4.  Click **New Bank Details**.
    
5.  Complete the fields on the Bank Details page:
    
    | Field | Description |
    | --- | --- |
    | Name | Enter a name for the bank record. |
    | Payment File Format | Select **Zengin** or **Zengin XML**. Zengin is the standard payment file format used by Japanese banks for electronic fund transfers. Note: The Zengin text format can only be used until December 2020, after which, you must use the Zengin XML format. |
    | Type | Select whether the bank account is the vendor's primary or secondary bank account. |
    | Bank Number | Enter the number that identifies the vendor's bank. |
    | Branch Number | Enter the number that identifies the vendor's bank branch. |
    | Bank Account Number | Enter the vendor's bank account number. |
    | Bank Account Name | Enter the vendor's bank account name. |
    | Bank Name | Enter the name of the vendor's bank. |
    | Branch Name | Enter the name of the bank branch where the vendor's account is maintained. |
    | Account Type | Select whether the vendor's bank account is an ordinary or checking account. |
    
6.  Click **Save**.
    

You can also set up bank records of vendors, employees, customers and partners by importing bank details in CSV format into NetSuite using the Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html).

### Related Topics

-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Support for Japan Zengin XML Payment Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547540023.html)
-   [Setting Up Company Bank Records in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1627354.html)
-   [Setting Up Bank Records of Employees in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1628890.html)
-   [Setting Up Bank Records of Customers in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1629882.html)
-   [Setting Up Bank Records of Partners in Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851223847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
