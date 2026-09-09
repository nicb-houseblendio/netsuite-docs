---
id: "section_N1856762"
type: "section"
title: "Creating Tax Codes - Canada"
branch: "canada-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Canada Help Topics > Canada Tax Topics For Accounts Without SuiteTax > Creating Tax Codes - Canada"
parent: "section_156941156434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856762.html"
anchors: ["procedure_N1856781", "procedure_N1856919"]
sha256: "c13de93e77afa2d0d951be6f56a872122d4d64f6f71e8f8de4785eb16875a101"
---

It is important to create tax codes for several reasons:

-   Tax codes help you track taxes after you specify the tax codes on your transaction records.
    
-   Tax codes contain information about tax rates and the transaction types they should be applied to.
    
-   Tax codes help you apply special tax conditions, for example tax exemption.
    

For more information about tax codes, see [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html).

#### To create a tax code for Canada: {#procedure_N1856781}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  If you are using NetSuite OneWorld, click the **Canada** nexus link.
    
3.  In the **Tax Name** field of the Tax Code page, enter a name or an abbreviation for this tax code .
    
    This code appears in the **Tax Code** column on sales transactions.
    
4.  In the **Display Name/Code** field, enter a name or code that NetSuite should display instead of the name entered in the **Tax Name** field. For example, if you enter **PST** in the **Tax Name** field, you can enter **Provincial Sales Tax** in the **Display Name/Code** field.
    
5.  Enter a description for this tax code.
    
6.  In the **Rate** field, enter the tax percentage that the nexus, or jurisdiction, charges on an item with this tax code.
    
7.  In the **Province** field, enter the name of the province that collects the tax associated with this tax code.
    
8.  In the **Tax Type** field, select a tax type (for example, **GST** or **PST**) for this tax code.
    
9.  Select the tax agency to which your company pays this tax.
    
    You can set up vendor records for tax agencies. For more information, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).
    
10.  In the **Purchase Tax Account** field and **Sales Tax Account** field, select the general ledger account for this tax code.
     
11.  Check the **Exclude from Tax Report** box if you don't want this tax code reflected in tax reports.
     
12.  Clear the **Inactive** box to make this tax code available on transactions.
     
13.  Click **Save**.
     

Now, you can add this tax code to a transaction or tax group.

Important:

The **Tax Type** field on the tax code record can no longer be changed if the tax code has already been added to a tax group.

You can create tax codes for customers that are exempt from paying Provincial Sales Tax (PST).

To do this, you first create a 0% tax code for the PST.

#### To create a 0% PST tax code: {#procedure_N1856919}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  If you are using NetSuite OneWorld, click the **Canada** nexus link.
    
3.  In the **Tax Name** field of the Tax Code page, enter a name or an abbreviation for this tax code.
    
4.  In the **Display Name/Code** field, enter a name or code that NetSuite should display instead of the name entered in the **Tax Name** field. For example, if you enter **PST** in the **Tax Name** field, you can enter **Provincial Sales Tax** in the **Display Name/Code** field.
    
5.  In the **Description** field, enter a description for this tax code.
    
6.  In the **Rate** field, enter **0%**.
    
7.  In the **Tax Type** field, select **PST**.
    
    For more information about Tax Types, see [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).
    
8.  Select the tax agency associated with this type of tax.
    
9.  Select the tax control account that you want to use to track this tax on purchases and on sales.
    
10.  Click **Save**.
     

Now, you can create a new tax group to apply to PST-exempt customers. On the tax code record, select the province and the Goods and Services Tax/Harmonized Sales Tax (GST/HST) item you want to apply with this tax code. In the **PST** field, select the 0% tax PST tax code you created, and click **Save**.

For more information, see [Setting Tax Preferences for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html) and [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html).

In the **Tax Code for Out-of-Province Sale** field on the **Canada** tab at _Setup > Accounting > Taxes > Set Up Taxes_, you can select a tax code to apply to orders placed by PST-exempt customers.

### Related Topics

-   [Setting Tax Preferences for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html)
-   [Creating Tax Groups - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857206.html)
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)
-   [Viewing Canadian Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1860262.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Processing Goods and Services Tax (GST) Refunds - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859567.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
