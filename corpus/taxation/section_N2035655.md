---
id: "section_N2035655"
type: "section"
title: "Uruguay Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Uruguay Tax Topics > Uruguay Tax Codes"
parent: "chapter_N2035552"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2035655.html"
anchors: ["subsect_1030044330", "bridgehead_N2035714"]
sha256: "39d59a03479389a1de3922d9341917b90774d1cf4795e41488e9a8e6af0d065e"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Uruguay are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030044330}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Uruguay {#bridgehead_N2035714}

The following table shows the tax properties required to correctly generate the Uruguay tax report provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Rate | Property | Tax Type | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- | --- |
| E-UY | IVA Exempt | 0% | Exempt | IVA\_UY | VAT on Purchases UY | VAT on Sales UY | Both (Sales and Purchases) |
| I-UY | IVA Import | 22% | Import | IVA\_UY | VAT on Purchases UY |  | Purchases |
| IE-UY | IVA Import Exempt | 0% | Import Exempt | IVA\_UY | VAT on Purchases UY |  | Purchases |
| R-UY | Reduced IVA Rate | 10% | Reduced Rate | IVA\_UY | VAT on Purchases UY | VAT on Sales UY | Both (Sales and Purchases) |
| S-UY | Standard IVA Rate | 22% | Default Code | IVA\_UY | VAT on Purchases UY | VAT on Sales UY | Both (Sales and Purchases) |
| SS-UY | IVA Suspended | 0% | Suspended | IVA\_UY | VAT on Purchases UY | VAT on Sales UY |  |
| X-UY | IVA Export | 0% | Export | IVA\_UY |  | VAT on Sales UY | Sales |
| XE-UY | IVA Export Exempt | 0% | Export Exempt | IVA\_UY |  | VAT on Sales UY | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Uruguay Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2035655.html)
-   [Uruguay VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038372.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
