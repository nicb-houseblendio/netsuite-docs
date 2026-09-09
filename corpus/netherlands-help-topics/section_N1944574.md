---
id: "section_N1944574"
type: "section"
title: "What goes into each box - Netherlands VAT report"
branch: "netherlands-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Netherlands Help Topics > Netherlands Tax Topics In Accounts Without SuiteTax > Netherlands VAT Report > What goes into each box - Netherlands VAT report"
parent: "section_N1944310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1944574.html"
anchors: []
sha256: "f310d488715b1975d49c0b5802d0c8c28f666f37afef9d276e2b01ba2634d9b7"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Netherlands VAT Return.

| Box | Tax Codes | Transactions | Net Amount | Tax Amount |
| --- | --- | --- | --- | --- |
| 1 | Supplies of goods and services in the Netherlands |
|  | 1a VAT at standard rate | S | Sales | Net amount | Tax amount |
|  | 1b VAT at reduced rate | R | Sales | Net amount | Tax amount |
|  | 1c VAT at other rates | SP | Sales | Net amount | Tax amount |
|  | 1d Private use (car, etc.) |  |  | Editable field | Editable field |
|  | 1e Supplies/services taxed at 0% (tax not levied on you) | RC, Z | Sales | Net amount |  |
| 2 | Reverse Charge - VAT transferred to you |
|  | 2a Sales - supplies/services where the VAT has been reverse charged to you | RC | Purchases | Net amount | Notional amount |
| 3 | Sales and deliveries outside the Netherlands |
|  | 3a Goods exported by you from the Netherlands to countries oustide the EU | O | Sales | Net amount |  |
|  | 3b Goods delivered by you from the Netherlands to countries within the EU (i.e., EC Sales List) | ES, ER, EZ, ESSS | Sales | Net amount |  |
|  | 3c Installation/distance sales from the Netherlands to countries within the EU |  | Sales | Editable field | Editable field |
| 4 | Purchases from other countries |  |  |  |  |
|  | 4a Purchases from countries outside the EU (import) | I, IS | Purchases | Net amount | Tax amount + Notional amount |
|  | 4b Intra-community acquisitions from other EU countries | ES, ER, EZ, ESSP | Purchases | Net amount | Notional amount |
| 5 | Sales Tax Calculations |  |  |  |  |
|  | 5a Total VAT to be paid = Box 1 + Box 2 + Box 3 + Box 4 |  |  |  | Tax amount sum of boxes 1a to 4b |
|  | 5b Input tax on purchases and costs in the Netherlands | All purchase tax codes | Purchases |  | Tax amount + Notional amount + Net amount of IV-NL |
|  | 5c Subtotal (Box 5a minus Box 5b) |  |  |  | Tax amount 5a - 5b |
|  | 5d Reduction under the small business ruling |  |  |  | Editable field |
|  | 5g Total VAT to be paid or reclaimed | Total |  |  | Tax amount 5c - 5d |

### Additional Information

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

### Related Topics

-   [Netherlands VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1944310.html)
-   [Netherlands Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1942969.html)
-   [EU Sales List for Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1947306.html)
-   [Intrastat Report for Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503450407.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [EU One Stop Shop Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4174874694.html)
-   [OSS Tax Code Provisioning for Regular NetSuite Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4204428442.html)
-   [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html)
-   [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html)
-   [Netherlands Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636146.html)
-   [Netherlands Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549424762.html)
-   [Setting Up Netherlands-Specific Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549425210.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
