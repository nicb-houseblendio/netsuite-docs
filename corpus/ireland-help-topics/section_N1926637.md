---
id: "section_N1926637"
type: "section"
title: "Ireland Tax Codes"
branch: "ireland-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Ireland Help Topics > Ireland Tax Topics For Accounts Without SuiteTax > Ireland Tax Codes"
parent: "section_157985984564"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1926637.html"
anchors: ["subsect_1030023434", "bridgehead_N1926696", "subsect_159720247229"]
sha256: "e8d7a870be1b83e22ec6ae384d0de20fc5ad62b582379ccebcd4738fca683000"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Ireland are set up correctly.

For more information on tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030023434}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Ireland {#bridgehead_N1926696}

The following table shows the tax properties required to correctly generate the Ireland tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Ireland VAT reports, see [What goes into each box - Ireland VAT 3 report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1929852.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates. The standard rate in Ireland increased to 23%, effective January 1, 2012.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-IE | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| EE-IE | Exempt tax code for intra-community transactions | Effective from January 1, 2021 EC Code Exempt | 0% | E-IE | Both (Sales and Purchases) |
| EFR-IE | Flat-rate compensation percentage for farmers (intra-community) | Effective from January 1, 2021 EC Code | 0% | FR-IE | Both (Sales and Purchases) |
| ELR-IE | Livestock rate for intra-community transactions | Effective from January 1, 2021 EC Code | 0% | LR-IE | Both (Sales and Purchases) |
| ER-IE | EU sales/purchases - reduced rate (goods) | EC Code Reduced Rate | 0% | R-IE | Both (Sales and Purchases) |
| ES-IE | EU sales/purchases (goods) | EC Code | 0% | S-IE | Both (Sales and Purchases) |
| ESPR-IE | EU purchases - reduced rate (services) | EC Code Reverse Charge Reduced Rate Applies to Service Items | 0% | R-IE | Purchases |
| ESR-IE | EC sales/purchases to another EC country - second reduced rate | EC Code Special Reduced Rate | 0% | SR-IE | Both (Sales and Purchases) |
| ESSP-IE | EU purchases (services) Note: This tax code is applicable to intra-community purchase transaction. | EC Code Reverse Charge Code Applies to Service Items | 0% | S-IE | Purchases |
| ESSS-IE | EU sales (services) Note: This tax code is applicable to intra-community sales transaction. | Export EC Code Applies to Service Items | 0% | S-IE | Sales |
| EZ-IE | Zero rated sales tax code for intra-community transactions | Effective from January 1, 2021 EC Code | 0% | Z-IE | Both (Sales and Purchases) |
| FR-IE | Flat-rate compensation percentage for farmers | Effective from January 1, 2021 | 5.6% | \- | Both (Sales and Purchases) |
| I-IE | Purchase of goods from outside of EU | Import | 23% | \- | Purchases |
| IPA1-IE | Postponed import VAT on goods purchased from Great Britain and non-EU countries | Effective from January 1, 2021 Reverse Charge Code Import | 0% | S-IE | Purchases |
| IPA2-IE | Postponed import VAT on goods purchased from Great Britain and non-EU countries | Effective from January 1, 2021 Reverse Charge Code Reduced Rate Import | 0% | R-IE | Purchases |
| IPA3-IE | Postponed import VAT on goods purchased from Great Britain and non-EU countries | Effective from January 1, 2021 Reverse Charge Code Special Reduced Rate Import | 0% | SR-IE | Purchases |
| IPA4-IE | Postponed import VAT on goods purchased from Great Britain and non-EU countries | Effective from January 1, 2021 Reverse Charge Code Import | 0% | Z-IE | Purchases |
| IS-IE | Purchase of services from outside of EU | Import Reverse Charge Code Applies to Service Items | 0% | S-IE | Purchases |
| LR-IE | Livestock rate | Effective from January 1, 2021 | 4.8% | \- | Both (Sales and Purchases) |
| O-IE | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-IE | Supply of services outside of EU | Reverse Charge Code Export Applies to Service Items | 0% | S-IE | Sales |
| R-IE | Reduced rate | Reduced Rate | 13.5% | \- | Both (Sales and Purchases) |
| RC-IE | Reverse charge sales in country | Reverse Charge Code | 0% | S-IE | Sales |
| S-IE | Standard rate | \- | 23% | \- | Both (Sales and Purchases) |
| SR-IE | Second reduced rate | Special Reduced Rate | 9% | \- | Both (Sales and Purchases) |
| Z-IE | Zero rated sales (home, in country) |  | 0% | \- | Sales |

### Temporary Tax Codes for Ireland COVID-19 Tax Response {#subsect_159720247229}

In response to the COVID-19 tax relief measure, temporary tax codes with reduced rates are effective on September 1, 2020 until February 28, 2021. The International Tax Reports SuiteApp provisions the following tax codes to accounts with Ireland nexus:

| Tax Code | Description | Rate | Effective From | Property | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- | --- |
| S1-IE | Standard rate at 21% from September 1, 2020 to February 28, 2021 | 21% | September 1, 2020 |  |  | Both (Sales and Purchases) |
| RC1-IE | Reverse charge sales in country from September 1, 2020 to February 28, 2021 | 0% | September 1, 2020 | Reverse Charge Code | S1-IE | Both (Sales and Purchases) |
| I1-IE | Purchase of goods from outside of EC from September 1, 2020 to February 28, 2021 | 21% | September 1, 2020 | Import |  | Both (Sales and Purchases) |
| IS1-IE | Purchase of services from outside of EC from September 1, 2020 to February 28, 2021 | 0% | September 1, 2020 | Reverse Charge Code Applies to Service Items Import | S1-IE | Both (Sales and Purchases) |
| ES1-IE | EC sales/purchases to another EC country (goods) from September 1, 2020 to February 28, 2021 | 0% | September 1, 2020 | EC Code | S1-IE | Both (Sales and Purchases) |
| ESSP1-IE | EC purchases (services) from outside of EC from September 1, 2020 to February 28, 2021 Note: This tax code is applicable to intra-community purchase transaction. | 0% | September 1, 2020 | EC Code Reverse Charge Code Applies to Service Items | S1-IE | Both (Sales and Purchases) |
| ESSS1-IE | EC Sales (services) from outside of EC from September 1, 2020 to February 28, 2021 Note: This tax code is applicable to intra-community sales transaction. | 0% | September 1, 2020 | EC Code Applies to Service Items | S1-IE | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Setting Up Tax Filing for Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1929131.html)
-   [Ireland VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1929434.html)
-   [What goes into each box - Ireland VAT 3 report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1929852.html)
-   [EU Sales List for Ireland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1931683.html)
-   [What goes into each box - Ireland Return of Trading Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1930183.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
