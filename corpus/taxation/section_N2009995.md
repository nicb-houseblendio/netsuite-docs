---
id: "section_N2009995"
type: "section"
title: "Switzerland Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Switzerland Tax Topics > Switzerland Tax Codes"
parent: "chapter_N2009888"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2009995.html"
anchors: ["subsect_1030041900", "bridgehead_N2010054"]
sha256: "fa168307542341d160e6e47740847a943cf6d66d7c8614a67b7c01daaea96e0c"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Switzerland are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030041900}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes aren't used in the same tax period.
    

## Tax Code Table for Switzerland {#bridgehead_N2010054}

The following table shows the tax properties required to correctly generate the Switzerland tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Switzerland VAT report, [What goes into each box - Switzerland VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4115270565.html).

Important:

Consult your tax agency for the correct tax rates.

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-CH | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| IV-CH | 100% Input VAT at customs | Import | 0% | \- | Purchases |
| R2-CH | Reduced rate | Reduced Rate | 2.6% | \- | Both (Sales and Purchases) |
| RC-CH | Reverse charge in country | Reverse Charge Code | 0% | S-CH | Both (Sales and Purchases) |
| S-CH | Standard rate | \- | 8.1% | \- | Both (Sales and Purchases) |
| SR-CH | Special reduced rate | Special Reduced Rate | 3.8% | \- | Both (Sales and Purchases) |
| Z-CH | Zero rated sales | \- | 0% | \- | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Switzerland VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2010657.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
