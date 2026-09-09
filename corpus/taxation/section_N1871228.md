---
id: "section_N1871228"
type: "section"
title: "Colombia Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Colombia Tax Topics > Colombia Tax Codes"
parent: "chapter_N1867954"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1871228.html"
anchors: ["subsect_1030013247", "bridgehead_N1871292"]
sha256: "702f67a5ebbebab330ff76b96f255f1c9b31ed7734fdf6e16f8d44da9f1bb772"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Colombia are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030013247}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Colombia {#bridgehead_N1871292}

Important:

Tax codes and tax rates for Colombia have changed for 2013. Be sure to edit your pre-2013 tax code records and set the Valid Until date to 31 December 2012. For 2013 transactions, create the following new tax codes with an Effective From date of 1 January 2013.

The following table shows the tax properties required to correctly generate the Colombia VAT report provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Colombia VAT report, see [What goes into each box - Colombia VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775975736.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Rate | Property | Tax Type | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- | --- |
| E-CO | IVA Exempt | 0% | Exempt | IVA\_CO | IVA on Purchases | IVA on Sales | Both (Sales and Purchases) |
| I-CO | IVA Import | 19% | Import | IVA\_CO | IVA on Purchases |  | Purchases |
| I5-CO | IVA Import - Reduced Rate | 5% | Import Reduced Rate | IVA5\_CO | IVA on Purchases |  | Purchases |
| IS-CO | IVA Import - Services (reduced rate) | 5% | Import Applies to Service Items Reduced Rate | IVA5\_CO | IVA on Purchases |  | Purchases |
| N-CO | Non Taxable | 0% | Non-Taxable | IVA\_CO | IVA on Purchases | IVA on Sales | Both (Sales and Purchases) |
| NI-CO | Non Operational Import | 0% | Non-Taxable Import | IVA\_CO | IVA on Purchases |  | Purchases |
| NT-CO | No Tax Credit | 0% | No Tax Credit | IVA\_CO |  | IVA on Sales | Sales |
| S-CO | IVA Default | 19% |  | IVA\_CO | IVA on Purchases | IVA on Sales | Both (Sales and Purchases) |
| S5-CO | IVA Reduced Rate | 5% | Reduced Rate | IVA5\_CO | IVA on Purchases | IVA on Sales | Both (Sales and Purchases) |
| S5S-CO | IVA Reduced Rate - Services | 5% | Applies to Service Items Reduced Rate | IVA5\_CO | IVA on Purchases |  | Purchases |
| SB-CO | Special IVA rate - Beer | 19% | Category: Beer | IVA\_CO |  | IVA on Sales | Sales |
| SG-CO | Special IVA rate - Game of chance | 19% | Category: Gambling | IVA\_CO |  | IVA on Sales | Sales |
| SS-CO | IVA Default - Services | 19% | Applies to Service Items | IVA\_CO | IVA on Purchases |  | Purchases |
| X-CO | IVA Export | 0% | Export | IVA\_CO |  | IVA on Sales | Sales |
| XS-CO | IVA Export - Services | 0% | Export Applies to Service Items | IVA\_CO |  | IVA on Sales | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Colombia Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1868140.html)
-   [Colombia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1872768.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
