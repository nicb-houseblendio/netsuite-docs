---
id: "section_N2022864"
type: "section"
title: "Ukraine Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Ukraine Tax Topics > Ukraine Tax Codes"
parent: "chapter_N2022755"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2022864.html"
anchors: ["subsect_1030043536", "bridgehead_N2022923"]
sha256: "d78209b93925767df093eb5e68bd57b137ae6fd5ddf8d7031a03668a692973e6"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Ukraine are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030043536}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Ukraine {#bridgehead_N2022923}

The following table shows the tax properties required to correctly generate the Ukraine tax report provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Available On |
| --- | --- | --- | --- | --- |
| CGNT-UA | Capital goods - non taxable | Non Taxable Capital Goods | 0% | Purchases |
| CGS-UA | Capital goods - standard rate | Capital Goods | 20% | Purchases |
| CGZ-UA | Capital goods - zero rate | Capital Goods | 0% | Purchases |
| E-UA | VAT exempt sales | Exempt | \- | Sales |
| IE-UA | VAT exempt imports | Exempt Import | 0% | Purchases |
| IS-UA | Imports with VAT | Import | 20% | Purchases |
| NRS-UA | Purchases from non residents - not recoverable | Non Resident Non Recoverable | 20% | Purchases |
| NRZ-UA | Purchases from non residents - not recoverable, zero rate | Non Resident Non Recoverable | 0% | Purchases |
| NT-UA | Non taxable transactions in country | Non Taxable | 0% | Both (Sales and Purchases) |
| NTI-UA | Non taxable imports | Non Taxable Import Non Resident | 0% | Purchases |
| NTS-UA | Non taxable services received from non residents | Non Taxable Applies to Service Items Non Resident | 0% | Purchases |
| O-UA | Exports | Export | 0% | Sales |
| S-UA | Standard rate | \- | 20% | Both (Sales and Purchases) |
| SS-UA | In country services received from non residents | Applies to Service Items Non Resident | 20% | Purchases |
| SSO-UA | Services provided outside the customs territory of Ukraine | Applies to Service Items Outside Customs Territory | \- | Sales |
| Z-UA | Zero rate | \- | 0% | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Ukraine VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2025824.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
