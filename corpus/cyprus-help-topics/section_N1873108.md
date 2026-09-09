---
id: "section_N1873108"
type: "section"
title: "Cyprus Tax Codes"
branch: "cyprus-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Cyprus Help Topics > Cyprus Tax Topics For Accounts Without SuiteTax > Cyprus Tax Codes"
parent: "chapter_N1873007"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1873108.html"
anchors: ["subsect_1030014431", "bridgehead_N1873167"]
sha256: "0fb23d18254d4903c149459aa8886d6913b56a40bf5a65b225465b5c46010e3e"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate the correct values on transaction records and tax reports, make sure that the tax codes for Cyprus are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030014431}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Cyprus {#bridgehead_N1873167}

The following table shows the tax properties needed to correctly generate the tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates. The following table shows standard and reduced rates that take effect on January 13, 2014.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-CY | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ES-CY | Sales within EU - standard rate | EC Code | 0% | S-CY | Both (Sales and Purchases) |
| ESSP-CY | Purchase of services from within EU | EC Code Applies to Service Items Reverse Charge Code | 0% | S-CY | Both (Sales and Purchases) |
| ESSS-CY | Supply of services within EU | EC Code Applies to Service Items | 0% | S-CY | Both (Sales and Purchases) |
| EZ-CY | Sales within EU - zero rate | EC Code | 0% | Z-CY | Both (Sales and Purchases) |
| I-CY | Purchase of goods from outside EU | Import | 0% | \- | Both (Sales and Purchases) |
| IS-CY | Purchase of services from outside EU | Applies to Service Items Reverse Charge Code Import | 0% | S-CY | Both (Sales and Purchases) |
| O-CY | Sales outside of EU | Export | 0% | \- | Both (Sales and Purchases) |
| R1-CY | Reduced rate | Reduced | 9% | \- | Both (Sales and Purchases) |
| R2-CY | Special reduced rate | Super Reduced | 5% | \- | Both (Sales and Purchases) |
| RC-CY | Reverse charge in country | Reverse Charge | 0% | S-CY | Both (Sales and Purchases) |
| S-CY | Standard rate | \- | 19% | \- | Both (Sales and Purchases) |
| Z-CY | Zero rate | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Cyprus VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1874088.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
