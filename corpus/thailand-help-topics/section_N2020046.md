---
id: "section_N2020046"
type: "section"
title: "What goes into each box - Thailand VAT report"
branch: "thailand-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Thailand Help Topics > Thailand Tax Topics > Thailand VAT Reports > What goes into each box - Thailand VAT report"
parent: "section_N2019313"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2020046.html"
anchors: []
sha256: "fed290389fb15f3497efe51be82291d3537eead1f07e7a17b7a76410e25da366"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page is not supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Value Added Tax Return for Thailand.

| Box | Tax Codes | Transactions | Amount |
| --- | --- | --- | --- |
| Output tax |  |
| 1 | Sales amount this month | S, Z, EX | Sales | Net amount |
| 2 | Less sales subject to 0% tax rate | Z | Sales | Net amount |
| 3 | Less exempted sales | EX | Sales | Net amount |
| 4 | Taxable sales amount |  | Sales | Box 1 - Box 2 - Box 3 |
| 5 | This month's output tax | S | Sales | Tax amount |
| Input tax |
| 6 | Purchase amount that is entitled to deduction of input tax from output tax in this month's tax computation | S | Purchases | Net amount |
| 7 | This month's input tax | S | Purchases | Tax amount |
| Value added tax |
| 8 | This month's tax payable |  |  | If Box 5 is greater than or equal to Box 7, then Box 8 = Box 5 - Box 7. Otherwise, Box 8 is blank. |
| 9 | This month's excess tax payable |  |  | If Box 5 is less than Box 7, then Box 9 = Box 7 - Box 5. Otherwise, Box 9 is blank. |
| 10 | Excess tax payment carried forward from last month |  |  | Editable field |
| Net tax |
| 11 | Net tax payable |  |  | If Box 8 is greater than or equal to Box 10, then Box 11 = Box 8 - Box 10. Otherwise, Box 11 is blank. |
| 12 | Net excess tax payable |  |  | If Box 8 is less than Box 10, then Box 12 = Box 10 - Box 8. Otherwise, Box 12 is blank. |
| 13 | Surcharge |  |  | Editable field |
| 14 | Penalty |  |  | Editable field |
| 15 | Total tax payable: tax, surcharge, and penalty |  |  | If Box 11 has a value, then Box 15 = Box 11 + Box 13 + Box 14. If Box 12 has a value, and the sum of Box 13 + Box 14 is greater than or equal to Box 12, then Box 15 = Box 13 + Box 14 - Box 12. Otherwise, Box 15 is blank. |
| 16 | Total excess tax payable after computation of surcharge and penalty |  |  | If Box 11 has a value, then Box 16 is blank. If Box 12 has a value, and Box 13 + Box 14 is less than Box 12, then Box 16 = Box 12 - Box 13 - Box 14. Otherwise, Box 16 is blank. |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Thailand Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2018677.html)
-   [Thailand VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2019313.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
