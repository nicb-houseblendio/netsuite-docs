---
id: "section_N1865743"
type: "section"
title: "Chile Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Chile Tax Topics > Chile Tax Codes"
parent: "chapter_N1865199"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1865743.html"
anchors: ["subsect_1030015027", "bridgehead_N1865810"]
sha256: "a0401440e4c36553295ae4f2d3386880ffad96d4ed36bf9c7ecb08fb93550250"
---

Tax codes determine how much tax is paid on each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, make sure that the tax codes for Chile are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Important Things to Note {#subsect_1030015027}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## Tax Code Table for Chile {#bridgehead_N1865810}

The following table shows the tax properties required to correctly generate the Chile tax reports provided by the International Tax Reports SuiteApp. The tax code names used in the following table are suggested names. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

Important:

Please consult your tax agency for the correct tax rates.

| Tax Code | Description | Rate | Property | Available On |
| --- | --- | --- | --- | --- |
| E-CL | IVA Exempt | 0% | Exempt | Both (Sales and Purchases) |
| EElec-CL | IVA Exempt Electronic | 0% | E-invoice Exempt | Both (Sales and Purchases) |
| ENop-CL | IVA Exempt Nonoperational | 0% | Exempt Nonoperational Transaction | Both (Sales and Purchases) |
| I-CL | IVA Import | 19% | Import | Both (Sales and Purchases) |
| INoc-CL | IVA Import Without Tax Credit | 19% | Import No Tax Credit | Both (Sales and Purchases) |
| INop-CL | IVA Import Nonoperational | 19% | Import Nonoperational Transaction | Both (Sales and Purchases) |
| S-CL | IVA Standard | 19% | Default | Both (Sales and Purchases) |
| SElec-CL | IVA Standard Electronic Invoice | 19% | E-invoice | Both (Sales and Purchases) |
| SElecNoc-CL | IVA Standard Electronic Invoice Without Tax Credit | 19% | E-invoice No Tax Credit | Both (Sales and Purchases) |
| SNoc-CL | IVA Standard Without Tax Credit | 19% | No Tax Credit | Both (Sales and Purchases) |
| SNop-CL | IVA Standard Nonoperational | 19% | Nonoperational Transaction | Both (Sales and Purchases) |
| X-CL | IVA Export | 0% | Export | Both (Sales and Purchases) |

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Chile Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1865357.html)
-   [Chile VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1867667.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
