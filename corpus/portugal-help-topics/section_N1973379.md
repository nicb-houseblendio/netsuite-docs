---
id: "section_N1973379"
type: "section"
title: "Portugal Tax Codes"
branch: "portugal-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Portugal Help Topics > Portugal Tax Topics In Accounts Without SuiteTax > Portugal Tax Codes"
parent: "section_161044164894"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1973379.html"
anchors: ["subsect_1030034844", "bridgehead_N1973445", "bridgehead_161224461017", "bridgehead_161224466999"]
sha256: "3671536965a8d583b8583f309ecaa1416723cb8dc2d70293c3294fbd0606b530"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Portugal are set up correctly.

Important:

To be able to set the correct properties for the Portugal tax codes, you need to install the NetSuite International Tax Reports SuiteApp.

For more information about tax codes, see [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html) and [Portugal Tax Code Properties and Fiscal Space](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160751184059.html).

## Important Things to Note {#subsect_1030034844}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Portugal {#bridgehead_N1973445}

The following tables show the tax properties required to correctly generate the tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used on the following tables are suggested names or default system preference. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

## Automatically Provisioned Tax Codes {#bridgehead_161224461017}

The following tax codes are automatically provisioned by the International Tax Reports SuiteApp.

| Tax Code | Description | Property | Rate | Notional Rate | Available On | Category |
| --- | --- | --- | --- | --- | --- | --- |
| E-PT | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) | S1 (Fixed Asset), S0 (None), or S2 (Other Goods and Services) |
| ER-PT | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | 0% | R-PT | Both (Sales and Purchases) | S0 (None) |
| ES-PT | EU sales/purchases (goods) | EC Code | 0% | S-PT | Both (Sales and Purchases) | S0 (None) |
| ESSP-PT | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-PT | Purchases | S0 (None) |
| ESSS-PT | EU sales (services) | EC Code Applies to Service Items | 0% | S-PT | Sales | S0 (None) |
| EZ-PT | EU sales/purchases - zero rate | EC Code | 0% | Z-PT | Both (Sales and Purchases) | S0 (None) |
| MA-PT | Madeira Standard | Special Territory | 22% | \- | Both (Sales and Purchases) | \- |
| O-PT | Sale of goods outside of EU | Export | 0% | \- | Both (Sales and Purchases) | S0 (None) |
| OS-PT | Supply of services outside of EU | Export Applies to Service items | 0% | \- | Both (Sales and Purchases) | S0 (None) |
| R-PT | Reduced rate | Reduced Rate | 6% | \- | Both (Sales and Purchases) | S0 (None) |
| R2-PT | Intermediate rate | Special Reduced Rate | 13% | \- | Both (Sales and Purchases) | S0 (None) |
| RC-PT | Reverse charge in country | Reverse Charge Code | 0% | S-PT | Both (Sales and Purchases) | S1 (Fixed Asset) |
| S-PT | Standard rate | \- | 23% | \- | Both (Sales and Purchases) | S0 (None) |
| UNDEF-PT | Used when NetSuite can't determine the appropriate tax code for a transaction. | \- | 0% | \- | Both (Sales and Purchases) | \- |
| Z-PT | Zero rated sales and purchases | \- | 0% | \- | Both (Sales and Purchases) | S0 (None) |

## Supported Tax Codes {#bridgehead_161224466999}

The following tax codes aren't provisioned by the International Tax Reports SuiteApp but supported in NetSuite. You can create the following tax codes for Portugal and use it for tax reporting. For more information about creating new tax codes, see [Creating Tax Codes - Other Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html).

| Tax Code | Property | Available On | Notional Rate | Category |
| --- | --- | --- | --- | --- |
| FA-PT |  | Both (Sales and Purchases) | \- | S1 (Fixed Asset) |
| G-PT |  | Both (Sales and Purchases) | \- | S2 (Other Goods and Services) |
| EUFA-PT | EC Code | Purchases | Select Notional rate. | S1 (Fixed Asset) |
| EUG-PT | EC Code | Purchases | Select Notional rate. | S2 (Other Goods and Services) |
| A-PT |  | Both (Sales and Purchases) | Select Notional rate. | S4 (Adjustment) |
| AP-PT | Government | Both (Sales and Purchases) | \- | S4 (Adjustment) |
| EUA-PT | EC Code | Both (Sales and Purchases) | \- | S4 (Adjustment) |

### Additional Information

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)

### Related Topics

-   [Portugal Standard Audit File for Tax Purposes (PT SAF-T)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1971159.html)
-   [Portugal Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1973379.html)
-   [Portugal VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1974556.html)
-   [What goes into each box - Portugal VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1974877.html)
-   [EU Sales List for Portugal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1978248.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
