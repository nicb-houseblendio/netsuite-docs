---
id: "section_N1918921"
type: "section"
title: "Indonesia Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Indonesia Tax Topics > Indonesia Tax Codes"
parent: "chapter_N1918792"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1918921.html"
anchors: ["subsect_1030023032", "bridgehead_N1918980"]
sha256: "47a5cd2abf1420a951386a4bc186be211836d0dce6c7b218d26aeaae07fd0f89"
---

Tax codes determine how much tax is paid on each transaction line item. To make sure NetSuite calculates the correct values on transaction records and tax reports, ensure the tax codes for Indonesia are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030023032}

-   The International Tax Reports SuiteApp supports up to 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes per country if they aren't used in the same tax period.
    

## Tax Code Table for Indonesia {#bridgehead_N1918980}

The following table lists the tax properties needed to generate Indonesia VAT reports with the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes if you'd like.

Tax reports identify transactions based on tax code properties, not tax code names. On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the VAT Declaration Form 1111 and Form 1111AB, see [What goes into each box - Indonesia VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1920183.html).

Note:

Effective April 1, 2022, the VAT rate for Indonesia increased to 11%.

| Tax Code | Description | Rate | Property | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- |
| EX-ID | Delivery of taxable goods and services exempt from VAT (VAT Invoice Transaction Code 08) | 11% | Exempt | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| G-ID | Delivery of taxable goods and services to designated VAT collectors or VAT withholding agents (VAT Invoice Transaction Code 02 and 03) | 11% | Government | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| IMPT-ID | Importation of goods, consumption of foreign intangible goods, and services outside the customs area where input VAT cannot be credited | 11% | Import | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| NC-ID | Imports or acquisitions where input VAT cannot be credited | 11% | No Tax Credit | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| NV-ID | Delivery of taxable goods and services where VAT was not collected (VAT Invoice Transaction Code 07) | 11% | No Tax Invoice | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| S-ID | Standard rate (VAT Invoice Transaction Code 01, 04, 06 and 09) | 11% | Default | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| UNDEF\_ID | Used when NetSuite cannot determine the appropriate tax code for a transaction | 0% | Exclude from VAT Reports | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |
| Z-ID | Zero rated | 0% | Export | PPN on Purchases ID | PPN on Sales ID | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Indonesia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1919850.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
