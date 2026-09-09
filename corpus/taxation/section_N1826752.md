---
id: "section_N1826752"
type: "section"
title: "What goes into each box - Austria VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Austria Tax Topics > Austria VAT Report > What goes into each box - Austria VAT report"
parent: "section_N1826422"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1826752.html"
anchors: []
sha256: "260bd14eb01df70329a15cd69fc3818c497ac29357bdd99fae1958a8f63bbea2"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Austria VAT report.

| Calculation of sales tax: | Taxable base Euros and Cents |
| --- | --- |
| **Total Supplies of Goods and Services** | \- | \- |
| \- | a) Total amount of all taxable sales | **000** | \- | Net amount of sales with O-AT, ES-AT, ER-AT, ER3-AT, EZ-AT, ESR-AT, S-AT, R-AT, R2-AT, R3-AT, S2-AT +052+007 |
| \- | b) plus own consumption | **001** | + | Editable field |
| \- | c) less sales for which the tax liability has been transferred to the receiver | **021** | \- | Net amount of sales with RC-AT |
| \- | \- | **Total** | \- | 000+001-021 |
| **Tax free sales WITH input tax deduction** | \- | \- |
| \- | a) Sales to non EU countries (Exports) | **011** | \- | Net amounts of sales with O-AT |
| \- | b) Subcontracting wages | **012** | \- | Editable field |
| \- | c) Sea traffic, aviation, cross-border passenger transport, etc | **015** | \- | Editable field |
| \- | d) Intra-Community supplies | **017** | \- | Net amount of sales with ES-AT, ER-AT, ER3-AT, EZ-AT, ESR-AT |
| \- | e) Supplies of new vehicles to customers without a VAT number | **018** | \- | Editable field |
| **Tax free sales WITHOUT input tax deduction** | \- | \- |
| \- | a) Land sales | **019** | \- | Editable field |
| \- | b) Small businesses | **016** | \- | Editable field |
| \- | c) Other tax free sales without input tax deduction | **020** | \- | Editable field |
| **Total of Taxable Supplies of Goods and Services (including prepayments)** | \- | (000+001-021) -011-012-015-017-018-019-016-020 |
| **Sales subject to** | **Tax Base** | **VAT** |
| \- | Sales at 20% standard rate | **022** | Net amount of sales with S-AT | \- | Tax amount of sales with S-AT + Tax amount of sales adjustment in 022b with S-AT |
| \- | Sales at 10% reduced rate | **029** | Net amount of sales with R-AT | + | Tax amount of sales with R-AT + Tax amount of sales adjustment in 029b with R-AT |
| \- | Sales at 13% reduced rate | **006** | Net amount of sales with R2-AT | + | Tax amount of sales with R2-AT + Tax amount of sales adjustment in 006b with R2-AT |
| \- | Sales at 19% (Jungholz and Mittelberg) | **037** | Net amount of sales with S2-AT | + | Tax amount of sales with S2-AT + Tax amount of sales adjustment in 037b with S2-AT |
| \- | Sales at 10% agricultural enterprises | **052** | Editable field | + | Tax amount of 052 |
| \- | Sales at 8% agricultural enterprises | **007** | Editable field | + | Tax amount of 007 |
| \- | Sales at 5% according to § 28 Abs. 52 Z 1 from July 1, 2020 until December 31, 2020 | **009** | Net amount of sales R3-AT | + | Tax amount of sales with R3-AT + Tax amount of sales adjustment in 009b with R3-AT |
| **Carry over** | \- | 022+029+006+037+052+007+009 |
| \- | Tax liability according to § 11 Abs. 12 and 14, § 16 Abs. 2 and according to 7 Abs. 4 | **056** | + | Editable field |
| \- | Tax liability according to § 19 Abs. 1 zweiter Satz, § 19 Abs. 1c, Abs. 1d and according to Art. 25 Abs. 5 Abs. 5 | **057** | + | Notional tax amount of purchases with RC-AT, IS, ESSP-AT |
| \- | Tax liability according to § 19 Abs. 1a (construction works) | **048** | + | Editable field |
| \- | Tax liability according to § 19 Abs. 1b (pledged property, land in compulsory auctions) | **044** | + | Editable field |
| \- | Tax liability (scrap waste) | **032** | + | Editable field |
| \- | \- | **Tax Base** | \- |
| **Intra-Community purchases** |
| \- | Total value of Intra-Community purchases | **070** | Net amount of purchases with ES-AT, ER-AT, ER3-AT, ESR-AT, EZ-AT |
| \- | of which tax free amounts according to Art. 6 Abs. 2 | **071** | Net amount of purchases with EZ-AT |
| **Total amount** of taxable intra-community purchases | 070-071 |
| **Thereof subject to sales tax with:** | \- | \- |
| \- | 20% standard tax rate | **072** | Net amounts of purchases with ES-AT | + | Notional amounts of purchases with ES-AT |
| \- | 10% reduced tax rate | **073** | Net amounts of purchases with ER-AT | + | Notional amounts of purchases with ER-AT |
| \- | 13% reduced rate | **008** | Net amount of purchases ESR-AT | + | Notional amount of purchases ESR-AT |
| \- | 19% for Jungholz and Mittelberg | **088** | Editable field | + | Notional amount of 088 |
| \- | 5% according to § 28 Abs. 52 Z 1 from July 1, 2020 until December 31, 2020 | **010** | Net amount of purchases ER3-AT | + | Notional amount of purchases ER3-AT |
| **Purchases not to be taxed:** | \- |
| \- | Purchases which have been taxed in a member country of the destination country | **076** | Editable field |
| \- | Purchases which count as being taxed inland | **077** | Editable field |
| \- | **Total** | \- | 022+029+006+037+052+007+ 056+057+048+044+032+072+073+008+088+010 |
| **Calculation of the deductable input tax** | \- | \- |
| \- | Total amount of input tax excluding amounts shown separately below | **060** | \- | Tax amount of purchases of S-AT, R-AT, R2-AT, S2-AT, K-AT, G-AT, R3-AT, Deduct, Non-Deduct, tax amount of purchase adjustment accrued in 060 with S-AT, R-AT, R2-AT, S2-AT, K-AT, G-AT, R3-AT |
| \- | Third Country Imports (outside the EU) | **061** | \- | Net amount of purchases with DUTY-P, I-AT, tax amount of purchase adjustment in 061 with I-AT |
| \- | Input tax concerning owing importation VAT recorded on tax account | **083** | \- | Net amounts of purchases with DUTY-U |
| \- | Input tax from intra-Community purchases | **065** | \- | Notional amount of purchases with ES-AT, ER-AT, ER3-AT, ESR-AT, EK-AT, EC-G |
| \- | Input tax for supplies subject to Reverse Charge | **066** | \- | Notional tax amount of purchases with RC-AT, IS, ESSP-AT |
| \- | Input tax - construction works | **082** | \- | Editable field |
| \- | Input tax - pledged property, land in compulsory auctions | **087** | \- | Editable field |
| \- | Input tax concerning tax liabilities according to § 19 Abs. 1d (scrap and waste) | **089** | \- | Editable field |
| \- | Input tax concerning intra-Community deliveries of new vehicles from vehicle deliverers according to Art. 2 | **064** | \- | Editable field |
| \- | Thereof according to § 12 Abs. 3iVm Abs. 4 and 5 | **062** | \- | Editable field |
| \- | Correction according to § 12 Abs. 10 and 11 | **063** | \- | Editable field |
| \- | Correction according to § 16 | **067** | \- | Editable field |
| **Total amount of deductable input tax** | \- | 060+061+083+065+066+082+ 087+089+064+062+063+067 |
| \- | Input tax for motor vehicles Note: For the 2014 VAT form, line 27 is no longer included. | **027** | \- | Tax amount of purchases with K-AT, Notional amount of purchases with EK-AT, Tax amount of purchase adjustments of 027 with K-AT |
| \- | Input for buildings and other assets Note: For the 2014 VAT form, line 28 is no longer included. | **028** | \- | Tax amount of purchases with G-AT, Notional amount of purchases with EG-AT, Tax amount of purchase adjustments of 028 with G-AT |
| **Other corrections:** | **090** | \- | Editable field |
| \- | Remaining VAT/advance payment | **095** | \- | (006+007+008+022+029+037+052+056+057+048+044+032+072+073+088) - (060+061+083+065+066+082+ 087+089+064+062+ 063+067) - 27 - 28 + 90 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Austria Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1823786.html)
-   [Setting Up Tax Filing for Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1826176.html)
-   [EU Sales List for Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1831754.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
