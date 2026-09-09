---
id: "section_N1929852"
type: "section"
title: "What goes into each box - Ireland VAT 3 report"
branch: "ireland-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Ireland Help Topics > Ireland Tax Topics For Accounts Without SuiteTax > Ireland VAT Reports > What goes into each box - Ireland VAT 3 report"
parent: "section_N1929434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1929852.html"
anchors: []
sha256: "2bda4b9fc77b51be523874ea7e1cc694a90268986d04d4f8d6776f7f982ee52e"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Ireland VAT 3 report.

| Box | Description | Value |
| --- | --- | --- |
| T1 | VAT on Sales | VAT amount of Sales S-IE, S1-IE, R-IE, SR-IE, LR-IE, FR-IE Notional tax amount of Purchases RC-IE, RC1-IE, ES-IE, ES1-IE, ER-IE, ESSP-IE, ESSP1-IE, ESPR-IE, IS-IE, IS1-IE, ESR-IE, ELR-IE, EFR-IE, IPA1-IE, IPA2-IE, IPA3-IE, IPA4-IE VAT amount of Sales Adjustment BoxT1, S-IE, S1-IE, R-IE, SR-IE, LR-IE, FR-IE |
| T2 | VAT on Purchases | (VAT amount of Purchases S-IE, S1-IE, R-IE, I-IE, I1-IE, SR-IE, LR-IE, FR-IE + Notional tax amount of Purchases RC-IE, RC1-IE, ES-IE, ES1-IE, ER-IE, ESSP-IE, ESSP1-IE, ESPR-IE, IS-IE, IS1-IE, ESR-IE, ELR-IE, EFR-IE, IPA1-IE, IPA2-IE, IPA3-IE, IPA4-IE + VAT amount of Purchases Adjustment BoxT2, S-IE, S1-IE, R-IE, I-IE, I1-IE, SR-IE, LR-IE, FR-IE) - VAT amount of NonDeductible NonDeduct-IE |
| T3 | Excess of T1 over T2 (Payable) | T1 - T2. Box shows value if positive. Otherwise, box shows zero. |
| or T4 | Excess of T2 over T1 (Repayable) | T2 - T1. Box shows value if positive. Otherwise, box shows zero. |
|  | Amount of Payment | Box shows value of T3, but field is editable. |
| E1 | Value of Goods Sent to other EU Countries | Net amount of Sales ES-IE, ES1-IE, ER-IE, ESR-IE, EE-IE, EZ-IE |
| E2 | Value of Goods Received from other EU Countries | Net amount of Purchases ES-IE, ES1-IE, ER-IE, ESR-IE, EE-IE, EZ-IE |
| ES1 | Total Services to other EU countries | Net amount of Sales ESSS-IE, ESSS1-IE |
| ES2 | Total Services from other EU countries | Net amount of Purchases ESSP-IE, ESSP1-IE, ESPR-IE |
| PA1 | Postponed Accounting | Net amount of Purchases IPA1-IE, IPA2-IE, IPA3-IE, IPA4-IE |

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
