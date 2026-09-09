---
id: "section_N1846495"
type: "section"
title: "Bulgaria Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Bulgaria Tax Topics > Bulgaria Tax Codes"
parent: "chapter_N1846363"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1846495.html"
anchors: ["subsect_1030012854", "bridgehead_N1846558"]
sha256: "06cc4040f819ac27a162f157a036f72cf12c6bfdd16d1231416adcde0680c917"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Bulgaria are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030012854}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Bulgaria {#bridgehead_N1846558}

The following table shows the tax properties required to correctly generate the Bulgaria tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-BG | Exempt | Exempt | 0% | 0% | Both (Sales and Purchases) |
| ER-BG | EU sales/purchases (goods) - reduced rate | EC Code | 0% | R-BG | Both (Sales and Purchases) |
| ES-BG | EU sales/purchases (goods) | EC Code | 0% | S-BG | Both (Sales and Purchases) |
| ESSP-BG | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-BG | Purchases |
| ESSS-BG | EU sales (services) | EC Code Applies to Service Items | 0% | S-BG | Sales |
| EZ-BG | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-BG | Both (Sales and Purchases) |
| I-BG | Purchase of goods from outside of EU | Import | 0% | \- | Purchases |
| IS-BG | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge Code | 0% | S-BG | Purchases |
| O-BG | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-BG | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Sales |
| P-BG | Protocol related purchases | Category: Protocol | 20% | \- | Both (Sales and Purchases) |
| PC-BG | Partial credit | Partial Tax Credit | 20% | \- | Purchases |
| PC2-BG | Partial credit - reduced rate | Partial Tax Credit Reduced Rate | 9% | \- | Purchases |
| R-BG | Reduced rate | Reduced Rate | 9% | \- | Both (Sales and Purchases) |
| RC-BG | Reverse charge | Reverse Charge Code | 0% | S-BG | Both (Sales and Purchases) |
| S-BG | Standard rate | \- | 20% | \- | Both (Sales and Purchases) |
| T-BG | Zero rated NATO, Tourism transactions | Category: Tourism | 0% | \- | Both (Sales and Purchases) |
| TR-BG | Transactions involving triangulation | Category: Triangulation | 0% | \- | Both (Sales and Purchases) |
| Z-BG | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Bulgaria VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1850643.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
