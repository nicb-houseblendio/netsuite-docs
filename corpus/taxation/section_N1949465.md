---
id: "section_N1949465"
type: "section"
title: "Peru Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Peru Tax Topics > Peru Tax Codes"
parent: "chapter_N1949362"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1949465.html"
anchors: ["subsect_1030033705", "bridgehead_N1949524"]
sha256: "521b83bec2ce0537ef361b859b12708e0fc277572b0b8e37fdb03e3c6466613d"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Peru are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030033705}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Peru {#bridgehead_N1949524}

The following table shows the tax properties required to correctly generate the Peru tax reports provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Rate | Property | Tax Type | Purchase Tax Account | Sales Tax Account | Available On |
| --- | --- | --- | --- | --- | --- | --- | --- |
| E-PE | IGV Exempt | 0% | Exempt | IGV\_PE | IGV on Purchases | IGV on Sales | Both (Sales and Purchases) |
| I-PE | IGV Import | 18% | Import | IGV\_PE | IGV on Purchases |  | Purchases |
| IE-PE | IGV Exempt on Import | 0% | Import Exempt | IGV\_PE | IGV on Purchases |  | Purchases |
| INoc-PE | IGV Import Without Tax Credit | 18% | Import No Tax Credit | IGV\_PE | IGV on Purchases |  | Purchases |
| IUn-PE | IGV Import With Unknown Credit | 18% | Import Unknown Tax Credit | IGV\_PE | IGV on Purchases |  | Purchases |
| S-PE | Standard IGV | 18% | Default | IGV\_PE | IGV on Purchases | IGV on Sales | Both (Sales and Purchases) |
| SNoc-PE | IGV Without Tax Credit | 18% | No Tax Credit | IGV\_PE | IGV on Purchases |  | Purchases |
| SNop-PE | IGV Non Operational Sales | 18% | Non Operational | IGV\_PE |  | IGV on Sales | Sales |
| SUn-PE | IGV Purchases With Unknown Credit | 18% | Unknown Tax Credit | IGV\_PE | IGV on Purchases |  | Purchases |
| X-PE | IGV Export | 0% | Export | IGV\_PE |  | IGV on Sales | Sales |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Peru VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1950682.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
