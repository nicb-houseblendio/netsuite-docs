---
id: "section_N2030237"
type: "section"
title: "What goes into each box - United Kingdom VAT100 report"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom Tax Topics For Accounts Without SuiteTax > United Kingdom VAT100 Tax Report > What goes into each box - United Kingdom VAT100 report"
parent: "section_N2029877"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2030237.html"
anchors: []
sha256: "fa8f4e6952ade7521bd54a378a8fa74c42ea3fedfd6054f7dd813439fe85d873"
---

Note:

This topic is for NetSuite accounts that use the Tax Reports (International) page to generate the United Kingdom VAT100 Return. If you are using the Country Tax Report page, see [Periodic VAT Return - VAT100](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156775976739.html).

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the United Kingdom VAT100 report.

| Box | Label | Tax Codes |
| --- | --- | --- |
| 1 | VAT due on sales and other outputs | Sales tax amounts of S-GB, R-GB, R1-GB + Purchases notional tax amounts of RC-GB, RC1-GB, RCS-GB, RCS1-GB, ESSP-GB, IPA1-GB, IPA2-GB Tax amount of sales adjustment in box 1 with S-GB, R-GB, R1-GB |
| 2 | VAT due in this period on intra-community acquisitions of goods made in Northern Ireland from EU Member States | Purchases notional tax amounts of ES-GB, ER-GB, EZ-GB |
| 3 | Total VAT due (the sum of boxes 1 and 2) | Box 1 + Box 2 |
| 4 | VAT reclaimed in this period on purchases and other inputs (including acquisitions from the EC) | Purchases tax amounts of S-GB, R-GB, R1-GB + Purchases notional tax amounts of RC-GB, RC1-GB, ESSP-GB, RCS-GB, RCS1-GB, ES-GB, ER-GB, IPA1-GB, IPA2-GB + Net and Tax amount of IV-GB Tax amount of purchases adjustment in box 1 with S-GB, R-GB - Nondeductible tax amounts of S-GB, R-GB Note: For IV tax code, both the net and tax amount is reported by default due to a limitation. Please set net amount to 0 if you need only tax amount reported. |
| 5 | Net VAT to be paid to Customs or reclaimed by you (difference between boxes 3 and 4) | Box 3 - Box 4 |
| 6 | Total value of sales and all other outputs excluding any VAT. Include your box 8 figure. | Sales net amounts of S-GB, R-GB, Z-GB, O-GB, E-GB, RC-GB, RC1-GB, ESSS-GB, ES-GB, ER-GB, ESSN-GB, EZ-GB, R1-GB + Purchases net amounts of ESSP-GB, RCS-GB, RCS1-GB |
| 7 | Total value of purchases and all other inputs excluding any VAT. Include your box 9 figure. | Purchases net amounts of S-GB, R-GB, Z-GB, I-GB, E-GB, RC-GB, RC1-GB, ESSP-GB, RCS-GB, RCS1-GB, ES-GB, ER-GB, EZ-GB, IPA1-GB, IPA2-GB, R1-GB + Deductible net amounts of S-GB, R-GB |
| 8 | Total value of intra-community dispatches of goods and related costs (excluding VAT) from Northern Ireland to other EU Member States | Sales net amounts of ES-GB, ER-GB, EZ-GB |
| 9 | Total value of intra-community acquisitions of goods and related costs (excluding VAT) made in Northern Ireland from EU Member States, | Purchases net amounts of ES-GB, ER-GB, EZ-GB |

### Related Topics:

-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Setting Up Tax Filing for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029554.html)
-   [United Kingdom VAT100 Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029998.html)
-   [Generating a United Kingdom VAT100 Tax Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2031051.html)
-   [Making Tax Digital for VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543299566.html)
-   [Making Tax Digital for VAT Overview and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833477.html)
-   [Submitting MTD VAT Returns to HMRC](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833633.html)
-   [Submitting an MTD VAT Return in a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547520822.html)
-   [Viewing Submission History of United Kingdom MTD CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1558408249.html)
-   [Viewing Previously Submitted MTD VAT Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833722.html)
-   [Viewing the MTD VAT Return Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833748.html)
-   [Handling MTD VAT Return Submission Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156385546699.html)
-   [Exporting a United Kingdom VAT Return to Excel](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833696.html)
-   [Sending of MTD Anti-Fraud Headers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161597724226.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
