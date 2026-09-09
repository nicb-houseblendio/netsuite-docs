---
id: "section_N2021408"
type: "section"
title: "Türkiye Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Türkiye Tax Topics > Türkiye Tax Codes"
parent: "chapter_N2021231"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2021408.html"
anchors: ["subsect_1030043203", "bridgehead_N2021467"]
sha256: "d1c2af5cb39da944b465eaa1b14bedffa328e4974ffb108d8a90db9e076c70d0"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Türkiye are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030043203}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Türkiye {#bridgehead_N2021467}

The following table shows the tax properties required to correctly generate the Türkiye tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Consult your tax agency for the correct tax rates.

Note:

Tax type should be set to VAT.

| Tax Code | Description | Property | Rate | Available On |
| --- | --- | --- | --- | --- |
| E-TR | Exempted Goods | \- | 0% | Sales |
| O-TR | Exports | Export | 18% | Sales |
| OR-TR | Reduced Rate Exports | Reduced Rate Export | 8% | Sales |
| R-TR | Reduced Rate | Reduced Rate | 8% | Both (Sales and Purchases) |
| RC-TR | Reverse Charge | Export Applies to Service Items | 18% | Purchases |
| S-TR | Standard Rate | \- | 18% | Both (Sales and Purchases) |
| SR-TR | Super Reduced Rate | Special Reduced Rate | 1% | Both (Sales and Purchases) |
| ZR-TR | Zero Rated Exports | Export | 0% | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Türkiye VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2022385.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
