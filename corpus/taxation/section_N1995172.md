---
id: "section_N1995172"
type: "section"
title: "South Africa Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > South Africa Tax Topics > South Africa Tax Codes"
parent: "chapter_N1995074"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1995172.html"
anchors: ["subsect_1030040515", "bridgehead_N1995231"]
sha256: "63500691c5cdb69e6570059abf745cf4345d1a500d42abc39539f1f8efb93797"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for South Africa are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030040515}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for South Africa {#bridgehead_N1995231}

The following table shows the tax properties required to correctly generate the tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Available On |
| --- | --- | --- | --- | --- |
| E-ZA | VAT exempt sales | Exempt | 0% | Both (Sales and Purchases) |
| I-ZA | Imports | Import | 0% | Purchases |
| O-ZA | Exports | Export | 0% | Sales |
| S-ZA | Standard rate | \- | 15% | Both (Sales and Purchases) |
| SC-ZA | Standard rate - capital goods | Capital Goods | 15% | Both (Sales and Purchases) |
| Z-ZA | Zero rate | \- | 0% | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [South Africa VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1995782.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
