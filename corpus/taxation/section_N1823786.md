---
id: "section_N1823786"
type: "section"
title: "Austria Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Austria Tax Topics > Austria Tax Codes"
parent: "chapter_N1823604"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1823786.html"
anchors: ["subsect_1030010904", "bridgehead_N1823901", "subsect_59093951013", "bridgehead_N1825737"]
sha256: "1a55561f858f270e9ee91694757f5fb7a3d05febc64f7c44bb22e3fb713fa345"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Austria are set up correctly.

## Important Things to Note {#subsect_1030010904}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    
-   You must use the tax code properties provided by the SuiteApp. In addition to the properties that are common to all nexuses, the Austria VAT reporting feature uses the following properties:
    
    -   Reduced Rate
        
    -   Special Reduced Rate
        
    -   Special Territory
        
    -   Paid
        
    -   Import
        
    -   Import VAT
        
    
    Carefully review your current tax codes and edit them to match the settings in the [Tax Code Table for Austria](#bridgehead_N1823901).
    
    For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).
    
-   The following boxes must be checked on the ESSP tax code used for purchases of services from EU:
    
    -   Reverse Charge Code
        
    -   EC Code
        
    -   Applies to Service Items
        

## Tax Code Table for Austria {#bridgehead_N1823901}

The following table shows the tax properties required to correctly generate the Austria tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Austrian VAT report, see [What goes into each box - Austria VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1826752.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-AT | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-AT | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | 0% | R-AT | Both (Sales and Purchases) |
| ER3-AT | EC sales and purchases (goods) - reduced rate at 5% according to Section 28 Abs. 52 Z 1 from July 1, 2020 - December 31, 2020 | EC Code Reduced Rate | 0% | R3-AT | Both (Sales and Purchases) |
| ES-AT | EU sales and purchases (goods) | EC Code | 0% | S-AT | Both (Sales and Purchases) |
| ESR-AT | EU sales/purchases (goods) - special reduced rate | EC Code Special Reduced Rate | 0% | R2-AT | Both (Sales and Purchases) |
| ESSP-AT | EU purchases (services) | EC Code Reverse Charge Code Applies to Service Items | 0% | S-AT | Purchases |
| ESSS-AT | EU sales (services) | EC Code Applies to Service Items | 0% | S-AT | Sales |
| EZ-AT | EU sales/purchases - zero rate | EC Code | 0% | Z-AT | Both (Sales and Purchases) |
| I-AT | Purchase of goods from outside of EU | Import | 0% | \- | Purchases |
| Import VAT-P | VAT paid to customs on imports | Paid Import VAT | 0% | \- | Purchases |
| Import VAT-U | VAT not yet paid on imports | Import VAT | 0% | \- | Purchases |
| IS-AT | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge | 0% | S-AT | Purchases |
| O-AT | Sales outside of EU | Export | 0% | \- | Sales |
| R-AT | Reduced rate | Reduced Rate | 10% | \- | Both (Sales and Purchases) |
| R2-AT | Special Reduced Rate | Special Reduced Rate | 13% | \- | Both (Sales and Purchases) |
| R3-AT | Reduced Rate at 5% according to Section 28 Abs. 52 Z 1 from July 1, 2020 - December 31, 2020 | Reduced Rate | 5% |  | Both (Sales and Purchases) |
| RC-AT | Reverse charge | Reverse Charge Code | 0% | S-AT | Both (Sales and Purchases) |
| S-AT | Standard rate | \- | 20% | \- | Both (Sales and Purchases) |
| S2-AT | Standard rate - other (Jungholz and Mittelberg) | Special Territory | 19% | \- | Both (Sales and Purchases) |
| Z-AT | Zero rated sales | \- | 0% | \- | Sales |

## Supported Tax Codes {#subsect_59093951013}

The following tax codes aren't provisioned by the International Tax Reports SuiteApp but supported in NetSuite. You can create the following tax codes for Austria and use it for tax reporting. For more information about creating new tax codes, see [Creating Tax Codes - Other Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html).

| Tax Code | Property | Available On | Category |
| --- | --- | --- | --- |
| D-AT | Customs Duty | Both (Sales and Purchases) | S0 (None) |
| DP-AT | Paid Customs Duty | Both (Sales and Purchases) | S0 (None) |
| EG-AT | EC Code | Both (Sales and Purchases) | S1 (Fixed Asset) |
| EK-AT | EC Code | Both (Sales and Purchases) | S2 (Other Goods and Services) |
| G-AT | \- | Both (Sales and Purchases) | S1 (Fixed Asset) |
| K-AT | \- | Both (Sales and Purchases) | S2 (Other Goods and Services) |

## Tracking VAT Paid on Imports into Austria {#bridgehead_N1825737}

Quite often, the customs office levies VAT on imports at the border crossing (inland or airports). This levy is paid either by the transporter before the goods are released, or by you directly on an account basis. These costs are basically 100% VAT bills. To make sure NetSuite picks up these taxes when you generate the VAT report for Austria, you should use the following tax codes:

| Tax Code | Description | Property | Rate | Notional Rate | Applies To |
| --- | --- | --- | --- | --- | --- |
| Import VAT-P | VAT paid to Customs on imports | Paid Import VAT | 0% | \- | Purchases |
| Import VAT-U | VAT not yet paid on imports | Import VAT | 0% | \- | Purchases |

When entering the transaction, you must record this cost as input tax, where the total amount represents the VAT amount. The full tax amount shown on the vendor bill must be entered in the Net Amount field (bills or journals).

The following lists examples of how you can use the tax codes:

-   In most cases, at the point of import (at the border, or airport, or customs house), the customs office will value the goods and impose VAT, that your company must pay before the goods are released. You can record this input tax using the **Import VAT-P** (VAT paid) tax code. The net amount for this tax will be picked up in box 61 of the Austrian VAT report.
    
-   Sometimes, the freight or transport company will pay the VAT to customs for you, then passes the charge to you. You can record this input tax using the **Import VAT-P** (VAT paid) tax code. The net amount for this tax will be picked up in box 83 of the Austrian VAT report.
    
-   Other times, the customs office bills your company, and you pay the VAT bill like any other vendor bill. You can record this input tax using the **Import VAT-U** (VAT unpaid) tax code.
    

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Setting Up Tax Filing for Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1826176.html)
-   [Austria VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1826422.html)
-   [What goes into each box - Austria VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1826752.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
