---
id: "section_N1999320"
type: "section"
title: "Spain Tax Codes"
branch: "spain-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Spain Help Topics > Spain Tax Topics For Accounts Without SuiteTax > Spain Tax Codes"
parent: "section_0628121941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1999320.html"
anchors: ["bridgehead_N1999332", "subsect_1030040829", "bridgehead_N1999427"]
sha256: "d5d4f9fbdf938b229451b7c310e7be02d257a7d960575058c4aa4297a0b46f03"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Spain are set up correctly.

## Spain Tax Code Changes {#bridgehead_N1999332}

If you're using the NetSuite International Tax Reports SuiteApp, take note of the following:

-   You must use the tax code properties provided by the SuiteApp. The VAT reporting feature for Spain uses Surcharge, Reduced Rate, Special Reduced Rate properties, as well as special tax categories. These are in addition to the properties that are common to all nexuses. Carefully review your current tax codes and edit them to match the settings in the [Tax Code Table for Spain](#bridgehead_N1999427).
    
-   The ESSP tax code used for purchases of services from EU must have a check on the boxes for Reverse Charge Code, EC Code, and Applies to Service Items.
    

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030040829}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Spain {#bridgehead_N1999427}

The following table shows the tax properties required to correctly generate the tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Modelo 303 Quarterly VAT Return, see [What goes into each box - Spain VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2001334.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| CA-ES | Current assets | Import Category: Current Assets | 21% |  | Purchases |
| CG-ES | Capital goods | Category: Capital Goods | 21% |  | Purchases |
| EIG-ES | EC investment goods | EC Code Category: Investment Goods |  | S-ES | Purchases |
| ER-ES | EU sales/purchases (goods and related services) - reduced rate | EC Code Reduced Rate |  | R-ES | Both (Sales and Purchases) |
| ES-ES | EU sales/purchases (goods and related services) | EC Code |  | S-ES | Both (Sales and Purchases) |
| ESSP-ES | Purchase of services from another EU country | EC Code Reverse Charge Code Applies to Service Items |  | S-ES | Purchases |
| ESSS-ES | Sale of services to another EU country | EC Code Applies to Service Items |  | S-ES | Sales |
| EZ-ES | EU sales/purchases - zero rate | EC Code |  | Z-ES | Both (Sales and Purchases) |
| IG-ES | Investment goods | Import Category: Investment Goods | 21% |  | Purchases |
| O-ES | Sale of goods outside of EU | Export |  |  | Sales |
| OS-ES | Supply of services outside of EU | Export Applies to Service Items |  |  | Sales |
| R-ES | Reduced rate | Reduced Rate | 10% |  | Both (Sales and Purchases) |
| R2-ES | Special reduced rate | Special Reduced Rate | 4% |  | Both (Sales and Purchases) |
| RC-ES | Reverse charge in country | Reverse Charge Code |  | S-ES | Both (Sales and Purchases) |
| RI-ES | Regularization investments | Category: Regularization Investments | 21% |  | Purchases |
| SC1-ES | Retail surcharge rate | Special Reduced Rate Surcharge | 0.5% |  | Both (Sales and Purchases) |
| SC2-ES | Retail surcharge rate | Reduced Rate Surcharge | 1.4% |  | Both (Sales and Purchases) |
| SC3-ES | Retail surcharge rate | Surcharge | 5.2% |  | Both (Sales and Purchases) |
| S-ES | Standard rate |  | 21% |  | Both (Sales and Purchases) |
| Z-ES | Zero rated sales |  | 0% |  | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Spain VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2001072.html)
-   [EU Sales List for Spain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2004312.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
