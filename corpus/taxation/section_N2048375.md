---
id: "section_N2048375"
type: "section"
title: "What goes into each box - Viet Nam VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Viet Nam Tax Topics > Viet Nam VAT Report > What goes into each box - Viet Nam VAT report"
parent: "section_N2048042"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2048375.html"
anchors: []
sha256: "1eb9bf0b62a4d725ca7d0b7a12d76e4b404c09c7265d448702490e19ede48202"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page is not supported. If you'd like to create nondeductible tax codes that work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Viet Nam VAT report.

| No. | Item |  | Goods, services purchased (without VAT) | VAT |
| --- | --- | --- | --- | --- |
| A | No sales and purchases during the period (Mark "X") | 21 |  |  |  |  |
| B | Amount of deductible VAT carried forward from previous period |  |  |  | 22 | Editable field |
| C | Declaration of VAT payable to State Treasury |  |  |  |  |  |
| I | Goods, services purchased in the period |  |  |  |  |  |
| 1 | Total value and VAT of the goods, services purchased |  | 23 | Total purchases excluding VAT | 24 | VAT amount of all purchases |
| 2 | Total amount of VAT to be deducted in the period |  |  |  | 25 | Value of box 24 |
| II | Goods, services sold out in the period |  |  |  |  |  |
| 1 | Goods, services not subject to VAT |  | 26 | Sales amount with EX tax code |  |  |
| 2 | Goods, services being subject to VAT |  | 27 | Box 29 + 30 + 32 | 28 | Box 31 + 33 |
| a | Goods, services with VAT rate of 0% |  | 29 | Sales amount with Z tax code |  |  |
| b | Goods, services with VAT rate of 5% |  | 30 | Sales amount with R tax code | 31 | VAT amount of Sales with R tax code |
| c | Goods, services with VAT rate of 10% |  | 32 | Sales amount with S tax code | 33 | VAT amount of Sales with S tax code |
| 3 | Total revenue and VAT of the goods, services provided |  | 34 | Box 26 + 27 | 35 | Value of box 28 |
| III | VAT payable in the period |  |  |  | 36 | Box 35 - 25 |
| IV | Determination of VAT payable for the period: |  |  |  |  |  |
| 1 | Increase in VAT payable of previous periods |  |  |  | 37 | Editable field |
| 2 | Decrease in VAT payable of previous periods |  |  |  | 38 | Editable field |
| V | Total VAT payable of revenue from business of construction, installation, irregular sales outside the province |  |  |  | 39 | Editable field |
| III | Determination of VAT payable for the period: |  |  |  |  |  |
| 1 | VAT payable for manufacturing and trading activities in the period |  |  |  | 40a | Box 36 - 22 + 37 - 38 - 39 (if value is a positive number). If value is 0 or negative number, this box displays 0. |
| 2 | Input VAT of investment projects (in the same province, city under the Central Government) being offset against VAT payable of the manufacturing and trading activities in the same tax period |  |  |  | 40b | Editable field |
| 3 | VAT payable for the period |  |  |  | 40 | Box 40a - 40b |
| 4 | VAT not yet totally deducted for the period |  |  |  | 41 | Box 36 - 22 + 37 - 38 - 39. (Shows absolute value of result if value is a negative number). If value is 0 or positive number, this box displays 0. |
| 4.1 | Proposed VAT refund for the period |  |  |  | 42 | Editable field |
| 4.2 | VAT carried forward to the next period ( |  |  |  | 43 | Box 41 - 42 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Viet Nam Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2047326.html)
-   [Viet Nam VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2048042.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
