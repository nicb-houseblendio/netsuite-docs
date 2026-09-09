---
id: "section_N2039577"
type: "section"
title: "Creating Tax Codes - U.S. Nexus"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > Taxation Features For Accounts without SuiteTax > Creating Tax Codes - U.S. Nexus"
parent: "section_156940239941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html"
anchors: ["procedure_N2039609"]
sha256: "442253bcbfccf1d5b2a2da98d6a209a329b2747f07e5e03a0b82636b7c639db5"
---

Before you set up a tax code, you must first set up a vendor record for each taxing agency. To do this, go to _Lists > Relationships > Vendors > New_. On the **Info** subtab, select **Tax agency** in the **Category** field.

#### To create a U.S. tax code: {#procedure_N2039609}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  Click the nexus for which you want to create a tax code.
    
3.  In the **Tax Name** field, enter a name to identify this tax code.
    
4.  In the **Display Name/Code**, enter a unique name or number that you want to use for this tax code in addition to the tax name.
    
5.  In the **Description** field, enter the text that you want to appear on invoices or receipts that use this tax code.
    
6.  In the **Rate** field, enter the appropriate tax rate as a percentage (such as **3.5%** ).
    
7.  In the **Tax Type** field, select the tax type for the tax code you are creating.
    
    The tax control account for this tax type is selected by default.
    
    For more information about tax types, see [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).
    
8.  In the **Tax Agency** field, select the tax agency that this tax is paid to. If the tax agency does isn't available in the dropdown list, create a tax agency. Default tax agencies are automatically set up when a subsidiary or nexus is created, but you must edit the tax agency vendor record to provide details. To create a tax agency vendor record, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).
    
9.  A default tax control account is shown in the **Tax Account** field. You can select a different tax control account.
    
    You can create tax control accounts at _Setup > Accounting > Taxes > Tax Control Accounts_.
    
10.  The following fields are used to determine the sales tax to charge when you enter orders for your customers and when customers order from your web store:
     
     1.  In the **County** field, enter the name of the county where this tax applies.
         
     2.  In the **City** field, enter the name of the city where this tax applies.
         
     3.  In the **State** field, select the state where this tax applies.
         
     4.  In the **Zip Codes** field, enter the zip codes where this tax applies.
         
11.  Click **Save**.
     

Now, you can either use this tax code to calculate tax for orders, or you add this tax code to a tax group.

For more information about tax codes, see [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html)
-   [Paying Sales Tax - United States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html)
-   [U.S. Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042330.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
