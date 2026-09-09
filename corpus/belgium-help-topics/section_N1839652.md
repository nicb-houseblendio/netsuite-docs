---
id: "section_N1839652"
type: "section"
title: "Belgium Tax Codes"
branch: "belgium-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Belgium Help Topics > Belgium Tax Topics In Accounts Without SuiteTax > Belgium Tax Codes"
parent: "section_156742725505"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1839652.html"
anchors: ["subsect_1030011921", "bridgehead_N1839711", "bridgehead_N1841349", "bridgehead_3824087098"]
sha256: "f3db9a37938c114d253d58b4bbd0441b3798d2e53dd51efc13b642b6e0651d77"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Belgium are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030011921}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Belgium {#bridgehead_N1839711}

The following table shows the tax properties required to correctly generate the Belgium tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-BE | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| E2-BE | Purchase of services - exempt | Exempt Applies to Service Items | 0% | \- | Both (Sales and Purchases) |
| ECFA-BE | EC Investment assets | EC Code Category: Investment | 0% | FA-BE | Both (Sales and Purchases) |
| EDCSP-BE | Purchase of direct cost service items within EC | Applies to Direct Cost Service Items EC Code Reverse Charge Code | 0% | S-BE | Purchases |
| EP-BE | EC Property | EC Code Category: Property/Other Assets | 0% | S-BE | Both (Sales and Purchases) |
| ER-BE | EC sales/purchases within EC (goods) - reduced rate | EC Code Reduced Rate | 0% | R-BE | Both (Sales and Purchases) |
| ES-BE | EC sales and purchases (goods) | EC Code | 0% | S-BE | Both (Sales and Purchases) |
| ESSP-BE | Purchase of services within EC | EC Code Applies to Service Items Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| ESSS-BE | EC Sales (services) | EC Code Applies to Service Items Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| EZ-BE | EC sales/purchases - zero rate | EC Code | 0% | Z-BE | Both (Sales and Purchases) |
| FA-BE | Investment assets | Category: Investment | 21% | \- | Both (Sales and Purchases) |
| FA2-BE | Investment assets below the threshold | Category: Investment below the threshold | 21% | \- | Purchases |
| I-BE | Purchase of goods from outside of EC | Import Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| ID-BE | Imports subject to customs duties | Import VAT Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| IS-BE | Purchase of services from outside of EC | Import Applies to Service Items Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| ISND-BE | Reverse Charge Services - Non-deductible | Reverse Charge Code Import Applies to Service Items Nondeductible | 0% | S-BE | Both (Sales and Purchases) |
| IV-BE | 100% VAT bill | Effective from January 1, 2021 Import VAT | 0% | \- | Purchases |
| O-BE | Sales outside of the EU | Export | 0% | \- | Both (Sales and Purchases) |
| OS-BE | Supply of services outside of EC | Export Applies to Service Items Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| R-BE | Reduced rate | Reduced Rate | 12% | \- | Both (Sales and Purchases) |
| RC-BE | Reverse charge | Reverse Charge Code | 0% | S-BE | Both (Sales and Purchases) |
| RCFA-BE | Reverse Charge -Investment | Category: Investment Reverse Charge Code | 0% | FA-BE | Both (Sales and Purchases) |
| RCFAND-BE | Reverse Charge Investment - Non-deductible | Category: Investment Nondeductible Reverse Charge Code | 0% | FA-BE | Both (Sales and Purchases) |
| RCND-BE | Reverse Charge - Non-deductible | Nondeductible Reverse Charge | 0% | S-BE | Both (Sales and Purchases) |
| RS-BE | Reduced rate - Service | Reduced Rate Applies to Service Items | 12% | \- | Both (Sales and Purchases) |
| S-BE | Standard rate | \- | 21% | \- | Both (Sales and Purchases) |
| SR-BE | Reduced rate - other | Special Reduced Rate | 6% | \- | Both (Sales and Purchases) |
| SRS-BE | Reduced rate service - other | Special Reduced Rate Applies to Service Items | 6% | \- | Both (Sales and Purchases) |
| SS-BE | Standard rate - Service | Applies to Service Items | 21% | \- | Both (Sales and Purchases) |
| Z-BE | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

## Tracking VAT Paid on Imports into Belgium {#bridgehead_N1841349}

You should have a tax code for imports that are subject to VAT (refer to tax code IV in the tax code table). When recording the type of bill (which is a 100% VAT bill), ensure that you record this import VAT as input tax, where the net amount represents the VAT amount. NetSuite reports the full tax amount in box 57 of the VAT report for Belgium.

## Tracking Nondeductible Input Tax for Belgium {#bridgehead_3824087098}

For guidance on setting up tax codes for nondeductible input tax, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

Important:

The tax code for the nondeductible portion of the VAT and the tax code for the reclaimable portion should have the same tax properties. For example, if the Reduced Rate property applies, then both tax codes should have the Reduced Rate box checked.

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Setting Up Tax Filing for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1841509.html)
-   [Belgium VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1843546.html)
-   [What goes into each box - Belgium VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1843870.html)
-   [EU Sales List for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1846111.html)
-   [Intrastat Report for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1552962932.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
