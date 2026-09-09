---
id: "section_N1920183"
type: "section"
title: "What goes into each box - Indonesia VAT report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Indonesia Tax Topics > Indonesia VAT Report > What goes into each box - Indonesia VAT report"
parent: "section_N1919850"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1920183.html"
anchors: ["bridgehead_N1922653", "bridgehead_N1924438"]
sha256: "a772ee3d844c8437efd64ef5118b68edd3726ec11af5b0da91b1137936a9158e"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page is not supported. If you'd like to create nondeductible tax codes that work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

Refer to the following table to understand how NetSuite uses the tax codes to get the values for the VAT Declaration Form 1111 and Form 1111AB.

## Form 1111 {#bridgehead_N1922653}

|  | Amount | VAT |
| --- | --- | --- |
| **I. Delivery of Goods and Services** | \- | \- |
| A. VAT Payable: | \- | \- | \- |
| 1\. Exports | A.1 | Sales Z | Sales Z |
| 2\. Deliveries subject to VAT | 1 | Total from Form 1111AB Section I.C.1 | Total from Form 1111AB Section I.C.1 |
| 3\. Deliveries to designated VAT collectors | 2 | Sales G | Sales G, Sales Adjustment VAT box + G |
| 4\. Deliveries where VAT was not collected | 3 | Sales NV | Sales NV, Sales Adjustment VAT box + NV |
| 5\. Deliveries exempt from VAT | 4 | Sales EX | Sales EX |
| Amount (I.A.1 + I.A.2 + I.A.3 + I.A.4 + I.A.5) | \- | I.A.1 + I.A.2 + I.A.3 + I.A.4 + I.A.5 | I.A.1 + I.A.2 + I.A.3 + I.A.4 + I.A.5 |
| B. VAT not Due | \- | Editable field | \- |
| C. Total of all Deliveries (I.A + I.B) | \- | I.A total + I.B | \- |
| **II. Calculation of VAT Payable/Overpayment** | \- | \- |
| A. Output VAT due for collection (VAT due on I.A.2) | 1 | \- | Total from Form 1111AB Section I.C.1 |
| B. VAT paid in advance in the same period | \- | \- | Editable field |
| C. Input VAT that can be credited | 5 | \- | Total from Form 1111AB Section III.C |
| D. VAT still payable (overpayment) (II.A - II.B - II.C) | \- | \- | II.A - II.B - II.C |
| E. VAT still payable (overpayment) in the corrected SPT form | \- | \- | Editable field |
| F. VAT payable (overpayment) for correction (II.D - II.E) | \- | \- | II.D - II.E |
| G. Underpayments of VAT on (dd-mm-yyyy) | \- | \- | Editable field |
| **III. VAT Payable on Construction Activities** | \- | \- |
| A. Tax Base | \- | Editable field | \- |
| B. VAT Due | \- | Editable field | \- |
| C. Settled On (dd-mm-yyyy) | \- | \- | Editable field |
| **IV. Repayment of Input Tax for Failed Production** | \- | \- |
| A. VAT to be paid back | \- | Editable field | \- |
| B. Settled On (dd-mm-yyyy) | \- | \- | Editable field |
| **V. Sales Tax on Luxury Goods** | \- | \- |
| A. LST due for collection | 1 | \- | This is the same value entered in Form 1111AB I.C.1 under the LST column |
| B. LST tax paid in advance in the same period | \- | \- | Editable field |
| C. LST still payable (overpayment) (V.A - V.B) | \- | \- | V.A - V.B |
| D. LST still payable (overpayment) in the corrected form | \- | \- | Editable field |
| E. LST still payable (overpayment) for correction (V.C - V.D) | \- | \- | V.C - V.D |
| F. LST payable (overpayment) settled on (dd-mm-yyyy) | \- | \- | Editable field |

## Form 1111 AB {#bridgehead_N1924438}

Note:

Although Luxury Sales Tax (PPnBM) fields are provided, NetSuite does not automatically calculate the values for them.

| Description |  | Tax Base | VAT | LST |
| --- | --- | --- | --- | --- |
| **I. Summary of Deliveries** | \- | \- | \- | \- |
| A. Export of Tangible/Intangible Goods and/or Services | A.1 | Sales Z | \- | \- |
| B. Domestic Deliveries | \- | \- | \- | \- |
| 1\. Domestic deliveries without pre-totaled VAT invoice | A.1 | Sales G, NV, EX | Sales G, NV, EX + Sales Adjustment VAT box, S, G, NV, EX | LST (PPnBM) - Editable field for user input |
| 2\. Domestic deliveries with pre-totaled VAT invoice | \- | Editable field | Editable field | Editable field (LST entered here goes into Form IIII V.A.1 under LST column) |
| C. Details of Domestic Deliveries | \- | \- | \- | \- |
| 1\. Deliveries subject to VAT and LST (The amount in I.B.1 with VAT Invoice Code 01, 04, 06 and 09 plus I.B.2) | 1 | Sales S + value in I.B.2 | Sales S + value in I.B.2 | Editable field |
| 2\. Deliveries with VAT where the VAT and LST were collected by the VAT/LST collector (The amount in I.B.1 with VAT Invoice Code 02 and 03) | 2 | Sales G | Sales G + Sales Adjustment VAT box, G | Editable field |
| 3\. Deliveries with VAT where VAT and LST were not collected (The amount in I.B.1 with VAT Invoice Code 07) | 3 | Sales NV | Sales NV + Sales Adjustment VAT box, NV | Editable field |
| 4\. Deliveries exempt from VAT and luxury sales tax (The amount in I.B.1 with VAT Invoice Code 08) | 4 | Sales EX | Sales EX | Editable field |
| **II. Summary of Acquisitions** | \- | \- | \- | \- |
| A. Importation of Goods (BKP), Consumption of Foreign Intangible Goods (BKP) and Services (JKP) outside the customs area where input VAT can be credited | B.1 | Purchases IMPT | Sales IMPT + Sales Adjustment VAT box, IMPT | Editable field |
| B. Acquisition of domestic goods/services BKP where input VAT can be credited | B.2 | Purchases S | Sales S + Sales Adjustment VAT box, S | Editable field |
| C. Imports or acquisitions where input VAT cannot be credited | B.3 | Purchases NC | Sales NC + Sales Adjustment VAT box, NC | Editable field |
| D. Number of acquisitions (II.A + II.B + II.C) | \- | II.A + II.B + II.C | II.A + II.B + II.C | II.A + II.B + II.C |
| **III. Calculation of Input VAT which can be Credited** | \- | \- | \- | \- |
| A. Input VAT on acquisitions which can be credited | \- | \- | Purchases S and IMPT + Purchases Adjustment VAT box, S, IMPT | \- |
| B. Other Input VAT | \- | \- | \- | \- |
| 1\. Compensation of excess VAT from previous tax period | \- | \- | Editable field | \- |
| 2\. Payment of excess for correction in the current form (SPT) submission | \- | \- | Editable field | \- |
| 3\. Additional items that can be included as an addition (deduction) to input VAT | \- | \- | Editable field | \- |
| 4\. Amount (III.B.1 + III.B.2 + III.B.3) | \- | \- | III.B.1 + III.B.2 + III.B.3 | \- |
| C. Total Input VAT which can be included (III.A+ III.B.4) | 5 | \- | III.A+ III.B.4 | \- |

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Indonesia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1918921.html)
-   [Indonesia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1919850.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
