---
id: "section_N1890308"
type: "section"
title: "France Tax Codes"
branch: "france-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > France Help Topics > France Tax Topics For Accounts Without SuiteTax > France Tax Codes"
parent: "section_1557736092"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1890308.html"
anchors: ["subsect_1030021217", "bridgehead_N1890366"]
sha256: "905f4240eff881fe01f161ad10e60e0a9051bd67bf06851775134dbe66746cef"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for France are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030021217}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for France {#bridgehead_N1890366}

The following table shows the tax properties required to correctly generate the France VAT report provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the France TVA Form, see [What goes into each box - France VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1892495.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| DTY-FR | Duty free purchases | Category: Duty Free | 0% |  | Purchases |
| E-FR | Exempt or Non Taxable | Exempt |  |  | Both (Sales and Purchases) |
| ER-FR | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate |  | R-FR | Both (Sales and Purchases) |
| ES-FR | EU sales/purchases (goods) | EC Code |  | S-FR | Both (Sales and Purchases) |
| ESR-FR | EU sales/purchases (goods) - special reduced rate | EC Code Special Reduced Rate |  | SR-FR | Both (Sales and Purchases) |
| ESSP-FR | EU purchases (services) | EC Code Applies to Service Items Reverse Charge |  | S-FR | Purchases |
| ESSS-FR | EU sales (services) | EC Code Applies to Service Items |  | S-FR | Sales |
| EZ-FR | EU sales/purchases (goods) - zero rate | EC Code |  | 0% | Both (Sales and Purchases) |
| FA-FR | Property regarded as fixed assets | Category: Fixed Assets | 20% |  | Purchases |
| GAZ-FR | Gas and electricity | Category: Gas & Electricity | 20% |  | Both (Sales and Purchases) |
| I-FR | Purchase of goods from outside of EU | Import |  |  | Purchases |
| IPA1-FR | Postponed import VAT on goods purchased from Great Britain and non-EU countries - standard rate 20% | Effective from January 1, 2022 Reverse Charge Code Import VAT | 0% | ­S-FR | Purchases |
| IPA2-FR | Postponed import VAT on goods purchased from Great Britain and non-EU countries - special reduced rate 10% | Effective from January 1, 2022 Reverse Charge Code Import VAT | 0% | SR-FR | Purchases |
| IPA3-FR | Postponed import VAT on goods purchased from Great Britain and non-EU countries - special territory 8.5% | Effective from January 1, 2022 Reverse Charge Code Import VAT | 0% | R1-FR | Purchases |
| IPA4-FR | Postponed import VAT on goods purchased from Great Britain and non-EU countries - reduced rate 5.5% | Effective from January 1, 2022 Reverse Charge Code Import VAT | 0% | R-FR | Purchases |
| IPA5-FR | Postponed import VAT on goods purchased from Great Britain and non-EU countries - reduced rate, special territory 2.1% | Effective from January 1, 2022 Reverse Charge Code Import VAT | 0% | R2-FR | Purchases |
| IPA6-FR | Postponed import VAT on goods purchased from Great Britain and non-EU countries - special reduced rate, special territory 1.05% | Effective from January 1, 2022 Reverse Charge Code Import VAT | 0% | R3-FR | Purchases |
| IS-FR | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge |  | S-FR | Purchases |
| IS1-FR | Purchase of services from outside the EU - standard rate | Effective from January 1, 2021 Import Applies to Service Items | 20% |  | Purchases |
| IS2-FR | Purchase of services from outside the EU - reduced rate (10%) | Effective from January 1, 2021 Import Applies to Service Items | 10% |  | Purchases |
| IS3-FR | Purchase of services from outside the EU - reduced rate (5.5%) | Effective from January 1, 2021 Import Applies to Service Items | 5.5% |  | Purchases |
| IS4-FR | Purchase of services from outside the EU - super reduced rate | Effective from January 1, 2021 Import Applies to Service Items | 2.1% |  | Purchases |
| MO-FR | Monaco transactions | Category: Monaco | Indicate the rate to be used. Consult your tax agency. |  | Sales |
| NF-FR | Sales of goods or services made to non-France-based customers | Category: Sales to Non France Customer | 0% |  | Sales |
| O-FR | Sale of goods outside of EU | Export |  |  | Sales |
| OS-FR | Supply of services outside of EU | Export Applies to Service Items |  |  | Sales |
| R-FR | Reduced rate | Reduced Rate | 5.5% |  | Both (Sales and Purchases) |
| R1-FR | Super reduced rate | Special Territory | 8.5% |  | Both (Sales and Purchases) |
| R2-FR | Super reduced rate | Reduced Rate Special Territory | 2.1% |  | Both (Sales and Purchases) |
| R3-FR | Super reduced rate | Special Reduced Rate Special Territory | 1.05% |  | Both (Sales and Purchases) |
| RC-FR | Reverse charge sales in country | Reverse Charge Code |  | S-FR | Both (Sales and Purchases) |
| RCI-FR | Reverse charge on import VAT | Import Reverse Charge | 0% | S-FR | Purchases |
| S-FR | Standard rate |  | 20% |  | Both (Sales and Purchases) |
| SR-FR | New reduced rate | Special Reduced Rate | 10% |  | Both (Sales and Purchases) |
| Z-FR | Zero rated sales |  | 0% |  | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [France VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1892249.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
