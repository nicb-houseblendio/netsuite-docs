---
id: "section_N2018677"
type: "section"
title: "Thailand Tax Codes"
branch: "thailand-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Thailand Help Topics > Thailand Tax Topics > Thailand Tax Codes"
parent: "chapter_N2018510"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2018677.html"
anchors: ["subsect_1030043100", "bridgehead_N2018736"]
sha256: "769ee347625215ff2d573c62ebe2e7669fd3376b353fdb0d70a6888d3b226929"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Thailand are set up correctly.

For more information on tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030043100}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Thailand {#bridgehead_N2018736}

The following table shows the tax properties required to correctly generate the Thailand tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Value Added Tax Return for Thailand, see [What goes into each box - Thailand VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2020046.html).

Note:

Tax type should be set to VAT.

| Tax Code | Description | Rate | Property | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- |
| EX-TH | Exempt sales or purchases | 0% | Exempt | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| S-TH | Standard rate | 7% | Default | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| UNDEF\_TH | Used when NetSuite cannot determine the appropriate tax code for a transaction | 0% | Exclude from VAT reports | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| Z-TH | Zero rates sales | 0% | Export | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Thailand VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2019313.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
