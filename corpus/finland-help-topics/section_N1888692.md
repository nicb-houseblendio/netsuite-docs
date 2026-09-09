---
id: "section_N1888692"
type: "section"
title: "Finland Tax Codes"
branch: "finland-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Finland Help Topics > Finland Tax Topics > Finland Tax Codes"
parent: "section_157858109755"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1888692.html"
anchors: ["subsect_1030020848", "bridgehead_N1888751"]
sha256: "c01a87fff044ceb54a008de2681fe5e0c4b54244892f50a88c962f1ac5e2ba25"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Finland are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030020848}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Finland {#bridgehead_N1888751}

The following table shows the tax properties required to enable NetSuite to correctly generate the Finland tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| ES-FI | EU sales/purchases (goods) | EC Code | 0% | S-FI | Both (Sales and Purchases) |
| ESSP-FI | EU purchases (services) | EC Code Reverse Charge Code Applies to Service Items | 0% | S-FI | Purchases |
| ESSS-FI | EU sales (services) | EC Code Applies to Service Items | 0% | S-FI | Sales |
| EZ-FI | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-FI | Both (Sales and Purchases) |
| IV-FI | 100% VAT bill | Import VAT | 0% | \- | Purchases |
| R1-FI | Reduced rate | Reduced | 14% | \- | Both (Sales and Purchases) |
| R2-FI | Special reduced rate | Special Reduced Rate | 10% | \- | Both (Sales and Purchases) |
| RC-FI | Reverse charge in country | Reverse Charge Code | 0% | \- | Both (Sales and Purchases) |
| RCF-FI | Reverse charge purchase outside EU | Import Reverse Charge Code | 0% | S-FI | Purchases |
| RCF1-FI | Reverse charge purchase outside EU | Import Reverse Charge Code Reduced Rate | 0% | R1-FI | Purchases |
| RCF2-FI | Reverse charge purchase outside EU | Import Reverse Charge Code Special Reduced Rate | 0% | R2-FI | Purchases |
| RCIS1-FI | Reverse charge for import of services from outside EU (standard rate) | Effective from January 1, 2020 Reverse Charge Code Applies to Service Items Import | 0% | S-FI | Purchases |
| RCIS2-FI | Reverse charge for import of services from outside EU (reduced rate) | Effective from January 1, 2020 Reverse Charge Code Applies to Service Items Import Reduced Rate | 0% | R1-FI | Purchases |
| RCIS3-FI | Reverse charge for import of services from outside EU (special reduced rate) | Effective from January 1, 2020 Reverse Charge Code Applies to Service Items Import Special Reduced Rate | 0% | R2-FI | Purchases |
| S-FI | Standard rate | Effective from September 1, 2024 | 25.5% | \- | Both (Sales and Purchases) |
| Z-FI | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Finland VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1889688.html)
-   [EU Sales List for Finland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1889930.html)
-   [Intrastat Report for Finland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504769975.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
