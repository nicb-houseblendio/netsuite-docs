---
id: "section_N2006403"
type: "section"
title: "What goes into each box - Sweden VAT report"
branch: "sweden-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Sweden Help Topics > Sweden Tax Topics For Accounts Without SuiteTax > Sweden VAT Report > What goes into each box - Sweden VAT report"
parent: "section_N2006138"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2006403.html"
anchors: []
sha256: "2a1dd1b9bb664d4aded592d9303e1e1c1501bcaa58fab7fe5fb4c864ca403153"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the VAT declaration for Sweden.

| Box | Tax Codes | Transactions | Net Amount | Tax Amount |
| --- | --- | --- | --- | --- |
| **A. VATable sales or withdrawals excluding VAT** |
| 05 | VATable sales which are not included elsewhere | S, R, SR | Sales | Net amount |  |
| 06 | VATable withdrawals | Editable field |  | Editable field |  |
| 07 | Tax base for margin scheme | Editable field |  | Editable field |  |
| 08 | Rental income from voluntary tax liability | Editable field |  | Editable field |  |
| **B. Output VAT on sales or withdrawals in boxes 05-08** |
| 10 | Output VAT | S (standard) | Sales |  | Tax amount |
| 11 | Output VAT | R (reduced) | Sales |  | Tax amount |
| 12 | Output VAT | SR (special reduced) | Sales |  | Tax amount |
| **C. VATable purchases when purchaser is tax liable** |
| 20 | Purchase of goods from other EU countries | ES, ER, ESR | Purchases | Net amount |  |
| 21 | Purchase of services from another EU country according to the main rule | ESSP | Purchases | Net amount |  |
| 22 | Purchase of services from countries outside EU | IS, ISR, ISSR | Purchases | Net amount |  |
| 23 | Purchase of goods in Sweden that the buyer is liable for | RCG | Purchases | Net amount |  |
| 24 | Other purchases of services in Sweden that the buyer is liable for | RCS | Purchases | Net amount |  |
| **D. Output VAT on purchases in boxes 20-24** |
| 30 | Output VAT | ES, IS, ESSP, RCG, RCS (standard) | Purchases |  | Tax amount + Notional amount |
| 31 | Output VAT | ER, ISR | Purchases |  | Notional amount |
| 32 | Output VAT | ESR, ISSR | Purchases |  | Notional amount |
| **H. Import** |
| 50 | Taxable amount import | IV, IVR, IVSR | Purchases | Net amount |  |
| **I. Output VAT on imports in box 50** |
| 60 | Output VAT | IV (standard) | Purchases |  | Notional tax amount |
| 61 | Output VAT | IVR (reduced) | Purchases |  | Notional tax amount |
| 62 | Output VAT | IVSR (special reduced) | Purchases |  | Notional tax amount |
| **E. Sales etc which are exempt from VAT** |
| 35 | Sale of goods to other EU countries | ES, ER, ESR, EZ | Sales | Net amount |  |
| 36 | Sale of goods outside EU | O | Sales | Net amount |  |
| 37 | Middleman's purchase of goods in triangulation | Editable field |  | Editable field |  |
| 38 | Middleman's sale of goods in triangulation | Editable field |  | Editable field |  |
| 39 | Sale of services to entrepreneurs in another EU country according to the main rule | ESSS | Sales | Net amount |  |
| 40 | Other sale of services supplied abroad | OS | Sales | Net amount |  |
| 41 | Sale where purchaser is taxable in Sweden | RCG, RCS | Sales | Net amount |  |
| 42 | Other sales etc. | E | Sales | Net amount |  |
| **F. Input VAT** |
| 48 | Input VAT to be deducted | All purchase tax codes | Purchases |  | Purchases TAX Amount + Purchase Notional Amount + Import Notional Amount |
| **G. VAT to pay or have repaid** |
| 49 | VAT to pay or have repaid |  |  |  | Total |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [Sweden VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2006138.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Sweden Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2004717.html)
-   [EU Sales List for Sweden](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2009636.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
