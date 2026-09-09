---
id: "section_N1850889"
type: "section"
title: "What goes into each box - Bulgaria VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Bulgaria Tax Topics > Bulgaria VAT Report > What goes into each box - Bulgaria VAT report"
parent: "section_N1850643"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1850889.html"
anchors: []
sha256: "a50e2141f670b22f2ae82b89ef32d483893c679b6fc388bad9ade2cf23fa0b53"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Bulgaria VAT report.

| Section A: Data about the VAT charged |
| --- |
| **Total amount of the taxable bases subject to VAT** | Cell 11 + 12 + 13 + 14 + 15 + 16 | 01 | Total VAT charged | Cell 21 + 22+ 23 + 24 | 20 |
| **Taxable base subject to VAT rate:** | \- | \- | \- | \- | \- |
| \- taxable base of the taxable supplies, including supplies qualifying for distance sales with a place of supply in Bulgaria | Net amount of sales S-BG | 11 | VAT charged | Tax amount of sales S-BG | 21 |
| \- taxable base of the intra-community acquisitions and taxable base of supplies received under Art. 82, para 2-5 of the VAT Act | Net amount of purchases RC-BG, ES-BG, ESSP-BG | 12 | VAT charged for intra-community acquisitions and for supplies received under Art. 82, para 2-5 of the VAT Act | Notional VAT of purchases ES-BG, RC-BG, ESSP-BG | 22 |
| \- | \- | \- | VAT charged () in other cases stipulated in the VAT Act | Tax amount sales protocol | 23 |
| Taxable base of the supplies subject to VAT rate | Net amount of sales R-BG | 13 | VAT charged () | Tax amount of sales R-BG | 24 |
| **Taxable base subject to 0% VAT rate:** | \- | \- | \- | \- | \- |
| \- taxable base of supplies under Chapter 3 of the VAT Act | Net amount of sales RC-BG, Z-BG, O-BG, OS-BG, EZ-BG | 14 | \- | \- | \- |
| \- taxable base of the intra-community supplies of goods | Net amount of sales ES-BG, ER-BG | 15 | \- | \- | \- |
| \- taxable base of the supplies under Art. 140, 146 and 173, para 1 and 4 of the VAT Act | Net amount of sales T-BG | 16 | \- | \- | \- |
| Taxable base of the supplies of services as per Art. 21, para 2 of the VAT Act with a place of supply in another EU member state | Net amount of sales ESSS-BG | 17 | \- | \- | \- |
| Taxable base of the supplies under Art. 69, para 2 of the VAT Act, Including supplies qualifying as distance sales with a place of supply in another EU member state, as well as of supplies carried out as an intermediary in a triangular transaction | Net amount of sales TR-BG | 18 | \- | \- | \- |
| Taxable base of the exempt supplies and exempt intra-community acquisitions | Net amount of purchases EZ-BG, Net amount of sales E-BG | 19 | \- | \- | \- |

| Section B: Data about exercised right to VAT Credit |
| --- |
| Taxable base and VAT of the supplies received, Intra-community acquisitions, supplies received under Art. 82, para 2-5 of the VAT Act and import not entitled to VAT credit or without VAT | Net amount of purchases E-BG, Z-BG, EZ-BG, I-BG, IS-BG | 30 | \- | \- | \- |
| Taxable base of the supplies received, Intra-community acquisitions, supplies received under Art. 82, para 2-5 of the VAT Act, Import, as well as taxable base of the supplies received which are used for carrying out supplies under Art. 69, para 2 of the VAT Act: | \- | \- | \- | \- | \- |
| \- entitled to full VAT Credit | Net amount of purchases S-BG, R-BG, RC-BG, ES-BG, ESSP-BG | 31 | VAT entitled to full tax credit | Tax amount of purchases S-BG, R-BG, RC-BG, ES-BG + Notional amount of purchases RC-BG, ES-BG, ESSP-BG + Tax amount of purchase adjustments of box 41 with S-BG, R-BG, RC-BG | 41 |
| \- entitled to partial VAT Credit | Net amount of PC-BG, PCR-BG, Deduct\_Partial | 32 | VAT entitled to partial tax credit | Tax amount of purchases PC-BG, PCR-BG, Deduct\_Partial, NonDeduct\_Partial + Tax amount of purchase adjustments of box 42 with PC-BG, PCR-BG | 42 |
| \- | \- | \- | Annual adjustment under Art. 73, para 8 (+/-) of the VAT Act | Editable field | 43 |
| Coefficient determined under Art. 73, para 5 of the VAT Act | Editable field | 33 | **Total VAT Credit** | Cell 41 + (Cell 42 × Cell 33) + Cell 43 | 40 |

| Section C: Net result for the period |
| --- |
| VAT payable | (Cell 20 - Cell 40) ≥ 0 | 50 | VAT reclaimable | (Cell 20 - Cell 40) < 0 | 60 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Bulgaria Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1846495.html)
-   [Bulgaria VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1850643.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
