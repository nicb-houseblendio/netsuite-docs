---
id: "section_N1942969"
type: "section"
title: "Netherlands Tax Codes"
branch: "netherlands-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Netherlands Help Topics > Netherlands Tax Topics In Accounts Without SuiteTax > Netherlands Tax Codes"
parent: "chapter_N1942820"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1942969.html"
anchors: ["subsect_1030032835", "bridgehead_N1943113"]
sha256: "769fa0df93bf052c62a27706df8aabdde430fc73346d6ead4c504761913cf456"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Netherlands are set up correctly.

## Important Things to Note {#subsect_1030032835}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    
-   You must use the tax code properties provided by the SuiteApp. In addition to the properties that are common to all nexuses, the VAT reporting feature for Netherlands uses the following properties:
    
    -   Import
        
    -   Reduced Rate
        
    -   Special Reduced Rate
        
    
    Carefully review your current tax codes and edit them to match the settings in the [Tax Code Table for Netherlands](#bridgehead_N1943113).
    
-   The following boxes must be checked on the ESSP tax code used for purchases of services from other EU member states:
    
    -   Reverse Charge Code
        
    -   EC Code
        
    -   Applies to Service Items
        
-   Transactions with the following tax code settings aren't included in the Netherlands VAT report:
    
    -   Tax code for purchases of goods from outside the EU with the following boxes checked:
        
        -   Export
            
        -   Reverse Charge Code
            
    -   Tax codes for sales or purchases of services from outside the EU with the following boxes checked:
        
        -   Applies to Service Items
            
        -   Reverse Charge Code
            
        -   Export
            
    
    Edit your tax codes and refer to the [Tax Code Table for Netherlands](#bridgehead_N1943113) for the new tax code settings.
    
    For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).
    

## Tax Code Table for Netherlands {#bridgehead_N1943113}

The following table shows the tax properties required to correctly generate the tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Netherlands VAT Return, see [What goes into each box - Netherlands VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1944574.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult your tax agency for the correct tax rates. As of October 1, 2012, the standard tax rate increased to 21%.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-NL | Exempt | Exempt | 0% |  | Both (Sales and Purchases) |
| ER-NL | EU sales/purchases (goods and related services) - reduced rate | EC Code Reduced Rate |  | R-NL | Both (Sales and Purchases) |
| ES-NL | EU sales/purchases (goods and related services) | EC Code |  | S-NL | Both (Sales and Purchases) |
| ESSP-NL | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code |  | S-NL | Purchases |
| ESSS-NL | EU sales (services) | EC Code Applies to Service Items | 0% | S-NL | Sales |
| EZ-NL | EU sales/purchases - zero rate | EC Code |  | Z-NL | Both (Sales and Purchases) |
| I-NL | Purchase of goods from outside of EU | Import Reverse Charge Code |  |  | Purchases |
| IS-NL | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge Code |  | S-NL | Purchases |
| IV-NL | 100% VAT bill Note: This tax code is recorded as input tax where the net amount represents the VAT amount. | Import VAT | 0% |  | Purchases |
| O-NL | Sales outside of EU | Export | 0% |  | Sales |
| OS-NL | Supply of services outside of EU | Export Applies to Service items Exclude from VAT Reports |  |  | Sales |
| R-NL | Reduced rate | Reduced Rate | 9% |  | Both (Sales and Purchases) |
| RC-NL | Reverse charge | Reverse Charge Code |  | S-NL | Both (Sales and Purchases) |
| S-NL | Standard rate |  | 21% |  | Both (Sales and Purchases) |
| SP-NL | Other rate | Special Reduced Rate | 12% |  | Both (Sales and Purchases) |
| Z-NL | Zero rated sales |  | 0% |  | Both (Sales and Purchases) |

### Additional Information

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

### Related Topics

-   [Netherlands VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1944310.html)
-   [What goes into each box - Netherlands VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1944574.html)
-   [EU Sales List for Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1947306.html)
-   [Intrastat Report for Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503450407.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [EU One Stop Shop Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4174874694.html)
-   [OSS Tax Code Provisioning for Regular NetSuite Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4204428442.html)
-   [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html)
-   [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html)
-   [Netherlands Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636146.html)
-   [Netherlands Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549424762.html)
-   [Setting Up Netherlands-Specific Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549425210.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
