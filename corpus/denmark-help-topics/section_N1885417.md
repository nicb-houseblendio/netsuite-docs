---
id: "section_N1885417"
type: "section"
title: "Denmark Tax Codes"
branch: "denmark-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Denmark Help Topics > Denmark Tax Topics For Accounts Without SuiteTax > Denmark Tax Codes"
parent: "section_157495175064"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1885417.html"
anchors: ["subsect_1030015950", "bridgehead_N1885476"]
sha256: "8c90a004062f9951201cee8e73e1b8c4a601c0314282ee3791db23b37b209d99"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Denmark are set up correctly.

For more about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030015950}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Denmark {#bridgehead_N1885476}

The following table shows the tax properties required to correctly generate the Denmark tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-DK | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ES-DK | EU sales/purchases (goods) | EC Code | 0% | S-DK | Both (Sales and Purchases) |
| ESSP-DK | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-DK | Purchases |
| ESSS-DK | EU sales (services) | EC Code Applies to Service Items | 0% | S-DK | Sales |
| EZ-DK | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-DK | Both (Sales and Purchases) |
| I-DK | Purchase of goods from outside of EU | Import | 25% | \- | Purchases |
| I2-DK | Purchase of goods outside the EU by business registered for import | Import Reverse Charge Code | 0% | S-DK | Purchases |
| ID-DK | Import duty for purchase of goods from outside of EU | Category: Import Duty Reverse Charge Code | 0% | S-DK | Purchases |
| IS-DK | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge Code | 0% | S-DK | Purchases |
| IV-DK | 100% VAT invoice | Import VAT | 0% | \- | Purchases |
| O-DK | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-DK | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Sales |
| RC-DK | Reverse charge sales in country | Reverse Charge Code | 0% | S-DK | Both (Sales and Purchases) |
| S-DK | Standard rate | \- | 25% | \- | Both (Sales and Purchases) |
| S2-DK | Oil and liquefied petroleum gas tax | Category: Oil and liquefied petroleum gas tax | 25% | \- | Purchases |
| S3-DK | Electricity Tax | Category: Electricity Tax | 25% | \- | Purchases |
| S4-DK | Natural and town gas tax | Category: Natural and town gas tax | 25% | \- | Purchases |
| S5-DK | Coal tax | Category: Coal tax | 25% | \- | Purchases |
| S6-DK | Carbon dioxide tax | Category: Carbon dioxide tax | 25% | \- | Purchases |
| S7-DK | Water tax | Category: Water tax | 25% | \- | Purchases |
| Z-DK | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Setting Up Tax Filing for Denmark](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1886840.html)
-   [Denmark VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1887046.html)
-   [Intrastat Report for Denmark](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505371864.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
