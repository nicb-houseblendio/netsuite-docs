---
id: "section_N1997819"
type: "section"
title: "What goes into each box - South Korea VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > South Korea Tax Topics > South Korea VAT Report > What goes into each box - South Korea VAT report"
parent: "section_N1997044"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1997819.html"
anchors: []
sha256: "424fd6e0110933ae68f6d98b2ab5567a9e086293572b0711fee7d3a549324c76"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page is not supported. If you'd like to create nondeductible tax codes that work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the General Value-Added Tax Return form for the Republic of Korea.

| Box | Net Amount | Tax Amount |
| --- | --- | --- |
| Tax base and sales tax |
| 1 | Tax invoice issued | S | S |
| 2 | Tax invoice issued by purchaser | SP | SP |
| 3 | Other | SO | SO |
| 4 | Tax invoice issued (zero rate) | Z |  |
| 5 | Other (zero rate) | ZO |
| 6 | Omitted preliminary return | Editable field | Editable field |
| 7 | Bad debts tax credits | Editable field |
| 8 | Total | 1+2+3+4+5+6 | 1+2+ 3+6+7 |
| Purchase tax |
| 9 | Tax invoice received (general purchase) | S | S |
| 10 | Tax invoice received (fixed asset purchase) | CAP | CAP |
| 11 | Omitted preliminary return | Editable field | Editable field |
| 12 | Tax invoice issued by purchaser | SP | SP |
| 13 | Other purchase tax deduction | SO | SO |
| 14 | Total | 9+10+ 11+12+13 | 9+10+ 11+12+13 |
| 15 | Purchase tax amount not deductible | Editable field | Editable field |
| 16 | Amount deducted | 14 - 15 | 14 - 15 |
|  | Tax amount due (total sales tax amount minus total purchase tax amount) | 8 - 14 |
| Reduced rate |
| 17 | Other reduced rate deduction | Editable field |
| 18 | Tax credit on cash receipt issuer, etcetera. | Editable field |
| 19 | Total | 17+18 |
| 20 | Preliminary return tax amount not refunded | Editable field |
| 21 | Preliminary return tax noticed | Editable field |
| 22 | Special VAT on gold metal trade | Editable field |
| 23 | Penalty total | Editable field |
| 24 | Payable tax amount after deduction and addition (refundable tax amount) | Tax amount due - Total reduced rate - 20-21-22+23 |
|  | Payable tax amount of combined payment (refundable tax) | Sum of all payable tax amounts for all subsidiaries + parent company |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [South Korea Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1996096.html)
-   [South Korea VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1997044.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
