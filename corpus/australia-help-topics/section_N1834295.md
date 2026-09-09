---
id: "section_N1834295"
type: "section"
title: "Creating Tax Codes - Australia"
branch: "australia-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Australia Help Topics > Australia Tax Topics > Creating Tax Codes - Australia"
parent: "chapter_N1832106"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1834295.html"
anchors: ["procedure_N1837423"]
sha256: "5830ea4455f584856680b352b65bae8fe81c1d0d70b62db41b751270cb853698"
---

Tax codes determine how much tax is paid on each transaction line item. From your transactions, NetSuite automatically calculates the tax amounts that appear in each box of the Business Activity Statement (BAS). The following table describes the standard tax codes provided by NetSuite for Australia. The last column indicates the boxes on the BAS where the tax amounts are shown.

The tax codes for Australia are already provided by NetSuite. See [Australia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3802804453.html).

If you need to create a new tax code, do the following steps.

#### To create a tax code: {#procedure_N1837423}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  In the **Tax Code** field, enter a name or abbreviation for this tax code.
    
    This code appears in the **Tax Code** column on transactions.
    
3.  In the **Description** field, enter a description for this tax code.
    
4.  In the **Rate** field, enter the tax percentage that is charged on an item with this tax code.
    
5.  In the **Effective From** field, enter the date this tax code first goes into effect.
    
6.  In the **Valid Until** field, enter the last date this tax code is in effect.
    
7.  In the **Tax Agency** field, select the tax agency that this tax is paid to.
    
    You can set up vendor records for tax agencies. For more information, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).
    
8.  In the **Tax Type** field, select the tax type for this tax code.
    
    When you select a tax type, the tax control accounts for this tax type appear in the **Purchase Tax Account** and **Sales Tax Account** fields. You can create new tax types at _Setup > Accounting > Taxes > Tax Types ( Administrator )_. For more information about Tax Types, see [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).
    
9.  In the **Available On** field, select the types of transactions that this tax code can be applied to.
    
10.  Check the appropriate tax properties:
     
     -   **Exempt** - to indicate that whatever this code applies to is exempt from tax
         
     -   **Default Code** - if you want this tax code to be selected by default on transactions
         
     -   **Export** - if this tax code is used for international sales
         
     -   **Exclude From GST Reports** - if you do not want this tax code to appear on reports
         
11.  Check the **Inactive** box if you want to inactivate this tax code. Inactive tax codes do not show in lists on transactions and records.
     
12.  Click **Save**.
     

### Related Topics

-   [Setting Tax Preferences for Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1832322.html)
-   [Australia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3802804453.html)
-   [Using Wine Equalization Tax (WET)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3830143961.html)
-   [Accounting for Goods and Services Tax (GST) - Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1833730.html)
-   [Setting Up Your Business Activity Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1834047.html)
-   [Viewing Australian Goods and Services Tax (GST) Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1837720.html)
-   [Australia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1832106.html)
-   [Australia Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1595666.html)
-   [Shipping Integration with Australia Post](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274389015.html)
-   [Setting Up Australia-specific Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540889422.html)
-   [Australia Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540887347.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
