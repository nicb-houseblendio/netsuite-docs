---
id: "section_N1948426"
type: "section"
title: "Norway Tax Codes"
branch: "norway-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Norway Help Topics > Norway Tax Topics For Accounts Without SuiteTax > Norway Tax Codes"
parent: "section_157926586299"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1948426.html"
anchors: ["subsect_1030033313", "bridgehead_N1948485", "subsect_163593735944"]
sha256: "5ea5651e349ac894b8c52a4d0a9af6c859045e361eac87d7503366a99fee507a"
---

Note:

This topic is for VAT reports generated from the Tax Reports (International) page. If you are using the Country Tax Report page, see [Norway Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159005737735.html).

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Norway are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030033313}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Norway {#bridgehead_N1948485}

The following table shows the tax properties required to correctly generate the Norway VAT reports provided by the International Tax Reports SuiteApp or Norway Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

These tax codes are valid until December 31, 2021. Starting Jan 1, 2022, use the tax codes listed in the 2022 tax code table in your transactions. See [2022 Tax Code Table for Norway](#subsect_163593735944).

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-NO | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| I-NO | Imports | Import | 25% | \- | Both (Sales and Purchases) |
| IS-NO | Import of service items | Import Applies to Service Items | 25% | \- | Both (Sales and Purchases) |
| IV-NO | Import VAT - goods | Import Reverse Charge Code | 0% | I-NO | Purchases |
| IVR1-NO | Import of goods - reduced rate | Reverse charge Import Reduced rate | 0% | R1-NO | Purchases |
| IVS-NO | Import VAT - services | Import Reverse Charge Code Applies to Service Items | 0% | IS-NO | Purchases |
| IZ-NO | Import of goods - zero rate | Import | 0% | \- | Purchases |
| O-NO | Outside of scope | Non Taxable | 0% | \- | Both (Sales and Purchases) |
| R1-NO | Reduced rate | Reduced Rate | 15% | \- | Both (Sales and Purchases) |
| R2-NO | Super reduced rate | Special Reduced Rate | 12% | \- | Both (Sales and Purchases) |
| RC-NO | Reverse charge - domestic | Reverse charge | \- | S-NO | Both (Sales and Purchases) |
| S-NO | Standard rate | \- | 25% | \- | Both (Sales and Purchases) |
| X-NO | Export | Export | 0% | \- | Sales |
| Z-NO | Zero rated supplies | \- | 0% | \- | Sales |

## 2022 Tax Code Table for Norway {#subsect_163593735944}

Effective January 1, 2022, all transactions for the new Norway digital VAT report will use the following tax codes and properties. Any changes in the tax code properties may cause incorrect reporting in your VAT report.

Note:

The International Tax Reports SuiteApp maintains the tax code provisioning for Norway whereas the Norway Tax Reports SuiteApp supports the new Norway eVAT reporting beginning year 2022. For more information, see [Norway Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159005737735.html).

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| 0\_NO | No VAT treatment (acquisitions) | Exempt Exclude in VAT report | 0% | \- | Purchases |
| 1\_NO | Input VAT deductible (domestic) Regular rate | \- | 25% | \- | Purchases |
| 11\_NO | Input VAT deductible (domestic) Reduced rate, middle | Reduced Rate | 15% | \- | Purchases |
| 12\_NO | Input VAT deductible (domestic) Reduced rate, raw fish | Special Reduced Rate | 11.11% | \- | Purchases |
| 13\_NO | Input VAT deductible (domestic) Reduced rate, low | Special Reduced Rate | 12% | \- | Purchases |
| 14\_NO | Input VAT deductible (payed on import) Regular rate | Import | 25% | \- | Purchases |
| 15\_NO | Input VAT deductible (payed on import) Reduced rate, middle | Import Reduced Rate | 15% | \- | Purchases |
| 3\_NO | Output VAT Regular rate | \- | 25% | \- | Sales |
| 31\_NO | Output VAT Reduced rate, middle | Reduced Rate | 15% | \- | Sales |
| 32\_NO | Output VAT Reduced rate, raw fish | Special Reduced Rate | 11.11% | \- | Sales |
| 33\_NO | Output VAT Reduced rate, low | Special Reduced Rate | 12% | \- | Sales |
| 5\_NO | No output VAT Zero rate | \- | 0% | \- | Sales |
| 51\_NO | Domestic sales of reverse charge /VAT obligation Zero rate | Reverse Charge Code | 0% | 3\_NO (25%) | Sales |
| 52\_NO | Export of goods and services Zero rate | Export | 0% | \- | Sales |
| 6\_NO | Not liable to VAT treatment, turnover outside the scope of the VAT legislation | Non Taxable | 0% | \- | Sales |
| 7\_NO | No VAT treatment - no turnover according to the VAT legislation (sales) | Exempt Exclude in VAT report | 0% | \- | Sales |
| 81\_NO | Importation of goods, VAT deductible Regular rate | Reverse Charge Code Import | 0% | 1\_NO (25%) | Purchases |
| 82\_NO | Importation of goods, without deduction of VAT Regular rate | Reverse Charge Code Import Effective From: January 1, 2022 | 0% | 1\_NO (25%) | Purchases |
| 83\_NO | Importation of goods, VAT deductible Reduced rate, middle | Reverse Charge Code Import Reduced Rate | 0% | 15\_NO (15%) | Purchases |
| 84\_NO | Importation of goods, without deduction of VAT Reduced rate, middle | Reverse Charge Code Import Reduced Rate Effective From: January 1, 2022 | 0% | 15\_NO (15%) | Purchases |
| 85\_NO | Importation of goods, not applicable for VAT-Zero rate | Import | 0% | \- | Purchases |
| 86\_NO | Services purchased from abroad, VAT deductible Regular rate | Reverse Charge Code Applies To Services Import | 0% | 1\_NO (25%) | Purchases |
| 87\_NO | Services purchased from abroad, without deduction of VAT Regular rate | Reverse Charge Code Applies To Services Import Effective From: January 1, 2022 | 0% | 1\_NO (25%) | Purchases |
| 88\_NO | Services purchased from abroad, VAT deductible Reduced rate, low | Reverse Charge Code Applies To Services Import Special Reduced Rate | 0% | 13\_NO (12%) | Purchases |
| 89\_NO | Services purchased from abroad, without deduction of VAT Reduced rate, low | Reverse Charge Code Applies To Services Import Special Reduced Rate Effective From: January 1, 2022 | 0% | 13\_NO (12%) | Purchases |
| 91\_NO | Purchase of emissions trading or gold, VAT deductible Regular rate | Reverse Charge Code | 0% | 1\_NO (25%) | Purchases |
| 92\_NO | Purchase of emissions trading or gold, without deduction of VAT Regular rate | Reverse Charge Code Effective From: January 1, 2022 | 0% | 1\_NO (25%) | Purchases |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Norway VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1949157.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Norway Standard Audit File for Tax (SAF-T) Financial](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_43132133850.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
