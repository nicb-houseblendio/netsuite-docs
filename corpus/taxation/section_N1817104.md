---
id: "section_N1817104"
type: "section"
title: "Creating Acquisition Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Creating Tax Codes - Other Nexuses > Creating Acquisition Tax Codes"
parent: "section_N1816436"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817104.html"
anchors: ["procedure_N1817131"]
sha256: "aff41b0203fd2a41cab7156db13a8b3bc223d9045acc45476a2d6efffb8b36fa"
---

Acquisition tax is calculated for goods purchased by EU businesses from vendors in other EU countries. Acquisition tax represents the tax that would have been paid had the goods been purchased outside the EU. Acquisition tax paid for purchases is offset by an equal purchase tax amount. Both the acquisition tax and the purchase tax are shown on VAT reports for transactions with vendors in other EU countries.

You can create tax codes for acquisition tax by selecting a notional tax rate on the tax code record.

#### To create an acquisition tax code: {#procedure_N1817131}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  Enter a name or abbreviation for this tax code.
    
3.  In the **Rate** field, enter 0%.
    
4.  Enter the date range this tax code is applicable.
    
5.  Check the **EC Code** box.
    
6.  In the **Notional Rate Derived From** field, select the tax code that thisn'tional tax rate is based on.
    
7.  In the **Tax Type** field, select **VAT**.
    
8.  In the **Available On** field, select **Purchase Transactions**.
    
9.  Click **Save**.
    

You can now select this tax code on purchase transactions.

When you view the VAT on Purchases Summary and Detail reports, the **Notional Tax Amount** column shows the acquisition tax amounts.

To understand tax code properties and how they are used for generating the VAT/GST reports from NetSuite, read the country-specific tax topics. For most countries, a tax code table is provided for guidance.

### Related Topics

-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Creating Tax Codes - Other Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html)
-   [Paying Tax Liabilities - Non-U.S. Editions and Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817593.html)
-   [VAT and GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2050955.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
