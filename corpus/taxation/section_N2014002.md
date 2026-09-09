---
id: "section_N2014002"
type: "section"
title: "What goes into each box - Taiwan (Province of China) VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Taiwan (Province of China) Tax Topics > Taiwan (Province of China) VAT Report > What goes into each box - Taiwan (Province of China) VAT report"
parent: "section_N2013226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2014002.html"
anchors: []
sha256: "c50ac638da0a3162781cdce3ca8d8ffb554c21f415cf1cafeed6e6df4025c8b4"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page is not supported. If you'd like to create nondeductible tax codes that work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Taiwan (Province of China) VAT report.

| Box | Tax Codes | Transactions | Amount |
| --- | --- | --- | --- |
| Output (Sales) |
| 1 | Triplicate invoice - computer invoice | T | Sales | Net amount |
| 2 | Triplicate invoice - computer invoice | T | Sales | Tax amount |
| 3 | Zero rate exports not through customs | \- | \- | Editable field |
| 5 | Cash register invoice (triplicate type) | TCR | Sales | Net amount |
| 6 | Cash register invoice (triplicate type) | TCR | Sales | Tax amount |
| 7 | Cash register invoice (triplicate type) - zero rate | TCRZ | Sales | Net amount |
| 9 | Duplicate invoice - cash register invoice (duplicate type) | D, DCR | Sales | Net amount |
| 10 | Duplicate invoice - cash register invoice (duplicate type) | D, DCR | Sales | Tax amount |
| 11 | Zero rate exports through customs | \- | \- | Editable field |
| 13 | Non uniform invoice | NU | Sales | Net amount |
| 14 | Non uniform invoice | NU | Sales | Tax amount |
| 15 | Non uniform invoice (zero rate) | NUZ | Sales | Net amount |
| 17 | Less: returns and allowances (sales amount) | T, TCR, D, DCR, NU | Sales | Editable field but defaults to net amount of Return Transactions |
| 18 | Less: returns and allowances (tax amount) | T, TCR, D, DCR, NU | Sales | Editable field but defaults to tax amount of Return Transactions |
| 19 | Less: returns and allowances (zero rate) | TCRZ, NUZ | Sales | Editable field but defaults to net amount Return Transactions |
| 21 | Total sales amount of taxable sales | \- | \- | 1+5+9 +13-17 |
| 22 | Total tax amount of taxable sales | \- | \- | 2+6+10 +14-18 |
| 23 | Total sales amount of zero-rated sales | \- | \- | 7+15-19 |
| 25 | Sales amount total | \- | \- | 21+23 |
| 27 | Sales amount total, including sales of fixed assets | TF, TCRF, DF, DCRF, NUF | \- | Editable field but defaults to net amount of Sales |
| Input (Purchases) |
| 28 | Uniform invoice deduction copy including computer invoice (purchase and expense) | T | Purchases | Net amount |
| 29 | Uniform invoice deduction copy including computer invoice (purchase and expense) | T | Purchases | Tax amount |
| 30 | Uniform invoice deduction copy including computer invoice (fixed asset) | TF | Purchases | Net amount |
| 31 | Uniform invoice deduction copy including computer invoice (fixed asset) | TF | Purchases | Tax amount |
| 32 | Triplicate cash register (purchase and expense) | TCR | Purchases | Net amount |
| 33 | Triplicate cash register (purchase and expense) | TCR | Purchases | Tax amount |
| 34 | Triplicate cash register (fixed asset) | TCRF | Purchases | Net amount |
| 35 | Triplicate cash register (fixed asset) | TCRF | Purchases | Tax amount |
| 36 | Other tax carried evidence including duplicate cash register invoice (purchase and expense) | DCR, OTE | Purchases | Net amount |
| 37 | Other tax carried evidence including duplicate cash register invoice (purchase and expense) | DCR, OTE | Purchases | Tax amount |
| 38 | Other tax carried evidence including duplicate cash register invoice (fixed asset) | DCRF, OTEF | Purchases | Net amount |
| 39 | Other tax carried evidence including duplicate cash register invoice (fixed asset) | DCRF, OTEF | Purchases | Tax amount |
| 78 | Business tax through the customs payment certificate deduction copy (purchase and expense) | BT | Purchases | Net amount |
| 79 | Business tax through the customs payment certificate deduction copy (purchase and expense) | BT | Purchases | Tax amount |
| 80 | Business tax through the customs payment certificate deduction copy (fixed asset) | BTF | Purchases | Net amount |
| 81 | Business tax through the customs payment certificate deduction copy (fixed asset) | BTF | Purchases | Tax amount |
| 40 | Less: returns and allowances (purchase and expense) | T, TCR, OTE, DCR, BT | Purchases | Editable field but defaults to net amount of Return Transactions |
| 41 | Less: returns and allowances (purchase and expense) | T, TCR, OTE, DCR, BT | Purchases | Editable field but defaults to tax amount of Return Transactions |
| 42 | Less: returns and allowances (fixed asset) | TF, TCRF, OTEF, DCRF, BTF | Purchases | Editable field but defaults to net amount of Return Transactions |
| 43 | Less: returns and allowances (fixed asset) | TF, TCRF, OTEF, DCRF, BTF | Purchases | Editable field but defaults to tax amount of Return Transactions |
| 44 | Total (purchase and expense) | \- | \- | 28+32+36+78-40 |
| 45 | Total (purchase and expense) | \- | \- | 29+33+37+79-41 |
| 46 | Total (fixed asset) | \- | \- | 30+34+38+80-42 |
| 47 | Total (fixed asset) | \- | \- | 31+35+39+81-43 |
| 48 | Total input amount (purchase and expense) | \- | \- | Editable field but defaults to value of box 45 |
| 49 | Total input amount (fixed asset) | \- | \- | Editable field but defaults to value of box 47 |
| 73 | Imported goods | IMPT | Purchases | Net amount |
| 74 | Purchase of foreign services | FSVC | Purchases | Net amount |
| Tax Computation |
| 101 | Current period output tax total | \- | \- | Value of box 22 |
| 107 | Deductible input tax total | \- | \- | 45+47 |
| 108 | Last period accumulated offset against tax payable | \- | \- | Editable field |
| 110 | Subtotal | \- | \- | 107+108 |
| 111 | Current period tax payable | \- | \- | 101 - 110 |
| 112 | Current period offset against tax payable | \- | \- | 110 - 101 |
| 113 | Tax refundable total | \- | \- | (Box 23 x 5%) + Box 47 |
| 114 | Current period tax refundable | \- | \- | Value of box 113 (if box 112 > box 113) or value of box 112 (if box 112 < box 113) |
| 115 | Current period accumulated offset against tax | \- | \- | 112 - 114 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Taiwan (Province of China) Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2011262.html)
-   [Taiwan (Province of China) VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2013226.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
