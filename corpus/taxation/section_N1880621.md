---
id: "section_N1880621"
type: "section"
title: "What goes into each box - Czechia VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Czechia Tax Topics > Czechia VAT Report > What goes into each box - Czechia VAT report"
parent: "section_N1880287"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1880621.html"
anchors: []
sha256: "821689d8b07469a3e3f83c1091e3775da4741139ad74d09260aa4dc6ef436dad"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Czechia VAT report.

| I. Taxable supplies | Tax base | Output tax |
| --- | --- | --- |
| Delivery of goods or provision of service with a domestic delivery place (For example: Sections 13, 14, 18) | Base | **1** | Net amount of sales S-CZ | Tax amount of sales S-CZ + Tax amount of sales adjustment of box 1b, S-CZ |
| Reduced | **2** | Net amount of Sales R-CZ, SR-CZ | Tax amount of sales R-CZ, SR-CZ + Tax amount of sales adjustment of box 2b, R-CZ, SR-CZ |
| Purchase of goods from another member state (Section 16; Section 17 (6) (e); Section 19 (3)) | Base | **3** | Net amount of Purchases ES-CZ | Notional tax amount of Purchases ES-CZ |
| Reduced | **4** | Net amount of Purchases ER-CZ | Notional tax amount of Purchases ER-CZ |
| Receiving services with place of supply according to section 9 (1) from an entity registered for tax in another member state | Base | **5** | Net amount of Purchases ESSP-CZ | Notional tax amount of Purchases ESSP-CZ |
| Reduced | **6** | Net amount of Purchases ESPR-CZ | Notional tax amount of Purchases ESPR-CZ |
| Import of goods (Section 23 (3-5)) | Base | **7** | Net amount of Purchases I-CZ, IZ2-CZ | Tax amount of purchases I-CZ + Notional tax amount of purchase IZ2 + Tax amount of purchase adjustment of box 7b, I, IZ2 |
| Reduced | **8** | Net amount of Purchases IR-CZ | Tax amount of Purchases IR-CZ + Tax amount of purchase adjustments of box 8b, IR-CZ |
| Purchase of new transport vehicle (Section 19 (4)) | **9** | Net amount of Purchases NV-CZ | Tax amount of Purchases NV-CZ + Tax amount of purchase adjustments of box 9b, NV-CZ |
| Regime of tax liability transfer (Section 92a) - goods supplier or service provider | Base | **10** | Net amount of Purchases RC-CZ | Notional tax amount of Purchases RC-CZ |
| Reduced | **11** | Net amount of Purchases RCR-CZ, RCSR-CZ | Tax amount of Purchases RCR-CZ, RCSR-CZ |
| Other taxable supplies where the tax is to be declared by the taxpayer upon receipt (Section 108) | Base | **12** | Net amount of Sales OT-CZ, Net amount of Purchases IS-CZ, RCOND-CZ | Tax amount of sales, OT-CZ, Notional tax amount of Purchases IS-CZ, RCOND-CZ |
| Reduced | **13** | Net amount of sales OTR-CZ, OTSR-CZ, Net amount of purchases ISR-CZ, ISSR-CZ, RCOND2-CZ, RCOND3-CZ | Tax amount of sales OTR-CZ, OTSR-CZ + Tax amount of sales adjustments box 13b, OTR-CZ, OTSR-CZ + Notional tax amount of purchases ISR-CZ, ISSR-CZ, RCOND2-CZ, RCOND3-CZ |

| II. Supplies exempt from tax and with a foreign delivery place and a tax abatement claim | Value |
| --- | --- |
| Delivery of goods to another member state (Section 64) | **20** | Net amount of sales ES-CZ, ER-CZ, EZ-CZ |
| Provision of services with a delivery place in other member state specified in section 102 clause 1 letter d | **21** | Net amount of sales ESSS-CZ |
| Export of goods (Section 66) | **22** | Net amount of sales O-CZ |
| Delivery of a new vehicle to an entity not registered for tax in another member state (Section 19 (4)) | **23** | Editable field |
| Shipment of goods to another member state (Section 18) | **24** | Editable field |
| Regime of tax liability transfer (section 92a) - goods supplier or service provider | **25** | Net amount of sales -CZ, RCR-CZ, RCSR-CZ |
| Other performed supplies with a tax abatement claim (For example: Sections 24a, 67, 68, 69, 70, 89, 90, 92) | **26** | Net amount of sales Z-CZ, E-CZ, OS-CZ, Net amount of purchases IG-CZ |

| III. Additional data |
| --- |
| Simplified procedure for delivery of goods in the form of a trilateral business (Section 17) by an intermediary | Purchase of goods | **30** | Editable field |
| Delivery of goods | **31** | Editable field |
| Exempted import of goods according to section 71g | **32** | Net amount of purchases IE-CZ |
| Tax correction for receivables from debtors involved in insolvency proceedings (section 44) | Creditor | **33** | Editable field |
| Debtor | **34** | Editable field |

| IV. Claim for tax abatement | Tax base | In full amount | Reduced claim |
| --- | --- | --- | --- |
| From received taxable supplies from taxpayers | Base | **40** | Net amount of purchases S-CZ, Deduct\_S-CZ | (Tax Amount of purchases S-CZ, Deduct\_S + Tax amount of purchase adjustments box 40b, S-CZ) - Tax amount of nondeductible NonDeduct\_S | Editable field |
| Reduced | **41** | Net amount of Purchases R-CZ, SR-CZ, Deduct\_R, Deduct\_SR | (Tax Amount of Purchases R-CZ, Deduct\_R, Deduct\_SR + Tax Amount of Purchase Adjustments box 41b, R-CZ, SR-CZ) - Tax Amount of Nondeductible NonDeduct\_R, NonDeduct\_SR | Editable field |
| Upon import of goods when the tax administrator is the customs duty office | **42** | Editable field | Editable field | Editable field |
| From taxable supplies recorded on lines 3 to 13 | Base | **43** | 3(Box 3a + box 5a + box 7a + box 9a + box 10a + box 12a) - Net amount of Purchases RCOND-CZ | (Box 3b + box 5b + box 7b + box 9b + box 10b + box 12b) - Notional amount of Purchases RCOND-CZ | Tax amount of purchases NV-CZ; Excludes RCOND2-CZ and RCOND3-CZ |
| Reduced | **44** | (Box 4a + box 6a + box 8a + box 11a + box 13a) - Net amount of Purchases RCOND2-CZ, RCOND3-CZ | (Box 4b + box 6b + box 8b + box 11b + box 13b) - Notional amount of Purchases RCOND2-CZ, RCOND3-CZ | Editable field Excludes RCOND2-CZ and RCOND3-CZ |
| Tax deduction correction according to section 75 (4) 77 and 79 | **45** | \- | Editable field | Editable field |
| Tax abatement total | **46** | \- | Box 40b + box 41b + box 42b + box 43b + box 44b + box 45b | Editable field |
| Value of purchased assets specified in Section 4 (3d and 3e) | **47** | Editable field | Editable field | Editable field |

| Reduction of tax abatement |
| --- |
| Supplies exempt from tax without a tax abatement claim | **50** | Editable field | \- |
| Value of supplies not included in the calculation of Section 76 (4) | **51** | **Tax abatement claim** | **No tax abatement claim** |
| \- | Editable field | \- | Editable field | \- |
| Reduced tax deduction proportion | **52** | **Coefficient (%)** | Editable field | **Abatement** | Editable field |
| Settlement of tax abatement (Section 76 (7) to (10)) | **53** | **Settlement coefficient (%)** | Editable field | **Change of tax abatement** | Editable field |

| VI. Calculation of tax liability |
| --- |
| Adjustment of tax abatement (Section 78 to 78c) + deduction adjustment according to section 78 and equalization according to section 79 of the VAT Act in force until the end of the year 2010 | **60** | Editable field |
| Tax return (Section 84) | **61** | Editable field |
| Output tax (1+2+3+4+5+6+7+8+9+10+11+12+13-61+ tax according to Section 108 (1k)) | **62** | (Box 1b + box 2b + box 3b + box 4b + box 5b + box 6b + box 7b + box 8b + box 9b + box 10b + box 11b + box 12b + box 13b) - box 61 |
| Tax abatement (46 in full amount + 52 abatement + 53 change of abatement + 60) | **63** | 46 in full amount + 52 abatement + 53 change of abatement + 60 |
| Real tax liability (62-63) | **64** | 62-63 |
| Excess abatement (63-62) | **65** | 63-62 |
| Change of tax liability upon submission of additional declaration (62-63) | **66** | 62-63 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Czechia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1874517.html)
-   [Czechia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1880287.html)
-   [Czechia VAT Control Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4491314862.html)
-   [What goes into each box - Czechia VAT Control Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4491318921.html)
-   [EU Sales List for Czechia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1884938.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
