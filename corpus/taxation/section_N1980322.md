---
id: "section_N1980322"
type: "section"
title: "Serbia Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Serbia Tax Topics > Serbia Tax Codes"
parent: "chapter_N1980213"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1980322.html"
anchors: ["subsect_1030035519", "bridgehead_N1980381"]
sha256: "5f756d8d075c1782a9d503151d00c73a8c45aaa2dbbaab219d733e490e6c9abd"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Serbia are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030035519}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Serbia {#bridgehead_N1980381}

The following table shows the tax properties required to correctly generate the Serbia tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-RS | Exempt | Exempt | \- | \- | Both (Sales and Purchases) |
| I-RS | Imports | Import | 20% | \- | Purchases |
| IS-RS | Import of service items | Applies to Service Items Import | \- | \- | Purchases |
| O-RS | Exports | Export | \- | \- | Sales |
| R-RS | Reduced rate | Reduced Rate | 10% | \- | Both (Sales and Purchases) |
| RC-RS | Reverse Charge | Reverse Charge | 0% | S-RS | Purchases |
| S-RS | Standard rate | \- | 20% | \- | Both (Sales and Purchases) |
| Z-RS | Zero rated | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Serbia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981048.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
