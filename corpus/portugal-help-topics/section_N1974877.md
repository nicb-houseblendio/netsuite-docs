---
id: "section_N1974877"
type: "section"
title: "What goes into each box - Portugal VAT report"
branch: "portugal-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Portugal Help Topics > Portugal Tax Topics In Accounts Without SuiteTax > Portugal VAT Report > What goes into each box - Portugal VAT report"
parent: "section_N1974556"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1974877.html"
anchors: []
sha256: "afb1fb4fa1d6ba1468dfeeef1c1ed3d6a6d11bfaf48370b8272d4ca293266092"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Portugal VAT report.

| Value Added Tax |
| --- |
| **Calculation of the VAT for the period to which the return relates** |
|  | **Taxable Basis** |  | **VAT in favor of the State** |
| **1.** | Supply of goods and services in which the tax payer assessed VAT |  |
|  | Reduced rate | **1** | Sales net amount of R-PT | **2** | Sales tax amount of R-PT |
|  | Intermediate rate | **5** | Sales net amount of R2-PT | **6** | Sales tax amount of R2-PT |
|  | Standard rate | **3** | Sales net amount of S-PT, FA-PT, G-PT + Purchase net amount of RC-PT | **4** | Sales tax amount of S-PT, FA-PT, G-PT + Purchase notional tax amount of RC-PT |
|  | Exempt transactions or transaction outside the scope of VAT |  |
|  | Intra-Community supply of goods and supply of service included in the recapitulative statement | **7** | Sales net amount of ES-PT, ER-PT, ESSS-PT, ESSP-PT |  |
|  | Zero rated transactions | **8** | Sales net amount of O-PT, OS-PT, Z-PT |  |
|  | Exempt operations without right to deduct VAT on the inputs | **9** | Sales net amount of E-PT |  |
| **2.** | Intra-Community acquisitions of goods | **10** | Box 10 = Box 12 | **11** | Box 11 = Box 13 |
|  | In which the tax payer reverse charged the VAT | **12** | Purchase net amount of ES-PT, ER-PT, EZ-PT, EUFA-PT, EUG-PT | **13** | Purchase notional tax amount ES-PT, ER-PT, EUFA-PT, EUG-PT |
|  | In which the scope of articles 15 of CIVA and RITI | **14** | Editable field |  |
|  | In which the scope of article 22 (3), (4) and (5) of CIVA | **15** | Editable field |  |
| **3.** | Supplies of services acquired from entities established in other EU member states in which the VAT was reversed charged | **16** | Purchase net amount of ESSP-PT, ESSS-PT | **17** | Purchase notional tax amount of ESSP-PT, ESSS-PT |
|  | **VAT in favor of the tax payer** |  |
| **4.** | Deductible VAT (Purchases) |  |
|  | Assets | **20** | Purchase tax Amount of FA-PT, Deduct\_FA-PT + Purchase notional tax amount of EUFA-PT, RC-PT + Nondeductible tax amount of NonDeduct\_FA-PT |  |
|  | Inventory |  |
|  | Reduced rate | **21** | Purchase tax amount of R-PT, Deduct\_R-PT + Nondeductible tax amount of NonDeduct\_R-PT |  |
|  | Intermediate rate | **23** | Purchase tax amount of R2-PT, Deduct\_R2-PT + Nondeductible tax amount of NonDeduct\_R2-PT |  |
|  | Standard rate | **22** | Purchase tax amount of S-PT, Deduct\_S-PT + Nondeductible tax amount of NonDeduct\_S-PT |  |
|  | Other goods and services | **24** | Purchase tax amount of G-PT, Deduct\_G-PT + Purchase notional amount of EUG-PT + Nondeductible tax amount of NonDeduct\_G-PT |  |
| **Total amount (20 to 24)** |  |  |
| **5.** | Adjustments | **40** | Sales/Purchase tax amount of A-PT + Sales/Purchase notional amount of EUA-PT | **41** | Sales/Purchase tax amount of AP-PT + Sales/Purchase notional amount of EUA-PT |
| **6.** | VAT carried forward from earlier periods | **61** | Editable field |  |
| **7.** | VAT from a location other than the headquarter's location | **65** | Editable field | **66** | Editable field |
| **8.** | VAT from a location other than the headquarters' location (used in case there are transactions in 3 different locations) | **67** | Editable field | **68** | Editable field |
| **Total amount (field 65 and 67)** |  |  |  |
| **9.** | Adjustments in favour of tax payer communicated by the PTA | **81** | Editable field |  |
| **Total tax base** | **90** | Total 1 + 5 + 3 + 7 + 8 + 9 + 10 + 16 |
| **Total amount of VAT in favour of the tax payer** | **91** | Total (20 to 24) + 40 + 61 + 65 + 67 + 81 |
| **Total amount of VAT in favour of the State** | **92** | Total 2 + 6 + 4 + 11 + 17 + 41 + 66 + 68 |
| **VAT due** (Box 92-91) | **93** |  |  |
| **VAT credit** (Box 91-92 dependent on credit or debit above) | **94** |  |  |
| **Request a VAT refund** | **95** | Editable field |  |
| **Carry forward** | **96** | Editable field |  |

| 06-A |
| --- |
| **DESENVOLVIMENTO DO QUADRO 06** |
| **A** | OPERATIONS LOCATED IN PORTUGAL assessed by the VAT DUE (Amounts of tax bases, including fields 1, 5 and 3) |
| Performed by entities resident in EU countries (doesn't include operations mentioned in field 16) | **97** | Editable field | Performed by entities resident in third territories | **98** | Editable field |
| **B** | Operations where VAT is subject to Reverse Charge Liabilities (Amounts of tax bases, including fields 1, 5 and 3) |
| Gold (Decree - Law 362/99) | **99** | Editable field | Acquisitions of properties with waiver of exemption (Decree-Law 21/2007) | **100** | Editable field |
| Scrap \[Subparagraph i) n. 1 of art. 2. º of CIVA\] | **101** | Editable field | Construction services n. 1 of art. 2. º the CIVA | **102** | Editable field |
| **C** | Operations specified in subparagraphs F) EG) No. 3 OF ARTICLE 3. º E a) and b) Paragraph 2 OF ARTICLE 4. º CIVA (Amounts of tax bases, including fields 1, 5 and 3) |
| Value of the transactions If carried out | **103** | Editable field |
| **D** | Operations specified in subparagraphs A), B) EC) OF ARTICLE 42. º CIVA (Amounts of tax bases, including fields 1, 5, 3 and 9) |
| Value of the transactions If carried out | **104** | Editable field |
| **SUM OF TABLE 06-A (97 + .... + 104)** | **105** | Box 97 + 98 + 99 + 100 + 101 + 102 + 103 + 104 |

### Additional Information

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

### Related Topics

-   [Portugal VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1974556.html)
-   [Portugal Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1973379.html)
-   [Portugal Standard Audit File for Tax Purposes (PT SAF-T)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1971159.html)
-   [EU Sales List for Portugal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1978248.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
