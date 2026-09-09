---
id: "section_N1987905"
type: "section"
title: "What goes into each box - Singapore GST F5 Return"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Tax Topics for Accounts Without SuiteTax > Singapore GST Report > What goes into each box - Singapore GST F5 Return"
parent: "section_N1987604"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987905.html"
anchors: []
sha256: "674495ce3b1b4d5f7a97ca38a780074f0415d1d2aeff0b65e048be53f48a441b"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page is not supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Singapore GST F5 Return.

| Box |  | Tax Codes | Amount |
| --- | --- | --- | --- |
| **Supplies** |
| 1 | Total value of standard-rated supplies | Sales NET amount SR-SG, DS-SG,SRCA-S-SG, SROVR-RS-SG, SROVR-LVG-SG, SRLVG-SG + Purchases NET amount SRRC-SG, SRCA-C-SG | Net amount |
| 2 | Total value of zero-rated supplies | Sales NET amount ZR-SG | Net amount |
| 3 | Total value of exempt supplies | Sales NET amount ES33-SG, ESN33-SG | Editable field but defaults to net amount of transactions with tax property 'Exempt' (ES33 and ESN33 tax codes) Absolute value of net realized gain/loss arising from customer payments in foreign currency |
| 4 | Total value of (1)+(2)+(3) | Boxes 1+2+3 |
| **Purchases** |
| 5 | Total value of taxable purchases | Purchases NET amount TX-SG, TX-E33-SG, TXCA-SG, TXCA2-SG, TX-N33-SG, TX-RE-SG, ZP-SG, IM-SG, ME-SG | Net amount |
| **Taxes** |
| 6 | Output tax due | Sales Tax Amount SR-SG, DS-SG, SROVR-RS-SG, SROVR-LVG-SG, SRLVG-SG + Purchases Notional Amount SRRC-SG, SRCA-C-SG | Editable field but defaults to the amount of GST output tax from the Saved Report |
| 7 | Input tax and refunds claimed | Purchases Tax Amount TX-SG, IM-SG, TX-E33-SG, TX-N33-SG, TX-RE-SG + Purchases Notional Amount TXCA-SG, TXCA2-SG | Editable field but defaults to the amount of GST input tax from the Saved Report |
| 8 | Equals: Net GST to be paid to IRAS | Box 6 - Box 7 |
| **Applicable to Taxable Persons under Major Exporter Scheme/Approved 3rd Party Logistics Company Scheme Only/Other Approved Schemes Only** |
| 9 | Total value of goods imported under MES/ Approved 3PL/ Other Approved Schemes | Editable field + Purchase NET amount ME-SG | Net amount |
| **Did you make the following claims in Box 7?** |
| 10 | Did you claim for GST you had refunded to tourists? | Editable field (if Yes) |
| 11 | Did you make any bad debt relief claims and/or refund claims for reverse charge transactions? | Editable field (if Yes) |
| 12 | Did you make any pre-registration claims? | Editable field (if Yes) |
| **Revenue** |
| 13 | Revenue for the accounting period | Editable field but defaults to the amount from Box 4 |
| 14 | Did you import services and low-value goods subject to GST under reverse charge? | Editable field + Purchase net amount SRRC-SG |
| 15 | Did you operate an electronic marketplace to supply remote services (includes digital services and non-digital services) subject to GST on behalf of third-party suppliers? | Editable field + Sales net amount SROVR-RS-SG |
| 16 | Did you operate as a redeliverer, or an electronic marketplace to supply imported low-value goods subject to GST on behalf of third-party suppliers? | Editable field + Sales net amount SROVR-LVG-SG |
| 17 | Did you make your own supply of imported low-value goods that is subject to GST? | Editable field + Sales net amount SRLVG-SG |
| **Import GST Deferment Scheme** |
| 18 | Net GST per box 8 above | Defaults to the amount from Box 8 |
| 19 | Add: Deferred import of GST payable | Editable field |
| 20 | Equals: Total tax to be paid to IRAS | Box 16 + 17 |
| 21 | Total value of goods imported under this scheme | Editable field |

-   Position your mouse pointer over the callout icon ![alt=''](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/callouticon.png) of box 19 to see the amount of GST on Imports. This amount represents the total GST of transactions with the IM tax code.
    
-   Position your mouse pointer over the callout icon ![alt=''](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/callouticon.png) of box 21 to see the Total value of goods imported. This value represents the net amount of transactions with the IM tax code.
    

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html)
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Accounting for Goods and Services Tax - Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html)
-   [Singapore GST Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987604.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
