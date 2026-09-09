---
id: "section_N1823395"
type: "section"
title: "Applying Nondeductible Input Tax on Transactions"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Recording Nondeductible Input Tax > Applying Nondeductible Input Tax on Transactions"
parent: "section_N1822590"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1823395.html"
anchors: ["procedure_N1823419", "bridgehead_4677065000"]
sha256: "9048d8b717deb18b7aa0aaf7ebe2751e223239de972b73077bb25e67a4988a78"
---

Important:

Supplementary Tax Calculation SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

Note:

This feature is available for vendor bills, expense reports, checks, and vendor bill credits for countries that the [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) SuiteApp supports.

Important:

NetSuite does not recommend memorizing transactions or using the Make Copy function on existing transactions (with nondeductible tax) generated using the International Tax Reports SuiteApp. Doing so will cause inaccuracies with the computation of the Supplementary Tax Calculation SuiteApp. You can create a new transaction instead, and manually copy the details of the existing transaction onto the new one.

#### To apply nondeductible tax on a transaction: {#procedure_N1823419}

1.  Create a new transaction.
    
2.  Add items or expenses with nondeductible tax by using a tax code that represents the reclaimable portion of the VAT.
    
3.  In the **Expense Account** column, make sure that the correct account is selected.
    
4.  To view the computed nondeductible tax amount on the transaction, open the transaction record, and then click **Actions** > **GL Impact**.
    
    ![Example of nondeductible tax amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/STC_GLImpact.png)

## Reporting of Nondeductible Input Tax {#bridgehead_4677065000}

For boxes in the VAT returns that require nondeductible input tax, the amount is calculated by deducting the nondeductible input tax from the full input tax amount.

![Example of nondeductible input tax deduction from the full input tax amount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/NDTaxReporting.png)

Note:

Consolidated or group reporting isn't supported.

### Related Topics

-   [Recording Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822590.html)
-   [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
