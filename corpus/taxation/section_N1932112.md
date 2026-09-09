---
id: "section_N1932112"
type: "section"
title: "Italy Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Italy Tax Topics > Italy Tax Codes"
parent: "chapter_N1931995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1932112.html"
anchors: ["subsect_1030023803", "bridgehead_N1932170"]
sha256: "81f9ffc22df1fcae75acf117cc007ec57307e517e96b69ad326d229113f88523"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Italy are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030023803}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Italy {#bridgehead_N1932170}

The following table shows the tax properties required to correctly generate the Italy tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates. Starting October 1, 2023, the standard VAT rate is increased to 22%.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-IT | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-IT | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | 0% | R1-IT | Both (Sales and Purchases) |
| ES-IT | EU sales/purchases (goods) | EC Code | 0% | S-IT | Both (Sales and Purchases) |
| ESSP-IT | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-IT | Purchases |
| ESSS-IT | EU sales (services) | EC Code Applies to Service Items | 0% | S-IT | Sales |
| EZ-IT | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-IT | Both (Sales and Purchases) |
| I-IT | Purchase of goods from outside of EU | Import | 0% | \- | Purchases |
| IS-IT | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge Code | 0% | S-IT | Purchases |
| O-IT | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-IT | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Sales |
| R1-IT | Reduced rate | Reduced Rate | 10% | \- | Both (Sales and Purchases) |
| R2-IT | Special reduced rate | Special Reduced Rate | 4% | \- | Both (Sales and Purchases) |
| RC-IT | Reverse charge sales in country | Reverse Charge Code | 0% | S-IT | Both (Sales and Purchases) |
| S-IT | Standard rate | \- | 22% | \- | Both (Sales and Purchases) |
| U-IT | Non taxable | Non-Taxable | 0% | \- | Both (Sales and Purchases) |
| Z-IT | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Italy VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1933560.html)
-   [What goes into each box - Italy VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161131009378.html)
-   [EU Sales List for Italy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1933802.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
