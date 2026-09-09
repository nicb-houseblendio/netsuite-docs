---
id: "section_N1967757"
type: "section"
title: "Poland Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Poland Tax Topics > Poland Tax Codes"
parent: "chapter_N1967656"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1967757.html"
anchors: ["subsect_1030034712", "bridgehead_N1967816"]
sha256: "a85bcd240ae786ca9c90ff56b48b5bb0d1ee94e224cfb7ba69331735ee2fb943"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Poland are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030034712}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Poland {#bridgehead_N1967816}

The following table shows the tax properties required to correctly generate the Poland tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Poland VAT report, see [What goes into each box - Poland VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4037502030.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-PL | Exempt or non taxable | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-PL | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | 0% | R-PL | Both (Sales and Purchases) |
| ES-PL | EU sales/purchases (goods) | EC Code | 0% | S-PL | Both (Sales and Purchases) |
| ESSP-PL | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-PL | Purchases |
| ESSS-PL | EU sales (services) | EC Code Applies to Service Items | 0% | S-PL | Sales |
| EZ-PL | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-PL | Both (Sales and Purchases) |
| FA-PL | Fixed assets | Capital Goods | 23% | \- | Purchases |
| I-PL | Purchase of goods from outside of EU | Import | 23% | \- | Purchases |
| IS-PL | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge Code | 0% | S-PL | Purchases |
| O-PL | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-PL | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Sales |
| R-PL | Reduced rate | Reduced Rate | 8% | \- | Both (Sales and Purchases) |
| R1-PL | Super reduced rate | Special Reduced Rate | 5% | \- | Both (Sales and Purchases) |
| RC-PL | Reverse charge | Reverse Charge Code | 0% | S-PL | Both (Sales and Purchases) |
| S-PL | Standard rate | \- | 23% | \- | Both (Sales and Purchases) |
| Z-PL | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Poland VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1970414.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
