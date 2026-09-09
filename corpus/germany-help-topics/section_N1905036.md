---
id: "section_N1905036"
type: "section"
title: "What goes into each box - Germany Annual VAT Declaration"
branch: "germany-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Germany Help Topics > Germany Tax Topics For Accounts Without SuiteTax > Germany VAT Report > What goes into each box - Germany Annual VAT Declaration"
parent: "section_N1899458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1905036.html"
anchors: []
sha256: "134fff9c2c46b6cf345fbb5a09cf6a52c3ff70d74cdd181274648f6053f76167"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Annual VAT Declaration for Germany. For monthly/quarterly returns, see [What goes into each box - Germany Monthly/Quarterly VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899865.html).

| Line | Label | Box | Amount (Full EUR Amounts) |
| --- | --- | --- | --- |
| 31 | **B. Information on taxation of small businesses (§ 19 para. 1 UStG)** Lines 33 and 34 should only be filled out if income for 2021 (plus taxes) did not exceed EUR 22,000 and the application of § 19 para. 1 UStG was not waived. |
| 33 | Sales in calendar year 2021 | (Calculation under § 19 para. 1 and 3 UStG) | 238 | Editable field |
| 34 | Sales in calendar year 2022 | 239 | Editable field |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) | Box | Tax |
| --- | --- | --- | --- | --- | --- |
| 36 | **C. Taxable supplies, other services and goods and services granted free of charge** |
| 37 | **Sales at standard tax rate** |
| 38 | Supplies and other services at 19% including negative amount resulting from credit notes issued on invoices using wrong tax rates due to tax changes in context of COVID-19 government measures | 177 | Net amount of sales S-DE, EST-DE | \- | Tax amount of Sales S-DE, EST-DE |
|  | Goods and services granted free of charge |  |
| 39 | a) Deliveries under § 3 para. 1b UStG at 19% | 178 | Editable field | \- | Editable field |
| 40 | b) Other services under § 3 para. 9a UStG at 19% | 179 | Editable field | \- | Editable field |
|  | **Sales at reduced tax rate** |
| 41 | Supplies and other services at 7% including negative amount resulting from credit notes issued on invoices using wrong tax rates due to tax changes in context of COVID-19 government measures | 275 | Net amount of sales R-DE, ERT-DE | \- | Tax amount of sales R-DE, ERT-DE |
|  | Goods and services granted free of charge at 7% |  |
| 42 | a) Supplies under § 3 para. 1b UStG at 7% | 195 | Editable field | \- | Editable field |
| 43 | b) Other services under § 3 para. 9a UStG at 7% | 196 | Editable field | \- | Editable field |
| 45 | **Sales at other tax rates** | 155 | Net amount of sales S2-DE, R1-DE, SR-DE | 156 | Tax amount of sales S2-DE, R1-DE, SR-DE |
| 47 | **Sales from agriculture and forestry businesses under § 24 UStG** |
| 48 | a) Supplies to customer in another Member State in the Community territory **with** USt-IdNR | 777 | Editable field | \- | \- |
| 49 | b) Taxable supplies (including goods and services granted free of charge) of **sawmill products** that are not listed in Schedule 2 of the UStG | 255 | Editable field | 256 | Editable field |
| 50 51 | c) Taxable sales (including goods and services granted free of charge) of **drinks** that are not listed in Schedule 2 of the UStG, as well as **alcoholic beverages** (e.g. wine) at 9.5% | 345 | Editable field | \- | Editable field |
| 53 | d) Remaining taxable sales of agriculture and forestry businesses for which no tax must be paid | 361 | Editable field | \- | \- |
| 54 55 | **Change from the small business regulation (§19 UStG) to standard taxation or Average rate taxation (§ 24 UStG)** |
| 56 | Tax (post-tax) on advance payments received as a result of changing the form of taxation | \- | \- | 317 | Editable field |
| 58 | Back taxes on taxed advance payments, i.e. owing to tax rate amendment | \- | \- | 319 | Editable field |
| 60 | Total (carryover to line 92) | \- | \- | \- | Boxes 177b + 178b + 179b + 275b + 195b +196b +156 + 256 + 345b + 258 + 317 + 319 |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) |
| --- | --- | --- | --- |
| 61 | **D. Tax-free supplies, other services and goods and services granted free of charge** |
| 62 | **Tax-free sales with input tax deduction** |
| 63 | a) **Intra-Community supplies** (§ 4 no. 1 subpara. b UStG) to customer **with** USt-IdNr. | 741 | Net amount sales ES-DE, ER-DE, ER1-DE, ES1-DE |
| 64 | New vehicles to customers **without** USt-IdNr | 744 | Editable field |
| 65 | New vehicles outside a company (§ 2a UStG) | 749 | Editable field |
| 66 | **Further tax-free sales with input tax deduction** (e.g. under § 4 no. 1 subpara. a, 2 to 7 UStG) |  |
| 67 | **Export supplies** and contract finishing on export goods (§ 4 no. 1 subpara. a UStG) | \- | Net amount sales OS-DE, ZX-DE |
| 68 | Sales under § UStG | \- | Editable field but by default reports net amount sales of E-DE |
| 69 | Sales as defined by the Offshore Tax Agreement, the NATO Status of Forces Supplementary Agreement and the Supplementing Agreement to the NATO Headquarters Protocol | \- | Editable field |
| 70 | Travel services under § 25 para. 2 UStG | \- | Editable field |
| 71 | Total of lines 67 to 70 | 237 | Line 67 + Line 68 + Line 69 + Line 70 |
| 72 | **Tax-free sales without input tax deduction** |
| 73 | a) **not part of total sales** (§ 19 para. 3 UStG) under § 4 no. 12 UStG (Rental of real estate etc.) | 286 | Editable field |
| 74 | under § 4 no. UStG | 287 | Editable field |
| 75 | Total of lines 73 and 74 | 237 | Box 286 + Box 287 |
| 76 | b) **part of total sales** (§ 19 para. 3 UStG) |  |
| 77 | under § UStG | 240 | Editable field |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) | Box | Tax EUR Ct |
| --- | --- | --- | --- | --- | --- |
| 78 | **E. Intra-Community purchases** |
| 80 | **Tax-free intra-Community purchases** under §§ 4b and 25c UStG | 791 | Net amount purchase EZ-DE | \- | \- |
| 81 | **Taxable intra-Community purchases (§ 1a UStG)** |
| 82 | at tax rate 19% | 781 | Net amount purchase EST-DE, ES-DE | \- | Tax amount purchase EST-DE, ES-DE |
| 83 | at tax rate 7% | 793 | Net amount purchase ERT-DE, ER-DE | \- | Tax amount purchase ERT-DE, ER-DE |
| 84 | at other tax rate | 798 | Editable field but by default report Net amount of purchases ES1-DE, ER1-DE, ESR-DE | 799 | Editable field but by default report Notional amount of purchases ES1-DE, ER1-DE, ESR-DE |
| 85 | **New vehicles** (§ 1b Abs. 2 and 3 UStG) from suppliers **without** USt-IdNr. at standard tax rate | 794 | Editable field | 796 | Editable field |
| 86 | Total (carryover to line 153) | Total tax amount = Box 781b + Box 793b + Box 799 + Box 796 |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) | Box | Tax EUR Ct |
| --- | --- | --- | --- | --- | --- |
| 88 | **F. Taxpayer for removal of goods (§ 13a para. 1 no. 6 UStG)** |
| 89 | Supplies preceding removal of goods (§ 4 no. 4a sent. 1 subpara. a sent. 2 UStG) | 852 | Editable field | 853 | Editable field |
| 90 | Total (carryover to line 154) | (Equal to Box 853) |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) | Box | Tax EUR Ct |
| --- | --- | --- | --- | --- | --- |
| 91 | **G. Intra-Community triangular transactions (§ 25b UStG)** |
| 92 | Supplies of the **first customer** | 742 | Editable field | \- | \- |
| 93 | **Supplies for which the last customer owes VAT** |
| 94 | at tax rate 19% | 751 | Editable field | \- | Editable field |
| 95 | at tax rate 7% | 746 | Editable field | \- | Editable field |
| 96 | at other tax rate | 747 | Editable field | 748 | Editable field |
| 97 | Total (carryover to line 155) | Box 751b + Box 746b + Box 748 |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) | Box | Tax EUR Ct |
| --- | --- | --- | --- | --- | --- |
| 98 | **H. Recipient of goods and services as taxpayer (§ 13b UStG)** |
| 99 | Taxable other services of a company based in other Community zone (§ 13b para. 1 UStG) | 846 | Net amount of purchases ESSP-DE, ESSP1-DE | 847 | Notional amount of purchases ESSP-DE, ESSP1-DE |
| 100 | Revenue according to GrEStG (Land and buildings) (§ 13b para. 2 no. 2 and 3 UStG) | 873 | Editable field | 874 | Editable field |
| 101 | Other services (§ 13b Abs. 2 Nr. 1, 2, 4 to 12 UStG) | 877 | Net amount of purchases S1-DE, RC-DE, SS1-DE, RC1-DE, IS-DE, IS1-DE | 878 | Notional amount of purchases S1-DE, RC-DE, SS1-DE, RC1-DE, IS-DE, IS1-DE |
| 102 | Total (carryover to line 156) |  | Total tax amount = Box 847 + Box 874 + Box 878 |

| Line | Label | Box | Tax base without VAT (Full EUR amounts) |
| --- | --- | --- | --- |
| 103 | **I. Supplementary information on sales** |
| 104 | Sales treated as taxable owing to a tax-exemption waiver (§ 9 UStG) | \- | Editable field |
| 105 | Taxable sales as defined by § 13b para 5 UStG of a company based in Germany, for which the recipient of goods and services owes VAT | 209 | Editable field but by default reports net amount of sales S1-DE, RC-DE, SS1-DE, RC1-DE |
| 106 107 | **Telecommunications, radio** and **television services** as well as **other services provided electronically** to non-entrepreneurs resident in the rest of the community as well as **intra-Community distance sales** to the rest of the community under the condition of § 3a paragraph 5 sentences 3 and 4 UStG and § 3c paragraph 4 sentences 1 and 2 VAT Act |
| 108 | a) included in section B or C | 213 | Editable field |
| 109 | b) to be taxed in other EU member states | 214 | Editable field |
| 110 | Tax-exempt transfer of going concern purs. to § 1 para. 1a UStG | 211 | Editable field |
| 111 | Non-taxable other services under § 18b sent. 1 no. 2 UStG | 721 | Editable field but by default reports net amount of sales ESSS-DE, ESSS1-DE |
| 112 | Other non-taxable sales (place of performance not in Germany) | 205 | Editable field but by default reports net amount of sales OS-DE |
| 113 | Sales listed in lines 109, 111, and 112 that exclude input tax deduction under § 15 para. 2 and 3 UStG | 204 | Editable field |
| 114 | Transactions of cross-border passenger transport allocated to the national route sections in air traffic (§ 26 para. 3 UStG) | 212 | Editable field |
| 115 | Reduction of the basis of assessment according to § 17 paragraph 1 sentence 1 in conjunction with paragraph 2 no. 1 sentence 1 UStG (included in section B or C) | 650 | Editable field |

| Line | Label | Box | Tax EUR Ct |
| --- | --- | --- | --- |
| 121 | **J. Deductible input tax amounts (without adjustment under § 15a UStG)** |
| 122 | Input tax amounts from invoices from other companies (§ 15 para. 1 sent. 1 no. 1 UStG) | 320 | Tax amount of purchases S-DE, R-DE, S2-DE, R1-DE + Full Tax Amount: Deduct\_S, Deduct\_R, Deduct\_S2, Deduct\_R1
-   For Bill/Bill Credit/Cheque: FULL Tax Amount = Deduct's Transaction Line Tax Amount (STC generated)

-   For Expense Report: FULL Tax Amount = Deduct Tax Amount + ND Tax Amount (ITR generated)

 |
| 123 | Input tax amounts from Intra-Community purchases of goods (§ 15 para. 1 sent 1 no. 3 UStG) | 761 | Tax amount of purchase EST-DE, ERT-DE, ES-DE, ER-DE, ES1-DE, ER1-DE |
| 124 | VAT incurred on imports (§ 15 para. 1 sent 1 no. 2 UStG) | 762 | Net amount of purchase IT-DE |
| 125 | Input tax deduction for taxes owed by customer as trade consignor under § 13a para. 1 no. 6 UStG (§ 15 para. 1 sent. 1 no. 5 UStG) | 466 | Editable field |
| 126 | Input tax amounts from services as defined by § 13b UStG (§ 15 para. 1 sent. 1 no. 4 UStG) | 467 | Editable field but by default reports notional amount of purchases ESSP-DE, IS-DE, RC-DE, S1-DE, ESSP1-DE, IS1-DE, RC1-DE, SS1-DE |
| 127 | Input tax amounts calculated according to the standard average rates (§ 23 UStG) | 333 | Editable field |
| 128 | Input tax amounts according to the average rate for certain corporations, groups of shareholders and hybrid entities (§ 23a UStG) | 334 | Editable field |
| 129 | Input tax deducation for intra-Community deliveries of **new vehicles** outside a company (§ 2a UStG) as well as from small businesses as defined by § 19 para. 1 UStG (§ 15 para. 4a UStG) | 759 | Editable field |
| 130 | Input tax amounts from intra-Community triangular transactions (§ 25b para. 5 UStG) | 760 | Editable field |
| 131 | Total (carryover to line 158) | Box 320 + Box 761 + Box 762 + Box 466 + Box 467 + Box 333 + Box 334 + Box 759 + Box 760 |

| Line | Label | Box | Box Description |
| --- | --- | --- | --- |
| 132 | **Additional Information** Reduction of the deductible input tax amounts according to § 17 paragraph 1 sentence 2 in conjunction with paragraph 2 no. 1 sentence 1 UStG (included in lines 122, 127 to 129) | 637 | Editable field |
| 133 | **K. Adjustment of input tax deduction (§ 15a UStG)** |
| 134 | Were **real estate**, **parts of real estate**, **buildings** or **parts of buildings**, for which input tax has been deducted, first actually used in calendar year 2022? If yes, please enter „1' | 370 | Editable field Allowed value is 1 |
| 135 | (Please show separately on a separate sheet of paper for each piece of real estate or building: location, date of first actual use, kind and extent of use in first year, total input tax accrued, in the previous years - investment phase - input tax already deducted) |
| 136 | Have relevant circumstances for the original input tax deduction changed in 2022 for: |
| 137 | 1\. **Real estate, parts of real estate, buildings** or **parts of buildings** that were first actually used within the last 10 years and **not just once** to carry out transactions? If yes, please enter „1' | 371 | Editable field Allowed value is 1 |
| 138 | 2\. **Other assets and other services** that were first actually used within the last 5 years and **not just once** to carry out transactions? If yes, please enter „1' | 372 | Editable field Allowed value is 1 |
| 139 | 3\. **Assets and other services** that were used to carry out transactions **just once**? If yes, please enter „1' | 369 | Editable field Allowed value is 1 |
| 140 | The circumstances that were originally relevant for the assessment of the input tax deduction have changed since then owing to |
| 141 | Sale | Supply as defined by § 3 para. 1b UStG | Change in taxation from § 15a para. 7 UStG | \- | Click the box to mark which applies. |
| 142 | Change in utilization, namely | Click box if applicable. |
| 143 | Transition from taxable to tax-free rental or vice versa or change utilization code for mixed-use real estate (in particular for a change in tenant) | Click box if applicable. |
| 144 | Tax-free rental of previously owner-used commercial rooms or vice versa; transition from rental for NATO or similar purposes at tax-free rental under § 4 no. 12 UStG | Click box if applicable. |
| 145 | \- | \- | Click box if applicable. Enter details in input field. |

| Line | Label | Box | Subsequently deductible EUR CT | Box | To be paid back EUR CT |
| --- | --- | --- | --- | --- | --- |
| 146 | **Input tax adjustment amounts** |
| 147 | see 1. (real estate etc., § 15a para. 1 sent. 2 UStG) | \- | Editable field | \- | Editable field |
| 148 | see 2. (other assets etc., § 15a para. 1 sent. 1 UStG) | \- | Editable field | \- | Editable field |
| 149 | see 3. (other assets etc., § 15a para. 2 UStG) | \- | Editable field | \- | Editable field |
| 150 | Total | 357 | Box 147a + 148a + 149a | 359 | Box 147b + 148b + 149b |

| Line | Label | Box | Tax EUR ct |
| --- | --- | --- | --- |
| 151 | **L. Computation of VAT to be paid** |
| 152 | **VAT on taxable supplies, other services and goods and services granted free of charge** | \- | Total tax amount value from Line 60 |
| 153 | **VAT on intra-Community purchases** | \- | Total tax amount value from Line 86 |
| 154 | VAT owed by customer as trade consignor or warehouse keeper (§ 13a para. 1 no. 6 UStG) | \- | Equal to Box 854 from Line 90 |
| 155 | VAT owed by last customer in the Intra-Community triangular transaction (§ 25b para. 2 UStG) | \- | Total tax amount value from Line 97 |
| 156 | VAT owed by service recipient § 13b UStG | \- | From Line 102 |
| 157 | Subtotal | Line 152 + Line 153 + Line 154 + Line 155 + Line 156 |
| 158 | **Deductible input tax amounts** | \- | Total amount from Line 131 |
| 159 | Input tax amounts subsequently deductible under § 15a UStG | \- | Equal to Box 357 from Line 150 |
| 160 | Remaining amount | Line 157 - Line 158 - Line 159 |
| 161 | Input tax amounts to be paid back under § 15a UStG | \- | Equal to Box 369 from Line 150 |
| 162 | Tax amounts incorrectly or unjustifiably shown in invoices (§ 14c UStG) as well as tax amounts owed under § 6a para. 4 sent. 2 UStG | 318 | Editable field |
| 163 | Tax amounts owed under § 17 para. 1 sent. 7 UStG | 331 | Editable field |
| 164 | Tax amounts, input tax amounts and deduction amounts accrued from earlier taxation periods (only for small businesses that apply § 19 para. 1 UStG anwenden) | 391 | Editable field |
| 165 | **VAT Surplus** - please enter amount with a minus sign - | Line 160 + Line 161 + Line 162 + Line 163 + Line 164 |
| 166 | Creditable amounts (from line 22 of schedule UN) | Editable field |
| 167 | **Remaining VAT** Remaining Surplus - please enter amount with a minus sign - | 816 | Line 165 - 166 |
| 168 | Estimated advance payment for 2022 (including special advance payment) | \- | Editable field |
| 169 | **Still to be paid to tax office** - Final payment **Tax refund claim** - please enter amount with a minus sign - | 820 | Box 816 - Line 168 |

### Additional Information

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

### Related Topics

-   [What goes into each box - Germany Monthly/Quarterly VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899865.html)
-   [Germany Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1897828.html)
-   [Germany VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899458.html)
-   [Setting Up Tax Filing for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1917361.html)
-   [Submission of VAT Returns in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1917621.html)
-   [Recapitulative Statement (EU Sales List) for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1918495.html)
-   [Intrastat Report for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4149981058.html)
-   [Germany GoBD Data Export](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3838969498.html)
-   [Germany Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554981475.html)
-   [Germany Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726737.html)
-   [Setting Up Germany-Specific Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726820.html)
-   [Germany-specific SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158529777788.html)
-   [Germany Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554985535.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
