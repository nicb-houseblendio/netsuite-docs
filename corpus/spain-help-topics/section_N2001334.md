---
id: "section_N2001334"
type: "section"
title: "What goes into each box - Spain VAT report"
branch: "spain-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Spain Help Topics > Spain Tax Topics For Accounts Without SuiteTax > Spain VAT Report > What goes into each box - Spain VAT report"
parent: "section_N2001072"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2001334.html"
anchors: ["bridgehead_4059957541", "bridgehead_4059980121", "bridgehead_4060051577", "bridgehead_4060115657", "bridgehead_4060837080", "bridgehead_N2001351", "bridgehead_N2003197"]
sha256: "9e2db2945b126827ed3b26c35a43a40b5175dcca8ff611833d3010059c58775a"
---

The following table shows how NetSuite uses the tax codes to get the values for the **Modelo 303 Quarterly VAT Return**.

Note:

These tables are for the 2014 Spain Modelo 303 Quarterly VAT Return form. For pre-2014 Spain VAT report, see [Spain VAT Report for Periods Before 2014](#bridgehead_4060837080).

## General Regime {#bridgehead_4059957541}

| **Description** | **Base Amount** | **Tax Rate %** | **Tax Amount** |
| --- | --- | --- | --- |
| **VAT Due** |  |  |  |  |  |  |
| Sales normal regime | 01 | Net amount of sales S | 02 | standard tax rate | 03 | Sales tax amount S |
| Sales normal regime | 04 | Net amount of sales R | 05 | reduced tax rate | 06 | Sales tax amount R |
| Sales normal regime | 07 | Net amount of sales R2 | 08 | special reduced tax rate | 09 | Sales tax amount R2 |
| Intra-community acquisition of goods and services | 10 | Net amount of purchases ES, ER, EZ, EIG, ESSP |  |  | 11 | Notional purchase tax amount ES, ER, EZ, EIG, ESSP |
| Other transactions of reverse charge (except intra-community acquisition) | 12 | Net amount of purchases RC |  |  | 13 | Notional purchase tax amount RC |
| Modification of bases and VAT amounts | 14 | Editable field |  |  | 15 | Editable field |
| Sales retail business | 16 | Net amount of sales SC3 | 17 | standard tax rate | 18 | Sales tax amount SC3 |
| Sales retail business | 19 | Net amount of sales SC2 | 20 | reduced tax rate | 21 | Sales tax amount SC2 |
| Sales retail business | 22 | Net amount of sales SC1 | 23 | special reduced tax rate | 24 | Sales tax amount SC1 |
| Modification of bases and VAT amounts on sales retail business | 25 | Editable field |  |  | 26 | Editable field |
| Total due (03+06+09+11+13+15+18+21+24+26) |  |  |  |  | 27 | 03+06+09+11+13+15+18+21+24+26 |
| **Deductible VAT** |  |  |  |  |  |  |
| On common domestic transactions | 28 | Net amount of purchases S, R, R2, Z, RC |  |  | 29 | Purchase tax amount S, R, R2 Notional purchase tax amount RC |
| On domestic transactions with investment of goods | 30 | Net amount of purchases CG |  |  | 31 | Purchase tax amount CG |
| On imports of common goods | 32 | Net amount of purchases CA |  |  | 33 | Purchase tax amount CA |
| On imports of investment goods | 34 | Net amount of purchases IG |  |  | 35 | Purchase tax amount IG |
| Intra-community acquisition of common goods and services | 36 | Net amount of purchases ES, ER, EZ, ESSP |  |  | 37 | Notional purchase tax amount ES, ER, EZ, ESSP |
| Intra-community acquisitions of investment goods | 38 | Net amount of purchases EIG |  |  | 39 | Notional purchase tax amount EIG |
| Rectification of deductions | 40 | Editable field |  |  | 41 | Editable field |
| Compensations under special regime for agriculture, fishing industry |  |  |  |  | 42 | Editable field |
| Corrections of investment goods |  |  |  |  | 43 | Purchase tax amount RI |
| Corrections - application of definite pro rate percentage |  |  |  |  | 44 | Editable field |
| Total deductible (29+31+33+35+ 37+39+41+42+43+44) |  |  |  |  | 45 | 29+31+33+35+37+39+41+42+43+44 |
| Result general regime (27-45) |  |  |  |  | 46 | 27-45 |

## Simplified Regime {#bridgehead_4059980121}

| **Description** | **Tax Amount** |
| --- | --- |
| Result simplified regime | 58 | Editable field |

## Additional Information {#bridgehead_4060051577}

| **Description** | **Base Amount** | **Tax Amount** |
| --- | --- | --- |
| Intra-community supplies of goods and services |  |  | 59 | Net amount of sales ES, ER, EZ, ESSS |
| Export and related transactions |  |  | 60 | Net amount of sales O |
| Non-taxable transactions or reverse charge transactions which give right to deduct input VAT |  |  | 61 | Net amount of sales RC, OS |
| **These boxes have to be completed only by taxpayers who are taxed in special regime of cash accounting and those recipients of transactions affected by them:** |  |  |  |  |
| Value of supplies of goods or services to which the special regime of cash accounting applied was accrued in accordance to the general rule of accrual contained in Art. 75 LIVA | 62 | Editable field | 63 | Editable field |
| Value of supplies of goods or services which are applicable or affected by the special regime of cash accounting | 74 | Editable field | 75 | Editable field |

## VAT Result {#bridgehead_4060115657}

| **Description** | **Tax Rate %** | **Tax Amount** |
| --- | --- | --- |
| Total of results (46+58) |  |  | 64 | 46+58 |
| VAT payable to the Central Tax Authorities | 65 | % Editable field | 66 | Editable field |
| VAT carried forward from previous periods |  |  | 67 | Editable field |
| This box has to be completed only by taxpayers who are taxed in Spain jointly by the Central Spanish Tax Authorities and the Provincial Councils. Result of annual adjustment. |  |  | 68 | Editable field |
| VAT result (66-67+68) |  |  | 69 | 66-67+68 |
| Deductible VAT (only applicable to corrective returns): Result of the previous return(s) field for the same period and year |  |  | 70 | Editable field |
| VAT balance (69-70) |  |  | 71 | 69-70 |

## Spain VAT Report for Periods Before 2014 {#bridgehead_4060837080}

The Spain Modelo 303 Quarterly VAT Return form has changed for 2014. The following tables for pre-2014 Spain VAT report will be maintained as reference until the end of 2014 only.

## I.V.A. Accrued Taxes {#bridgehead_N2001351}

| Tax Base | % | IVA Amount |
| --- | --- | --- |
| 01 | Net amount of S sales and RC purchases, and net amount of ESSP | 02 | 18% | 03 | Tax amount of S sales, Notional amount of RC purchases, Notional amount of ESSP |
| 04 | Net amount of R sales | 05 | 18% | 06 | Tax amount of R sales |
| 07 | Net amount of R2 sales | 08 | 4% | 09 | Tax amount of R2 sales |

| Surcharge Equivalent | % | IVA Amount |
| --- | --- | --- |
| 10 | Net amount of SC1 sales | 11 | 0.5% | 12 | Tax amount of SC1 sales |
| 13 | Net amount of SC2 sales | 14 | 1% | 15 | Tax amount of SC2 sales |
| 16 | Net amount of SC3 sales | 17 | 4% | 18 | Tax amount of SC3 sales |

| Intra-Community Acquisitions | IVA Amount |
| --- | --- |
| 19 | Net amount of ES, ER, EZ, and EIG | 20 | Tax amount of ES, ER, EZ, and EIG |
| Total (03+06+09+12+15+18+20) | 21 | 03+06+09+12+15+18+20 |

## I.V.A. Deductibles {#bridgehead_N2003197}

|  | Base | Tax Payable |
| --- | --- | --- |
| Taxable purchase transactions in country | 22 | Net amount of S, R, R2, Z, RC, and ESSP | 23 | Tax amount of S, R, R2, and Z purchases, Notional amount of RC purchases, Notional amount of ESSP |
| Capital goods transactions | 24 | CG | 25 | CG |
| Imports of current assets | 26 | CA | 27 | CA |
| Imports of investment goods | 28 | IG | 29 | IG |
| Intra-Community acquisition of goods | 30 | Net amount of ES, ER, and EZ | 31 | Notional VAT of ES, ER, and EZ |
| Intra-Community acquisition of goods investments | 32 | EIG | 33 | Notional VAT of EIG |
| Compensation regime spices A G | 34 | Editable field |
| Regularization investments | 35 | RI |
| Regularization by application of the final percentage of pro-rata | 36 | Editable field |
| Total to deduct (23+25+27+29+31+33+34+35+36) | 37 | 23+25+27+29+31+33+34+35+36 |
| Difference (21-37) | 38 | 21 - 37 |
| Attributable to the administration of the state | 39 | Editable field | 40 | Editable field |
| Contributions for previous periods | 41 | Editable field |
| Intra-Community Deliveries | 42 | Net amount of ES, ER, EZ, and ESSS sales |
| Exports and other operations | 43 | Net amount of O and OS sales |
| Reverse charge leading to deductions | 44 | Net amount of RC sales |
| Exclusively for taxable persons who are jointly taxed at the state and forales | 45 | Editable field |
| Result (40+41+45) | 46 | 40+41+45 |
| Deduct earlier deductions | 47 | Editable field |
| Result (46-47) | 48 | 46 - 47 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Spain Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1999320.html)
-   [Spain VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2001072.html)
-   [EU Sales List for Spain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2004312.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
