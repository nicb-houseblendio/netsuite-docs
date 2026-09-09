---
id: "section_N1996096"
type: "section"
title: "South Korea Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > South Korea Tax Topics > South Korea Tax Codes"
parent: "chapter_N1995977"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1996096.html"
anchors: ["subsect_1030040608", "bridgehead_N1996151"]
sha256: "a913e2a8937d56b8ea71d6f41cbafcdca451435c89a2f26ab3a3e2f5b38bae02"
---

Tax codes determine how much tax is paid on each transaction line item. To make sure NetSuite calculates correct values on transaction records and tax reports, ensure the tax codes for South Korea are set up correctly.

For more details on tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030040608}

-   The International Tax Reports SuiteApp supports up to 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for South Korea {#bridgehead_N1996151}

The following table lists the tax properties needed to generate South Korea tax reports with the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes if you'd like. Tax reports identify transactions based on tax code properties, not tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Note:

Tax type should be set to VAT.

To understand how NetSuite uses the tax codes to get the values for the General Value-Added Tax Return form for the Republic of Korea, see [What goes into each box - South Korea VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1997819.html).

| Tax Code | Description | Rate | Property | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- |
| CAP-KR | Purchase of capital goods | 10% | Capital Goods | VAT on Purchases | VAT on Sales | Purchases |
| EX-KR | VAT exempt transactions | 0% | Exempt | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| S-KR | Sales or Purchases for which tax invoices were used | 10% | Default | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| SO-KR | Sales or Purchases where the issuance of tax invoices are not required | 10% | No tax invoice | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| SP-KR | Sales or Purchases where the tax invoice was issued by the purchaser | 10% | Purchaser Issued | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| UNDEF\_KR | Used when NetSuite cannot determine the appropriate tax code for a transaction | 0% | Exclude from VAT reports | VAT on Purchases | VAT on Sales | Both (Sales and Purchases) |
| Z-KR | Zero-rated sales for which tax invoices were issued | 0% | Export | VAT on Purchases | VAT on Sales | Sales |
| ZO-KR | Zero-rated sales for which tax invoices are not required | 0% | Export No tax invoice | VAT on Purchases | VAT on Sales | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [South Korea VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1997044.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
