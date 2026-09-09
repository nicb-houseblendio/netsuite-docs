---
id: "section_N1956367"
type: "section"
title: "What goes into each box - Philippines Monthly VAT Form 2550M"
branch: "philippines-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Philippines Help Topics > Philippines Tax Topics > VAT Reports - Philippines > Monthly and Quarterly VAT Reports for the Philippines > What goes into each box - Philippines Monthly VAT Form 2550M"
parent: "bridgehead_N1955366"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1956367.html"
anchors: []
sha256: "27515f1dc036429022871d95e2e7f45cd70cc46b0938ec7e7c6694cf13450c72"
---

Refer to the following table to understand how NetSuite uses the tax codes to get the values for the **Monthly Value-Added Tax Declaration form 2550M**.

| Monthly Value-Added Tax Declaration 2550M | Sales/Receipts (VAT exclusive) |  | Output Tax Due |
| --- | --- | --- | --- |
| 12 | Vatable sales/receipts - private | 12A | S-PH | 12B | S-PH + Tax amount of sales adjustment of box12b, S-PH |
| 13 | Sales to government | 13A | G-PH | 13B | G-PH + Tax amount of sales adjustment of box13b, G-PH |
| 14 | Zero rated sales/receipts | 14 | Z-PH |  |  |
| 15 | Exempt sales/receipts | 15 | EX-PH |  |  |
| 16 | Total sales/receipts and output tax due | 16A | 12A+13A+14+ 15 | 16B | 12B+13B |
| 17 | Less: Allowable input tax |
|  | 17A | Input tax carried over from previous period | 17A | Editable field |
|  | 17B | Input tax deferred on capital goods exceeding P1M from previous period | 17B | Editable field |
|  | 17C | Transitional input tax | 17C | Editable field |
|  | 17D | Presumptive input tax | 17D | Editable field |
|  | 17E | Others | 17E | Editable field |
|  | 17F | Total | 17F | 17A+17B+ 17 C+17D+17E |
| 18 | Current transactions |  | Purchases |
|  | 18A/B | Purchase of capital goods not exceeding P1M | 18A | CAP-PH (if <= P1M) | 18B | CAP-PH + Tax amount of purchase adjustment box18b, CAP-PH |
|  | 18C/D | Purchase of capital goods exceeding P1M | 18C | CAP-PH (if > P1M) | 18D | Editable field |
|  | 18E/F | Domestic purchase of goods other than capital goods | 18E | S-PH | 18F | S-PH + Tax amount of purchase adjustment box18f, S-PH |
|  | 18G/H | Importation of goods other than capital goods | 18G | IMPT-PH | 18H | IMPT-PH + Tax amount of purchase adjustment box18h, IMPT-PH |
|  | 18I/J | Domestic purchase of services | 18I | SVC-PH | 18J | SVC-PH + Tax amount of purchase adjustment box18j, SVC-PH |
|  | 18K/L | Services rendered by non residents | 18K | SVCA-PH | 18L | SVCA-PH + Tax amount of purchase box18l, SVCA-PH |
|  | 18M | Purchases not qualified for input tax | 18M | EX-PH, Z-PH |  |
|  | 18N/O | Others | 18N | Editable field | 18O | Editable field |
|  | 18P | Total current purchases | 18P | 18A+18C+18E+18G+18I+ 18K+18M+ 18N |  |  |
| 19 | Total available input tax | 19 | 17F+18B+18D18F+18H+ 18J+18L+18O |
| 20 | Less: Deductions from input tax |
|  | 20A | Input tax on purchases of capital goods exceeding P1Million | 20A | Editable field |
|  | 20B | Input tax on sales to government closed to expense | 20B | Editable field |
|  | 20C | Input tax allocable to exempt sales | 20C | Editable field |
|  | 20D | VAT refund/TCC claimed | 20D | Editable field |
|  | 20E | Others | 20E | Editable field |
|  | 20F | Total | 20F | 20A+20B+ 20C+20D+ 20E |
| 21 | Total allowable input tax | 21 | 19 - 20F |
| 22 | Net VAT payable | 22 | 16B - 21 |
| 23 | Less: Tax credits/payments |
|  | 23A | Creditable value-added tax withheld | 23A | Editable field |
|  | 23B | Advance payments of sugar and flour industries | 23B | Editable field |
|  | 23C | VAT withheld on sales to government | 23C | Editable field |
|  | 23D | VAT paid in return previously filed, if this is an amended return | 23D | Editable field |
|  | 23E | Advance payments made | 23E | Editable field |
|  | 23F | Others | 23F | Editable field |
|  | 23G | Total tax credits/payments | 23G | 23A+23B+23C+23D+23E+23F |
| 24 | Tax still payable/(Overpayment) | 24 | 22-23G |
| 25 | Add penalties: |
|  |  |  | Surcharge |  | Interest |  | Compromise |  |  |
|  |  | 25A | Editable field | 25B | Editable field | 25C | Editable field | 25D | 25A+25B+ 25C |
| 26 | Total amount payable/(Overpayment) | 26 | 24+25D |

### Related Topics

-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Philippines Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1952432.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [Philippines Quarterly VAT Form 2550Q](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0226025159.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
