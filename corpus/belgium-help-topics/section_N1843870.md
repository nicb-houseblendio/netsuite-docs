---
id: "section_N1843870"
type: "section"
title: "What goes into each box - Belgium VAT report"
branch: "belgium-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Belgium Help Topics > Belgium Tax Topics In Accounts Without SuiteTax > Belgium VAT Report > What goes into each box - Belgium VAT report"
parent: "section_N1843546"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1843870.html"
anchors: []
sha256: "51a098c0001f7ded8afa13b41ec65d36f7f6d68b4dfce9deb7fbb0b5d5d62a4f"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Belgium VAT report.

| **II. Output Operations** |
| --- |
| A | Transactions subject to a VAT rate of 0% | Net amount of Sales Z-BE | 00 |
| B | Activities under which VAT is due by the declarant: |  |  |
|  | \- Taxable sales at 6% | Net amount of Sales SR-BE, SRS-BE | 01 |
|  | \- Taxable sales at 12% | Net amount of Sales R-BE, RS-BE | 02 |
|  | \- Taxable sales at 21% | Net amount of Sales S-BE, SS-BE | 03 |
| C | Services for which the foreign VAT is payable by the contractor (EC Services) | Net amount of Sales ESSS-BE | 44 |
| D | Operations for which the VAT is due by the contractor | Net amount of Sales RC-BE | 45 |
| E | Exempt intracommunity supplies | Net amount of Sales ES-BE, ER-BE, EZ-BE | 46 |
| F | Other exempted operations and transactions abroad | Net amount of Sales E-BE, O-BE, OS-BE | 47 |
| G | Total amount of credit notes issued and negative corrections to sales figures: |  |
|  | \- Credit notes on intracommunity supplies | Net amount of sales EZ-BE, ESSS-BE, ES-BE, ER-BE | 48 |
|  | \- Credit notes on other transactions | Net amount of sales S-BE, R-BE, RC-BE, O-BE, OS-BE, SR-BE, E-BE, Z-BE, SS-BE, RS-BE, SRS-BE | 49 |
| **III. Input Operations** |
| A | Total amount of receipts including credit notes received and other positive corrections: |  |
|  | \- Goods and raw materials and components | Net amount of purchases S-BE, R-BE, SR-BE, O-BE, OS-BE, ES-BE, EZ-BE, ER-BE, RC-BE, RCND-BE, EDCSP-BE, I-BE, Z-BE, E-BE, ID-BE + Deduct Net amount for S-BE, R-BE, SR-BE + Non-Deduct Tax amount for S-BE, R-BE, SR-BE Note: The value of this box will display zero if the total bill credits exceed the total bills. | 81 |
|  | \- Incoming services and other assets | Net amount of purchases SS-BE, RS-BE, SRS-BE, EP-BE, ESSP-BE, E2-BE, IS-BE, FA2-BE, ISND-BE + Deduct Net amount for SS-BE, RS-BE, SRS-BE, FA2-BE + Non-Deduct Tax amount for SS-BE, RS-BE, SRS-BE, FA2-BE, ESSP-BE, IS-BE Note: The value of this box will display zero if the total bill credits exceed the total bills. | 82 |
|  | \- Investment assets | Net amount of purchases FA-BE, ECFA-BE, RCFA-BE, RCFAND-BE + Deduct Net amount for FA-BE + Non-Deduct Tax amount for FA-BE Note: The value of this box will display zero if the total bill credits exceed the total bills. | 83 |
| B | Total amount of credit notes received and negative corrections: |  |
|  | \- Relating to the operations listed in 86 and 88 | Net amount of purchases ES-BE, EP-BE, ER-BE, EZ-BE, ECFA-BE, ESSP-BE, EDCSP-BE | 84 |
|  | \- Credit notes on other transactions | Net amount of purchases S-BE, R-BE, SR-BE, RC-BE, I-BE, IS-BE, E-BE, E2-BE, SS-BE, RS-BE, SRS-BE, OS-BE, FA-BE, FA2-BE, Z-BE, ISND-BE, RCFA-BE + Deduct Net amount for S-BE, R-BE, SR-BE, SS-BE, RS-BE, SRS-BE, FA-BE, FA2-BE + Non-Deduct Tax amount for S-BE, R-BE, SR-BE, SS-BE, RS-BE, SRS-BE, FA-BE, FA2-BE | 85 |
| C | Acquisitions from EU member countries | Net amount of purchases ES-BE, EP-BE, ECFA-BE, ER-BE, EZ-BE Note: The value of this box will display zero if the total bill credits exceed the total bills. | 86 |
| D | Other incoming transactions for which VAT is due by the declaring party | Net amount of purchases RC-BE, IS-BE, I-BE, RCND-BE, RCFA-BE, ISND-BE, RCFAND-BE, OS-BE Note: The value of this box will display zero if the total bill credits exceed the total bills. | 87 |
| E | Services purchased from EU member countries | Net amount of purchases ESSP-BE, EDCSP-BE Note: The value of this box will display zero if the total bill credits exceed the total bills. | 88 |
| **IV. Taxes Due** |
| A | VAT relating to transactions declared in: |  |
|  | \- VAT due on boxes 01 to 03 | VAT amount of sales S-BE, R-BE, SR-BE, SS-BE, RS-BE, SRS-BE + Tax amount of sales adjustment in box 54 with S-BE, R-BE, SR-BE, SS-BE, RS-BE, SRS-BE | 54 |
|  | \- VAT due on intra-community acquisitions and services | Notional amount of purchases ES-BE, EP-BE, ESSP-BE, ER-BE, ECFA-BE, EDCSP-BE, EZ-BE | 55 |
|  | \- Box 87, excluding provisions on imports | Notional purchase tax amount RC-BE, RCND-BE, RCFA-BE, RCFAND-BE, OS-BE, IS-BE, ISND-BE | 56 |
| B | VAT due on imports | Notional amount of purchases I-BE + Net amount of purchases IV-BE | 57 |
| C | Other previously undeclared taxes in favour of the state | Notional purchase tax amount: RCFA-BE, RC-BE, ES-BE, ER-BE, EZ-BE, ESSP-BE, IS-BE + Inputted amount | 61 |
| D | VAT due on credit notes received | VAT amount of purchases S-BE, SS-BE, R-BE, RS-BE, SR-BE, SRS-BE, I-BE, Z-BE, FA-BE, FA2-BE + Notional amount of purchases: RC-BE, OS-BE, IS-BE + Deduct Net amount for S-BE, SS-BE, R-BE, RS-BE, SR-BE, SRS-BE, FA-BE, FA2-BE - Non-Deduct Tax amount for S-BE, SS-BE, R-BE, RS-BE, SR-BE, SRS-BE, FA-BE, FA2-BE | 63 |
|  | Don't complete |  | 65 |
|  | Sum of 54, 55, 56, 57, 61 and 63 | Box 54 + 55 + 56 + 57 + 61 + 63 | XX |
| **V. Taxes Deductible** |
| A | Deductible VAT | VAT amount of purchases S-BE, SS-BE, R-BE, RS-BE, SR-BE, SRS-BE, FA-BE, FA2-BE + Notional amount of purchases RC-BE, OS-BE, IS-BE, ES-BE, ER-BE, EP-BE, RCFA-BE, I-BE, ID-BE, EDCSP-BE, ECFA-BE, ESSP-BE + Deduct Net amount for S-BE, SS-BE, R-BE, RS-BE, SR-BE, SRS-BE, FA-BE, FA2-BE - Non-Deduct Tax amount for S-BE, SS-BE, R-BE, RS-BE, SR-BE, SRS-BE, FA-BE, FA2-BE + Tax amount of purchases adjustment in box 59 with S-BE, R-BE, SR-BE, SS-BE, RS-BE, SRS-BE, FA-BE, FA2-BE | 59 |
| B | Other previously undeclared taxes in favour of the declarant | Notional purchase tax amount: RCFA-BE, RC-BE, ES-BE, ER-BE, EZ-BE, ESSP-BE, IS-BE + Inputted amount | 62 |
| C | VAT to claim back on credit notes issued | VAT amount of sales S-BE, R-BE, SR-BE, O-BE, OS-BE, SS-BE, RS-BE, SRS-BE + Tax amount of sales adjustment in box 64 with S-BE, R-BE, SR-BE, SS-BE, RS-BE, SRS-BE | 64 |
|  | Don't complete |  | 66 |
|  | Sum of 59, 62 and 64 | Box 59 + 62 + 64 | YY |
| **VI. Balance** |
|  | VAT due to the State: Box XX - YY | Box XX - YY Note: The value of this box will display zero if the result is negative. | 71 |
|  | VAT due to you: Box YY - XX | Box YY - XX Note: The value of this box will display zero if the result is negative. | 72 |
| **VII. Advance Payments** |
|  | VAT due for the period from 1 to 20 December | Editable field | 91 |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Belgium Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1839652.html)
-   [Setting Up Tax Filing for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1841509.html)
-   [Belgium VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1843546.html)
-   [EU Sales List for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1846111.html)
-   [Intrastat Report for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1552962932.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
