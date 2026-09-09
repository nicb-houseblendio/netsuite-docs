---
id: "section_N1989642"
type: "section"
title: "Slovakia Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Slovakia Tax Topics > Slovakia Tax Codes"
parent: "chapter_N1989528"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989642.html"
anchors: ["subsect_1030040035", "bridgehead_N1989701", "bridgehead_N1991668"]
sha256: "2d64699a4d18549646ca2aae75d0121cc85ba3a9662ce5c199be46bc5542bf80"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Slovakia are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030040035}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Slovakia {#bridgehead_N1989701}

The following table shows the tax properties required to correctly generate the Slovakia tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Poland VAT report, see [What goes into each box - Slovakia VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3932968818.html).

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-SK | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-SK | EU sales/purchases (goods) - reduced rate | EC Code Reduced Rate | 0% | R-SK | Both (Sales and Purchases) |
| ERND-SK | EU purchases (goods) - reduced rate (nondeductible) | EC Code Reduced Rate Nondeductible | 0% | R-SK | Purchases |
| ES-SK | EU sales/purchases (goods) | EC Code | 0% | S-SK | Both (Sales and Purchases) |
| ESND-SK | EU purchases (goods) - nondeductible | EC Code Nondeductible | 0% | S-SK | Purchases |
| ESSP-SK | EU purchases (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-SK | Purchases |
| ESSPND-SK | EU purchases (services) - nondeductible | EC Code Applies to Service Items Reverse Charge Nondeductible | 0% | S-SK | Purchases |
| ESSS-SK | EU sales (services) | EC Code Applies to Service Items | 0% | S-SK | Sales |
| EZ-SK | EU sales/purchases (goods) - zero rate | EC Code | 0% | Z-SK | Both (Sales and Purchases) |
| I-SK | Purchase of goods from outside of EU | Import VAT | 0% | \- | Purchases |
| IS-SK | Purchase of services from outside of EU | Import Applies to Service Items Reverse Charge Code | 0% | S-SK | Purchases |
| ISND-SK | Purchase of services from outside of EU - nondeductible | Import Applies to Service Items Reverse Charge Nondeductible | 0% | S-SK | Purchases |
| O-SK | Sale of goods outside of EU | Export | 0% | \- | Sales |
| OS-SK | Supply of services outside of EU | Export Applies to Service Items | 0% | \- | Sales |
| R-SK | Reduced rate | Reduced Rate | 10% | \- | Both (Sales and Purchases) |
| RC-SK | Reverse charge | Reverse Charge Code | 0% | S-SK | Sales |
| S-SK | Standard rate | \- | 20% | \- | Both (Sales and Purchases) |
| Z-SK | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

## Tracking VAT Paid on Imports into Slovakia {#bridgehead_N1991668}

Often, the customs office levies VAT on imports at the border crossing (inland or airport). This levy is paid either by the transporter before the goods are released, or by you directly on an account basis. These costs are basically 100% VAT bills. To make sure NetSuite picks up these taxes when you generate the VAT report for Slovakia, you should use the following tax codes:

| DUTY-P | Import VAT - paid | Paid Import VAT | Purchases |
| --- | --- | --- | --- |
| DUTY-U | Import VAT - unpaid | Import VAT | Purchases |
| DUTY-PR | Import VAT - paid (reduced rate) | Paid Import VAT Reduced Rate | Purchases |
| DUTY-UR | Import VAT - unpaid (reduced rate) | Import VAT Reduced Rate | Purchases |

When entering the transaction, you must record this cost as input tax, where the total amount represents the VAT amount. The full tax amount shown on the vendor bill must be entered in the Net Amount field (bills or journals).

The following lists examples of how you can use the tax codes:

-   In most cases, at the point of import (at the border, or airport, or customs house), the customs office values the goods and impose VAT that your company must pay before the goods are released. You can record this input tax using the **DUTY-P** tax code for import VAT paid on standard rate purchases. For import VAT paid on reduced rate purchases, you can use the **DUTY-PR** tax code.
    
-   Sometimes, the freight or transport company pays the VAT to customs for you, then passes the charge to you. You can record this input tax using the **DUTY-P** tax code for import VAT paid on standard rate purchases. For import VAT paid on reduced rate purchases, you can use the **DUTY-PR** tax code.
    
-   Other times, the customs office bills your company, and you pay the tax bill like any other vendor bill. You can record this input tax using the **DUTY-U** tax code for unpaid import VAT on standard rate purchases. For unpaid import VAT on reduced rate purchases, you can use the **DUTY-UR** tax code.
    

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Slovakia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1992117.html)
-   [What goes into each box - Slovakia VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3932968818.html)
-   [Slovakia VAT Ledger Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4497423773.html)
-   [What goes into each box - Slovak VAT Ledger Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4524799494.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
