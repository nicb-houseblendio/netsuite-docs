---
id: "section_N1978614"
type: "section"
title: "Romania Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Romania Tax Topics > Romania Tax Codes"
parent: "chapter_N1978514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1978614.html"
anchors: ["subsect_1030035024", "bridgehead_N1978673"]
sha256: "4115e501446b11a9d373d97d0f928d439d1da6d78c2359b38e3aa8b5ae2b3d02"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Romania are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030035024}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Romania {#bridgehead_N1978673}

The following table shows the tax properties required to correctly generate the Romania tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-RO | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-RO | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | \- | R1-RO | Both (Sales and Purchases) |
| ES-RO | EU sales/purchases (goods) | EC Code | \- | S-RO | Both (Sales and Purchases) |
| ESSP-RO | EU purchases (services) | EC Code Reverse Charge Code Applies to Service Items | \- | S-RO | Purchases |
| ESSS-RO | EU sales (services) | EC Code Applies to Service Items | \- | S-RO | Sales |
| EZ-RO | EU sales/purchases (goods) - zero rate | EC Code | \- | Z-RO | Both (Sales and Purchases) |
| I-RO | Purchase of goods from outside of EU | Import | \- | \- | Purchases |
| IS-RO | Purchase of services from outside of EU | Import Reverse Charge Code Applies to Service Items | \- | S-RO | Purchases |
| O-RO | Sale of goods outside of EU | Export | \- | \- | Sales |
| OS-RO | Supply of services outside of EU | Export Applies to Service Items | \- | \- | Sales |
| R1-RO | Reduced rate | Reduced Rate | 9% | \- | Both (Sales and Purchases) |
| R2-RO | Special reduced rate | Special Reduced Rate | 5% | \- | Both (Sales and Purchases) |
| RC-RO | Reverse charge in country | Reverse Charge Code | \- | S-RO | Both (Sales and Purchases) |
| S-RO | Standard rate | \- | 19% | \- | Both (Sales and Purchases) |
| Z-RO | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Romania VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1979984.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
