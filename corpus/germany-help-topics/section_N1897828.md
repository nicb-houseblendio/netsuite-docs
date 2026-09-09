---
id: "section_N1897828"
type: "section"
title: "Germany Tax Codes"
branch: "germany-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Germany Help Topics > Germany Tax Topics For Accounts Without SuiteTax > Germany Tax Codes"
parent: "section_1554981475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1897828.html"
anchors: ["subsect_1030022141", "bridgehead_N1897951", "subsect_159296420582", "bridgehead_N1899302"]
sha256: "0b0d01dd53f25cc926aceace44de1c88f58b14377eeff1297ff366fe48c35df3"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Germany are set up correctly.

## Important Things to Note {#subsect_1030022141}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    
-   You must use the tax code properties provided by the SuiteApp. In addition to the properties that are common to all nexuses, the Germany VAT reporting feature uses the following properties:
    
    -   Reduced Rate
        
    -   Special Reduced Rate
        
    -   Import
        
    -   Import VAT
        
    
    Carefully review your current tax codes and edit them to match the settings in the [Tax Code Table for Germany](#bridgehead_N1897951).
    
    For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).
    
-   The **Reverse Charge Code** box must be checked on the ESSP tax code used for purchases of services from other EU member states.
    
-   Tax codes for purchases of services from outside the EU must have the following boxes checked:
    
    -   Reverse Charge Code
        
    -   Import
        
    -   Applies to Service Items
        
    
    For more information about the settings for the IS tax code, see [Tax Code Table for Germany](#bridgehead_N1897951).
    
-   In response to the COVID-19 tax relief measures, temporary tax codes with effectivity date of July 1, 2020 to December 31, 2020 are provisioned to accounts with Germany nexus. For more information, see [Germany COVID-19 Tax Response: Temporary Tax Codes](#subsect_159296420582).
    

## Tax Code Table for Germany {#bridgehead_N1897951}

The following table shows the tax properties required to correctly generate the Germany tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Periodic VAT report for Germany, see [What goes into each box - Germany Monthly/Quarterly VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899865.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Deutsche Beschreibung | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- | --- |
| E-DE | Exempt | Steuerfrei | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-DE | EU sales/purchases (goods and related services) - reduced rate | EG-Verkäufe/Einkäufe (Waren und verb. Dienstleistungen) - Ermäßigter Steuersatz | EC Code Reduced Rate | 0% | R-DE | Both (Sales and Purchases) |
| ERT-DE | EC sales/purchases (goods and related services) - reduced rate, rate more than 0 | EG-Verkäufe/Einkäufe (Waren und verb. Dienstleistungen) - ermäßigter Satz, Satz höher als Null | EC Code Default Code Reduced Rate | Any rate greater than 0% | R-DE | Both (Sales and Purchases) |
| ES-DE | EC sales/purchases to another EC country (goods) | EG-Verkäufe/Einkäufe an anderen EG-Staat (Waren) | EC Code | 0% | S-DE | Both (Sales and Purchases) |
| ESR-DE | EU purchases - other rate | EG-Einkäufe - Sondersatz | EC Code Special Reduced Rate | 0% | Any rate greater than 0% | Both (Sales and Purchases) |
| ESSP-DE | EC purchases (services) | EG-Einkäufe (Dienstleistungen) | EC Code Reverse Charge Code Applies to Service Items | 0% | S-DE | Both (Sales and Purchases) |
| ESSS-DE | EC sales (services) | EG-Verkäufe (Dienstleistungen) | EC Code Applies to Service Items | 0% | S-DE | Both (Sales and Purchases) |
| EST-DE | EC sales/purchases to another EC country (goods), rate more than 0 | EG-Verkäufe/Einkäufe an anderen EG-Staat (Waren), Satz höher als Null | EC Code | Any rate greater than 0% | S-DE | Both (Sales and Purchases) |
| EZ-DE | Tax-free EU sales/purchases | Steuerfreie innergemeinschaftliche Erwerbe | EC Code Nontaxable | 0% | Z-DE | Both (Sales and Purchases) |
| EZR-DE | EU purchases - zero rate | EU-Einkäufe - Nullsatz | Effective from January 1, 2023 EC Code | 0% | ZR-DE | Both (Sales and Purchases) |
| IS-DE | Purchase of services from outside of EU | Einkauf von Dienstleistungen aus Nicht-EU-Staat | Reverse Charge Code Applies to Service Items Import | 0% | S-DE | Both (Sales and Purchases) |
| IT-DE | Import tax | Einfuhrsteuer | Import VAT | 0% | \- | Both (Sales and Purchases) |
| OS-DE | Sales to third country outside of EU | Verkauf an Drittstaat außerhalb der EU | Applies to Service Items Export | 0% | \- | Both (Sales and Purchases) |
| R-DE | Reduced rate | Ermäßigter Steuersatz | Reduced Rate | 7% | \- | Both (Sales and Purchases) |
| RC-DE | Reverse charge | Umkehrung der Steuerschuld | Reverse Charge Code | 0% | S-DE | Both (Sales and Purchases) |
| S-DE | Standard rate | Normal-Steuersatz | \- | 19% | \- | Both (Sales and Purchases) |
| S1-DE | Mobile Device | Mobilgerät | Reverse Charge Code Category: Mobile Device | 0% | S-DE | Both (Sales and Purchases) |
| SR-DE | Other rate | Sondersatz | Special Reduced Rate | 0% | \- | Both (Sales and Purchases) |
| Z-DE | Tax-free sales without input tax deduction | Steuerfreie Umsätze ohne Vorsteuerabzug | Nontaxable | 0% | \- | Both (Sales and Purchases) |
| ZR-DE | Zero rate | Nullsatz | Effective from January 1, 2023 | 0% | \- | Both (Sales and Purchases) |
| ZX-DE | International exports (third country) | Internationale Exporte (Drittstaat) | Export | 0% | \- | Both (Sales and Purchases) |

### Germany COVID-19 Tax Response: Temporary Tax Codes {#subsect_159296420582}

In response to the COVID-19 tax relief measure, temporary tax codes with reduced rates are effective on July 1, 2020 until December 31, 2020. The International Tax Reports SuiteApp provisions the following tax codes to accounts with Germany nexus:

| Tax Code | Description | Rate | Effective From | Valid Until | Property | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- | --- | --- |
| S2-DE | Standard rate from July 1, 2020 - December 31, 2020 | 16% | July 1, 2020 | December 31, 2020 |  |  | Both (Sales and Purchases) |
| R1-DE | Reduced rate from July 1, 2020 - December 31, 2020 | 5% | July 1, 2020 | December 31, 2020 | Reduced Rate |  | Both (Sales and Purchases) |
| RC1-DE | Reverse charge from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | Reverse Charge Code | S2-DE | Both (Sales and Purchases) |
| SS1-DE | Applicable for Mobile Devices from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | Reverse Charge Code Category: Mobile Device | S2-DE | Both (Sales and Purchases) |
| ES1-DE | EC sales/purchases to another EC country (goods) - standard rate from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | EC Code | S2-DE | Both (Sales and Purchases) |
| ER1-DE | EU sales/purchases (goods and related services) - reduced rate from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | EC Code Reduced Rate | R1-DE | Both (Sales and Purchases) |
| ESSS1-DE | EC sales (services) from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | EC Code Applies to Service Items | S2-DE | Both (Sales and Purchases) |
| ESSP1-DE | EC purchases (services) from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | EC Code Reverse Charge Code Applies to Service Items | S2-DE | Both (Sales and Purchases) |
| IS1-DE | Purchase of services from outside of EU from July 1, 2020 - December 31, 2020 | 0% | July 1, 2020 | December 31, 2020 | Reverse Charge Code Applies to Service Items Import | S2-DE | Both (Sales and Purchases) |

## Tracking VAT Paid on Imports into Germany {#bridgehead_N1899302}

You should have a tax code for imports that are subject to VAT (refer to tax code IT in the tax code table). When recording the type of bill (which is a 100% VAT bill), ensure that you record this import VAT as input tax, where the net amount represents the VAT amount. NetSuite reports the full net amount in box 62 of the German VAT report.

### Additional Information

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

### Related Topics

-   [Germany VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899458.html)
-   [Setting Up Tax Filing for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1917361.html)
-   [Submission of VAT Returns in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1917621.html)
-   [Recapitulative Statement (EU Sales List) for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1918495.html)
-   [Intrastat Report for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4149981058.html)
-   [Germany GoBD Data Export](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3838969498.html)
-   [Germany Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554981475.html)
-   [Germany Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726737.html)
-   [Setting Up Germany-Specific Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726820.html)
-   [Germany-specific SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158529777788.html)
-   [Germany Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554985535.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
