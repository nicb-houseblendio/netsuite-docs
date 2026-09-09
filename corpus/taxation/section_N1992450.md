---
id: "section_N1992450"
type: "section"
title: "Slovenia Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Slovenia Tax Topics > Slovenia Tax Codes"
parent: "chapter_N1992349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1992450.html"
anchors: ["subsect_1030040142", "bridgehead_N1992508"]
sha256: "e1332d4e51aec288c8ab6136850fcf2a9ff7d9de7333586b9a4baeb1b1e3c313"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Slovenia are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030040142}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Slovenia {#bridgehead_N1992508}

The following table shows the tax properties required to correctly generate the Slovenia tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-SI | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-SI | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | 0% | R-SI | Both (Sales and Purchases) |
| ES-SI | EU sales/purchases (goods) | EC Code | 0% | S-SI | Both (Sales and Purchases) |
| ESR-SI | EC sales/purchases to another EC country (goods) - super reduced rate | \- | 0% | 5% | Both (Sales and Purchases) |
| ESSP-SI | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code Special Reduced Rate | 0% | S-SI | Both (Sales and Purchases) |
| ESSP2-SI | EU purchases (services) - reduced rate | EC Code Applies to Service Items Reverse Charge Code Reduced Rate | 0% | R-SI | Both (Sales and Purchases) |
| ESSP3-SI | EC Purchases (services) - super reduced rate | Applies to Service Items | 0% | 5% | Both (Sales and Purchases) |
| ESSS-SI | EU sales (services) | EC Code Applies to Service Items | 0% | S-SI | Both (Sales and Purchases) |
| EZ-SI | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-SI | Both (Sales and Purchases) |
| FAE-SI | Exempt acquisition of fixed assets | Capital Goods | 0% | \- | Purchases |
| FAR-SI | Acquisition of fixed assets at 9.5% | Capital Goods | 9.5% | \- | Purchases |
| FAS-SI | Acquisition of fixed assets at 22% | Capital Goods | 22% | \- | Purchases |
| FASR-SI | Acquisition of fixed assets at 5% | Capital Goods | 5% | \- | Purchases |
| I-SI | Purchase of goods from outside of EU | Import | 20% | \- | Both (Sales and Purchases) |
| IS-SI | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge | 0% | S-SI | Both (Sales and Purchases) |
| O-SI | Sale of goods outside of EU | Export | 0% | \- | Both (Sales and Purchases) |
| OS-SI | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Both (Sales and Purchases) |
| R-SI | Reduced rate | Reduced Rate | 9.5% | \- | Both (Sales and Purchases) |
| RC-SI | Reverse charge in country | Reverse Charge Code | 0% | S-SI | Both (Sales and Purchases) |
| S-SI | Standard rate | \- | 22% | \- | Both (Sales and Purchases) |
| SR-SI | Super reduced rate | \- | 5% | \- | Both (Sales and Purchases) |
| Z-SI | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Slovenia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1993752.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
