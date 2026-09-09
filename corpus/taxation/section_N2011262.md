---
id: "section_N2011262"
type: "section"
title: "Taiwan (Province of China) Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Taiwan (Province of China) Tax Topics > Taiwan (Province of China) Tax Codes"
parent: "chapter_N2010868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2011262.html"
anchors: ["subsect_1030042314", "bridgehead_N2011321"]
sha256: "2bc17270ee71b3ad6dc9424b089e92a243adc707485a57c81138a968cbcb82e6"
---

Tax codes determine how much tax is paid on each transaction line item. To make sure NetSuite calculates correct values on transaction records and tax reports, ensure the tax codes for Taiwan (Province of China) are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030042314}

-   The International Tax Reports SuiteApp supports up to 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Taiwan (Province of China) {#bridgehead_N2011321}

The following table lists the tax properties needed to generate Taiwan (Province of China) tax reports with the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes if you'd like. Tax reports identify transactions based on tax code properties, not tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To see how NetSuite uses tax codes to get values for the Declaration of Sales and Business Tax by a Business Entity (401), see [What goes into each box - Taiwan (Province of China) VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2014002.html).

Note:

Tax type should be set to VAT.

| Tax Code | Description | Rate | Property | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- |
| BT-TW | Business Tax thorugh the Customs Payment Certificate Deduction Copy | 5% | Import No Tax Invoice | VAT on Purchases | VAT on Sales | Purchases |
| BTF-TW | Business Tax through the Customs Payment Certificate Deduction Copy for Fixed Asset Purchases | 5% | Import No Tax Invoice Capital Goods | VAT on Purchases | VAT on Sales | Purchases |
| D-TW | Uniform Invoice-Duplicate Invoice | 5% | Duplicate Invoice | VAT on Purchases | VAT on Sales | Sales |
| DCR-TW | Uniform Invoice-Cash Register Invoice (Duplicate Type) | 5% | Duplicate Invoice Cash Register | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| DCRF-TW | Uniform Invoice-Cash Register Invoice (Duplicate Type) for Fixed Asset Sales | 5% | Duplicate Invoice Cash Register Capital Goods | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| DF-TW | Uniform Invoice-Duplicate Invoice for Fixed Assets Sales | 5% | Duplicate Invoice Capital Goods | VAT on Purchases | VAT on Sales | Sales |
| EX-TW | VAT exempt transactions | 0% | Exempt | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| FSVC-TW | Purchase of Foreign Service | 5% | Applies to Service Items Import | VAT on Purchases | VAT on Sales | Purchases |
| IMPT-TW | Imported Goods |  | Import | VAT on Purchases | VAT on Sales | Purchases |
| NU-TW | Non-uniform Invoice | 5% | No Tax Invoice | VAT on Purchases | VAT on Sales | Sales |
| NUF-TW | Non-uniform invoice for Fixed Asset Sales/Purchases | 5% | No Tax Invoice Capital Goods | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| NUZ-TW | Non-uniform Invoice, Zero-rated Sales | 0% | Exports No Tax Invoice | VAT on Purchases | VAT on Sales | Sales |
| OTE-TW | Other tax carried evidence | 0% | Other Tax Evidence | VAT on Purchases | VAT on Sales | Purchases |
| OTEF-TW | Other tax carried evidence for Fixed Asset Purchases | 0% | Capital Goods Other Tax Evidence | VAT on Purchases | VAT on Sales | Purchases |
| T-TW | Uniform Invoice-Triplicate Invoice/Computer Invoice | 5% | Triplicate Invoice | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| TCR-TW | Uniform Invoice-Cash Register Invoice (Triplicate Type) | 5% | Triplicate Invoice Cash Register | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| TCRF-TW | Uniform Invoice-Triplicate Cash Register Invoice for Fixed Asset Purchases | 5% | Triplicate Invoice Cash Register Capital Goods | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| TCRZ-TW | Zero-rated Sales from Cash Registers (Triplicate Type) | 0% | Exports Triplicate Invoice Cash Register | VAT on Purchases | VAT on Sales | Sales |
| TF-TW | Uniform Invoice-Triplicate Invoice/Computer Invoice for Fixed Asset Sales/Purchases | 5% | Triplicate Invoice Capital Goods | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| UNDEF\_TW | Used when NetSuite cannot determine the appropriate tax code for a transaction | 0% | Exclude from VAT Reports | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| Z-TW | Zero-rated Sales | 0% | Exports | VAT on Purchases | VAT on Sales | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Taiwan (Province of China) VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2013226.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
