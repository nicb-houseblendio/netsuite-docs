---
id: "section_N1874517"
type: "section"
title: "Czechia Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Czechia Tax Topics > Czechia Tax Codes"
parent: "chapter_N1874317"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1874517.html"
anchors: ["subsect_1030015307", "bridgehead_N1874623"]
sha256: "2db21071a6e2cafe1ba2268ad67dcc5a10eb9c8916e7f8d8387a6b1359e83019"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Czechia are set up correctly.

## Important Things to Note {#subsect_1030015307}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    
-   You must use the tax code properties provided by the SuiteApp. In addition to the properties that are common to all nexuses, the Czechia VAT reporting feature uses the following properties:
    
    -   Reduced Rate
        
    -   Import
        
    
    Carefully review your current tax codes and edit them to match the settings in the [Tax Code Table for Czechia](#bridgehead_N1874623).
    
    For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).
    

## Tax Code Table for Czechia {#bridgehead_N1874623}

The following table shows the tax properties required to correctly generate the Czechia tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Czechia VAT report, see [What goes into each box - Czechia VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1880621.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-CZ | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-CZ | EU sales/purchases (goods and related services) - reduced rate | EC Code Reduced Rate | 0% | R-CZ | Both (Sales and Purchases) |
| ES-CZ | EU sales/purchases (goods and related services) | EC Code | 0% | S-CZ | Both (Sales and Purchases) |
| ESPR-CZ | Purchase of services from another EU country - reduced rate | EC Code Reverse Charge Code Applies to Service Items Reduced Rate | 0% | R-CZ | Purchases |
| ESSP-CZ | Purchase of services from another EU country | EC Code Reverse Charge Code Applies to Service Items | 0% | R-CZ | Purchases |
| ESSS-CZ | Supply of services to another EU country | EC Code Applies to Service Items | 0% | S-CZ | Sales |
| EZ-CZ | EU sales/purchases - zero rate | EC Code | 0% | Z-CZ | Both (Sales and Purchases) |
| I-CZ | Purchase of goods from outside of EU | Import | 20% | \- | Purchases |
| IE-CZ | Imports - exempted goods | Import | 0% | \- | Purchases |
| IG-CZ | Investment gold | Category: Investment Gold | 0% | \- | Purchases |
| IR-CZ | Purchase of goods from outside of EU - reduced rate | Import Reduced Rate | 10% | \- | Purchases |
| IS-CZ | Purchase of services from outside of EU - standard | Import Applies to Service Items Reverse Charge Code | 0% | S-CZ | Purchases |
| ISR-CZ | Purchase of services from outside of EU - reduced | Import Applies to Service Items Reverse Charge Code Reduced Rate | 0% | R-CZ | Purchases |
| ISSR-CZ | Purchase of services from outside of EU - special reduced | Import Applies to Service Items Reverse Charge Code Special Reduced Rate | 0% | SR-CZ | Purchases |
| IZ2-CZ | Tax Codes are supported but not provisioned | Import Reverse Charge Code Category: S0 | 0% | \- | Both (Sales and Purchases) |
| NV-CZ | New vehicles | Category: New vehicles | 21% | \- | Purchases |
| O-CZ | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-CZ | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Sales |
| OT-CZ | Other taxable transactions - standard rate | Category: Others | 21% | \- | Sales |
| OTR-CZ | Other taxable transactions - reduced rate | Reduced Rate Category: Others | 15% | \- | Sales |
| OTSR-CZ | Other taxable transactions - special reduced rate | Special reduced rate Category: Others | 10% | \- | Sales |
| R-CZ | Reduced rate | Reduced Rate | 15% | \- | Sales and Purchases |
| RC-CZ | Reverse charge in country | Reverse Charge Code | 0% | S-CZ | Both (Sales and Purchases) |
| RCOND-CZ | Other taxable supplies where the tax is nondeductible - standard rate | Category: Others Reverse Charge | 0% | S-CZ | Purchases |
| RCOND2-CZ | Other taxable supplies where the tax is nondeductible - reduced rate | Reduced Rate Category: Others Reverse Charge | 0% | R-CZ | Purchases |
| RCOND3-CZ | Other taxable supplies where the tax is nondeductible - special reduced rate | Special Reduced Rate Category: Others Reverse Charge | 0% | SR-CZ | Purchases |
| RCR-CZ | Reverse charge | Reverse Charge Code Reduced Rate | 0% | R-CZ | Purchases |
| RCSR-CZ | Reverse charge - special reduced rate | Reverse charge code Special Reduced Rate | 0% | SR-CZ | Both (Sales and Purchases) |
| S-CZ | Standard rate | \- | 21% | \- | Sales and Purchases |
| SR-CZ | Special reduced rate | Special reduced rate | 10% | \- | Both (Sales and Purchases) |
| Z-CZ | Zero rated sales | \- | 0% | \- | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Czechia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1880287.html)
-   [Czechia VAT Control Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4491314862.html)
-   [EU Sales List for Czechia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1884938.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
