---
id: "section_N1940638"
type: "section"
title: "Mexico Tax Codes (Mexico Compliance SuiteApp)"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Mexico Tax Topics (Mexico Compliance SuiteApp) > Mexico Tax Codes (Mexico Compliance SuiteApp)"
parent: "chapter_N1940317"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1940638.html"
anchors: ["bridgehead_N1940696"]
sha256: "9e40a2557d16781d0b6cc3fb651cfb40aeece649eeef1dcf4fd3d0b5bc223e9b"
---

Tax codes determine how much tax is paid on each transaction line item. Make sure that the properties and rates of your tax codes are correct.

Note:

The tax code properties required for Mexico tax codes are provided by the International Tax Reports SuiteApp.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Tax Code Table for Mexico {#bridgehead_N1940696}

Note:

The tax code properties required for Mexico tax codes are provided by the International Tax Reports SuiteApp.

The following table shows the tax properties required to generate the [Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html). The tax code names or letters used in the following table are suggested names or default system preferences. You can rename the tax codes.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. To understand how NetSuite uses the tax codes to get the values for DIOT reporting, see [Tax Code Mapping for Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3738825237.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Rate | Property | Tax Type | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- | --- |
| S-MX | Standard default tax rate for sales and purchases of goods and services traded/provided in Mexico, except for the bordering region | 16% | Default Code | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| R-MX | Reduced tax rate for sales and purchases of goods and services traded/provided in Mexico for specific regions. | 8% | Reduced Rate | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| Z-MX | Zero IVA rate for specifically defined goods and services | 0% | Special Reduced Rate | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| E-MX | Transactions exempt of IVA | 0% | Exempt | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| IS-MX | Standard IVA on import | 16% | Import | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| IR-MX | Reduced IVA on import | 11% | Import Reduced Rate | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| IZ-MX | Zero IVA rate on import | 0% | Import Special Reduced Rate | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| IE-MX | IVA Exempt on import | 0% | Import Exempt | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| ZX-MX | Zero IVA rate for export transactions | 0% | Export | VAT\_MX | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
|  |  |  |  |  |  |  |  |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Mexico Tax Setup (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941750.html)
-   [Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html)
-   [Tax Code Mapping for Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3738825237.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
