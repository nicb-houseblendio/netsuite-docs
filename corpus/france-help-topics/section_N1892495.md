---
id: "section_N1892495"
type: "section"
title: "What goes into each box - France VAT report"
branch: "france-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > France Help Topics > France Tax Topics For Accounts Without SuiteTax > France VAT Report > What goes into each box - France VAT report"
parent: "section_N1892249"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1892495.html"
anchors: []
sha256: "50305592e2eb49bf84337a8a8067acae7c25c3e5ebf97b2465cb7dfc68f8f29f"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the France TVA Form (2012).

| A | TRANSACTION AMOUNTS |
| --- | --- |
|  | TAXED OPERATIONS (H.T.) |  | NON-TAXED OPERATIONS |
| --- | --- | --- | --- |
| **A1** | Sales, services | **0979** | Net amounts of sales with tax codes S-FR, R-FR, SR-FR, R1-FR, R2-FR, RC-FR, GAZ-FR | **E1** | Exports outside of the EU | **0032** | Net amount of sales with tax codes O-FR, OS-FR |
| **A2** | Other Taxable Revenue | **0981** | Net amount of sales with tax code Z-FR Net amount of purchases IS1-FR, IS2-FR, IS3-FR, IS4-FR, FA-FR, GAZ-FR | **E2** | Other non-taxable transactions | **0033** | Net amount of sales with tax code E-FR |
| **A3** | Purchases of intra-community services | **0044** | Net amount of purchases with tax code ESSP-FR, ESSS-FR | **E3** | Sales of goods or services provided by non-French residents (Art 283-1 of Customs code) | **0047** | Editable field |
| **A4** | Imports (other than petroleum products) | **0056** | Editable Field | **E4** | Imports (other than petroleum products) | **0052** | Editable field |
| **E5** | Withdrawals from the suspensive tax regime (other than petroleum products) | **0053** | Editable field |
| **E6** | Imports placed under a suspensive tax regime (other than petroleum products) | **0054** | Editable field |
| **A5** | Withdrawals from the suspensive tax regime (other than petroleum products) | **0051** | Editable Field | **F1** | Intra-Community acquisitions | **0055** | Net amount of purchases with tax codes ES-FR, ER-FR, EZ-FR, ESSP-FR, ESR-FR |
| **F2** | Intra-Community sales | **0034** | Net amount of sales with tax codes ES-FR, ER-FR, EZ-FR, ESSS-FR, ESR-FR |
| **F3** | Non-taxable sales of natural gas or electricity in France | **0029** | Editable Field |
| **B1** | Releases for consumption of petroleum products | **0048** | Editable Field | **F4** | Releases for consumption of petroleum products | **0049** | Editable Field |
| **B2** | Remote sales taxable in another EC country, non-VAT registered customers - B2C sales | **0031** | Net amounts of purchases with tax codes ES-FR, ER-FR, EZ-FR, ESR-FR | **F5** | Imports of petroleum products placed under a suspensive tax regime | **0050** | Editable Field |
| **B3** | Taxable deliveries of natural gas or electricity in France | **0030** | Net amounts of sales with tax code GAZ-FR | **F6** | Purchasing duty free | **0037** | Net amount of purchases with tax code DTY-FR |
| **B4** | Purchases of goods and services from a business not based in France | **0040** | Net amounts of purchases with tax codes I-FR, IS-FR | **F7** | EC sales, VAT registered customers - B2B sales | **0043** | Net amount of sales with tax code NF-FR |
| **B5** | Adjustments/Payment of past due taxes | **0036** | Editable Field | **F8** | Adjustments/Payment of past due taxes | **0039** | Editable Field |

| B | VAT PAYABLE |
| --- | --- |
|  | Net VAT excluding Balance due | Net Amount | Tax Due |
| --- | --- | --- | --- |
|  | **Transactions carried out in France** |  |  |
| **08** | Normal rate 20% | **0207** | Net amount of sales S-FR, GAZ-FR + Net amount of purchases ESSP-FR, ESSS-FR, RC-FR, ES-FR, IS-FR, IS1-FR | Tax amount of sales S-FR, GAZ-FR + Tax amount of purchases ESSP-FR, ESSS-FR, RC-FR, ES-FR, IS-FR, IS1-FR |
| **09** | Reduced rate 5.5% | **0105** | Net amount of sales R-FR + Net amount of purchases ER-FR, IS3-FR | Tax amount of sales R-FR + Tax amount of purchases ER-FR, IS3-FR |
| **9B** | Reduced rate 10% | **0151** | Net amount of sales SR-FR + Net amount of purchases ESR-FR, IS2-FR | Tax amount of sales SR-FR + Tax amount of purchases ESR-FR, IS2-FR |
|  | **Sales made on outer-continental France** |  |  |
| **10** | Normal rate 8.5% | **0201** | Net amount of sales R1-FR | Tax amount of sales R1-FR |
| **11** | Reduced rate 2.1% | **0100** | Net amount of sales R2-FR + Net amount of purchases IS4-FR | Tax amount of sales R2-FR + Tax amount of purchases IS4-FR |
|  | **Taxable operations at other rates** |  |  |
| **13** | Old rates | **0900** | Editable field | Editable field |
| **14** | Revenue taxable on a pre-determined rate | **0950** | Editable field | Editable field |
|  | **Petroleum products** |  |  |
| **P1** | Normal rate 20% | **0208** | Editable field | Editable field |
| **P2** | Reduced Rate 13% | **0152** | Editable field | Editable field |
|  | **Imports** |  |  |
| **I1** | Normal rate 20% | **0210** | Net amount of purchases IPA1-FR | Notional tax amount of purchases IPA1-FR |
| **I2** | Reduced Rate 10% | **0211** | Net amount of purchases IPA2-FR | Notional tax amount of purchases IPA2-FR |
| **I3** | Reduced Rate 8.5% | **0212** | Net amount of purchases IPA3-FR | Notional tax amount of purchases IPA3-FR |
| **I4** | Reduced Rate 5.5% | **0213** | Net amount of purchases IPA4-FR | Notional tax amount of purchases IPA4-FR |
| **I5** | Reduced Rate 2.1% | **0214** | Net amount of purchases IPA5-FR | Notional tax amount of purchases IPA5-FR |
| **I6** | Reduced Rate 1.05% | **0215** | Net amount of purchases IPA6-FR | Notional tax amount of purchases IPA6-FR |
| **15** | VAT previously deducted now due - reverse VAT | (including VAT on petroleum products) | **0600** | Editable Field |
| (including VAT on imported products excluding petroleum products) |
| **5B** | Are to be added, including advance leave (in Euro) | **0602** | Editable Field |
|  | Line 11 applies to DOM only; other transactions taxable at 2.1% are declared on annex form 3310 A-SD | **16** | Total of the VAT gross (lines 08 to 5B) | Lines 08+09+9B+10+11+13+14+P1+ P2+I1+I2+I3+I4+I5+I6+15+5B |
| **17** | VAT due on intra-Community acquisitions | **0035** | Notional tax amount of purchases ER-FR, ES-FR, ESR-FR, ESSP-FR |
| **18** | VAT due on sales to customers in Monaco | **0038** | Tax amount of sales MO-FR |
|  | **VAT DEDUCTIBLE** |  |  |
| **19** | Property constituting fixed assets | **0703** | (Tax amount of purchases with tax code FA-FR, Deduct\_FA + Tax amount of purchase adjustments box0703, FA-FR) Tax amount of nondeductible NonDeduct\_FA-FR |
| **20** | Other goods and services | **0702** | (Tax amount of purchases S-FR, R-FR, R1-FR, R2-FR, SR-FR, IS1-FR, IS2-FR, IS3-FR, IS4-FR, Deduct-FR + Notional tax amount of purchases RC-FR, IS-FR, ES-FR, ER-FR, ESSS-FR, ESSP-FR, ESR-FR, RCI-FR + Tax amount of purchase adjustments box0702, S-FR, R-FR, R1-FR, R2-FR, SR-FR, IS1-FR, IS2-FR, IS3-FR, IS4-FR ) - Tax amount of nondeductible NonDeduct-FR |
| **21** | Other VAT to be deducted (including regularization of:
-   VAT on petroleum products:
-   VAT on imported products excluding petroleum products:
-   VAT collected on other products or PS \[cf. notice\] or deductible:)

 | **0059** | Editable field |
| **22** | Balance forward of the credit showing on line 27 of the previous VAT return | **8001** | Editable field |
| **2C** | Amounts to be charged, including holiday provisions (in Euro) | **0603** | Editable field |
| **22A** | Indicate the unique tax coefficient applicable for the period if it's different from 100 | **23** | Total deductible VAT (lines 19 to 2C) | Lines 19 + 20 + 21 + 22 + 2C |
| **24** | Of which deductible VAT on imports excluding petroleum products | **0710** | Tax amount of purchases IS1-FR, IS2-FR, IS3-FR, IS4-FR + Notional tax amount of purchases IS-FR |
| **2E** | Of which deductible VAT on petroleum products | **0711** | Editable field |

|  | CREDIT |  | TAX PAYABLE |
| --- | --- | --- | --- |
| **25** | VAT Credit (line 23 - line 16) | **0705** | Line 23 - Line 16 | **28** | Net VAT amount due (line 16 to line 23) | Line 16 - Line 23 |
| **26** | Refund requested on document N° 3519 | **8002** | Editable field | **29** | Total tax calculated for annex no 3310 A-SD | **9979** | Editable Field |
| **AA** | VAT credit transferred to the head company Group Reporting Summary 3310-CA3G (line 25 - line 26) | **8005** | Editable field | **AB** | Total liabilities paid by the head company of the Group Reporting Summary 3310-CA3G (lines 28 + 29) | **9991** | Line 28 + Line 29 |
| **27** | Credit to be carried forward (line 25 - line 26 - line AA) (amount to be carried forward to line 22 of the following VAT return) | **8003** | Line 25 - Line 26 - Line AA | **32** | Total Amount Payable (lines 28 +29 - AB) | Line 28 + Line 29 - Line AB |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [France Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1890308.html)
-   [France VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1892249.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
