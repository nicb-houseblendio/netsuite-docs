---
id: "section_N2004717"
type: "section"
title: "Sweden Tax Codes"
branch: "sweden-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Sweden Help Topics > Sweden Tax Topics For Accounts Without SuiteTax > Sweden Tax Codes"
parent: "section_157476810322"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2004717.html"
anchors: ["subsect_1030041358", "bridgehead_N2004861"]
sha256: "6fb36345054ea26058a8a9a53afa88b9bbdedcea11e635b4b0b3bdf9dd9a110c"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Sweden are set up correctly.

## Important Things to Note {#subsect_1030041358}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    
-   You must use the new tax code properties provided by the SuiteApp. In addition to the properties that are common to all nexuses, the VAT reporting feature for Sweden uses the following properties:
    
    -   Import
        
    -   Reduced Rate
        
    -   Special Reduced Rate
        
    
    Carefully review your current tax codes and edit them to match the settings in the [Tax Code Table for Sweden](#bridgehead_N2004861).
    
-   The following boxes must be checked on the ESSP tax code used for purchases of services from EU:
    
    -   Reverse Charge Code
        
    -   EC Code
        
    -   Applies to Service Items
        
-   Transactions with the following tax code settings are not included in the Sweden VAT report:
    
    -   Tax code for purchase of services with the following boxes checked:
        
        -   Applies to Service Items
            
        -   Reverse Charge Code
            
    -   Tax codes for sales or purchase of goods and services within the EU with the following boxes checked:
        
        -   Applies to Service Items
            
        -   Reverse Charge Code
            
        -   Export
            
    
    Edit your tax codes and refer to the [Tax Code Table for Sweden](#bridgehead_N2004861) for the new tax code settings.
    
    For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).
    

## Tax Code Table for Sweden {#bridgehead_N2004861}

The following table shows the tax properties required to correctly generate the tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the VAT declaration for Sweden, see [What goes into each box - Sweden VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2006403.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-SE | Exempt | Exempt | 0% |  | Both (Sales and Purchases) |
| ER-SE | EU sales/purchases (goods and related services) - reduced rate | EC Code Reduced Rate | 0% | R-SE | Both (Sales and Purchases) |
| ES-SE | EU sales/purchases (goods) | EC Code | 0% | S-SE | Both (Sales and Purchases) |
| ESR-SE | EU sales/purchases (goods and related services) - special reduced rate | EC Code Special Reduced Rate | 0% | SR-SE | Both (Sales and Purchases) |
| ESSP-SE | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-SE | Purchases |
| ESSS-SE | EU sales (services) | EC Code Applies to Service Items | 0% | S-SE | Sales |
| EZ-SE | EU purchases - zero rate | EC Code | 0% | Z-SE | Both (Sales and Purchases) |
| I-SE | Purchase of goods from outside of EU | Import | 0% |  | Purchases |
| IS-SE | Purchase of services from outside of EU | Import Reverse Charge Code Applies to Service Items | 0% | S-SE | Purchases |
| ISR-SE | Purchase of services from outside of EU | Effective From: January 1, 2022 Reverse Charge Code Import Applies to Service Items Reduced Rate | 0% | R-SE | Purchases |
| ISSR-SE | Purchase of services from outside of EU | Effective From: January 1, 2022 Reverse Charge Code Import Applies to Service Items Special Reduced Rate | 0% | SR-SE | Purchases |
| IV-SE | Import VAT at standard rate | Import Reverse Charge Code | 0% | S-SE | Purchases |
| IVR-SE | Import VAT at reduced rate | Import Reduced Rate Reverse Charge Code | 0% | R-SE | Purchases |
| IVSR-SE | Import VAT at special rate | Import Special Reduced Rate Reverse Charge Code | 0% | SR-SE | Purchases |
| O-SE | Sale of goods outside of EU | Export | 0% |  | Sales |
| R-SE | Reduced rate | Reduced Rate | 12% |  | Both (Sales and Purchases) |
| RCG-SE | Reverse charge in country (goods) | Reverse Charge Code | 0% | S-SE | Both (Sales and Purchases) |
| RCS-SE | Reverse charge in country (services) | Reverse Charge Code Applies to Service Items | 0% | S-SE | Both (Sales and Purchases) |
| S-SE | Standard rate |  | 25% |  | Both (Sales and Purchases) |
| SR-SE | Special reduced rate | Special Reduced Rate | 6% |  | Both (Sales and Purchases) |
| Z-SE | Zero rated sales |  | 0% |  | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Sweden VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2006138.html)
-   [EU Sales List for Sweden](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2009636.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
