---
id: "section_N1822730"
type: "section"
title: "Setting Up Nondeductible Input Tax"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Recording Nondeductible Input Tax > Setting Up Nondeductible Input Tax"
parent: "section_N1822590"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html"
anchors: ["bridgehead_4636417901", "bridgehead_4637276564", "procedure_4637308358", "procedure_4637311190", "procedure_N1823013", "procedure_N1823115", "bridgehead_4639631439", "procedure_4637312058"]
sha256: "c73d15a0fb9ea6131a9113de754f0ac872b728fa6c4e6fd6f38756adde8925b9"
---

Supplementary Tax Calculation SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

## Prerequisites {#bridgehead_4636417901}

To use the nondeductible input tax feature, make sure the following prerequisites are either installed or enabled on your account:

-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) SuiteApp (Bundle ID: 43003)
    
-   Supplementary Tax Calculation SuiteApp (Bundle ID: 123426)
    
    For more information about how to install a SuiteApp or bundle, see [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).
    
-   Go to Setup > Company > Enable Features and check the box for the following features on the SuiteCloud subtab:
    
    -   Custom Records
        
    -   Client SuiteScript
        
    -   Server SuiteScript
        
    -   Custom GL Lines
        

Before you can use the nondeductible input tax feature in NetSuite, you must do the following:

-   Set up the tax control account and tax codes for nondeductible tax. See [Setting Up Tax Control Account and Tax Codes for Nondeductible Tax](#bridgehead_4637276564).
    
-   Make sure that the Supplementary Tax Calculation plug-in is properly configured. See [Configuring the Supplementary Tax Calculation Plug-in](#bridgehead_4639631439).
    
-   Make sure that your role has the appropriate permissions. See [International Tax Reports Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054820.html).
    
-   If you don't have OneWorld account, be sure to enter an address on the vendor record. In particular, make sure that the Country field isn't blank. The saved search used for nondeductible tax codes checks the Country defined in the vendor record to properly subtract the nondeductible amount from the reclaimed VAT.
    

## Setting Up Tax Control Account and Tax Codes for Nondeductible Tax {#bridgehead_4637276564}

Before you use the nondeductible input tax feature, you have to set up a tax control account where the nondeductible tax will initially post to. After posting to the tax control account, the system will automatically reclassify this tax amount to the appropriate expense account. For more information about specifying the expense account, see [Creating a Tax Code for the Reclaimable Portion of the VAT](#procedure_N1823115).

You also need to set up tax codes to be used for purchases and expenses that have nondeductible tax. You can create as many tax codes as needed to represent different rates applied to nondeductible purchases. If you want to use any of your existing tax codes, you must edit the tax code and, in the **Nondeductible Rate Derived From** field, select the nondeductible tax code. You can also create a tax code for 100% nondeductible tax.

Important:

You should set up new tax codes for partially reclaimable input tax. Make sure that other properties of the existing tax code (for example, reduced rate tax code) are copied to the new tax code for partially reclaimable input tax. For example, if you need a partially reclaimable reduced rate tax code, you need to check the **Reduced Rate** box on the tax code setup for both the partially reclaimable and nondeductible tax codes. This ensures that the tax code will be reported properly.

#### Creating a Tax Control Account {#procedure_4637308358}

1.  Go to _Setup > Accounting > Taxes > Tax Control Accounts > New_.
    
2.  If you are using OneWorld, click the nexus that you are creating a tax control account for.
    
3.  Enter a name for the tax control account, for example **Nondeductible VAT on Purchases**.
    
4.  Enter a description for this tax control account.
    
5.  In the **Tax Account Type** field, select **Purchase**.
    
6.  Click **Save**.
    
7.  If you are using OneWorld, you must assign this account to subsidiaries:
    
    1.  Click the **Edit** link of the account, for example **Nondeductible VAT on Purchases**.
        
    2.  Select the parent company.
        
    3.  Make sure the **Include Children** box is checked.
        
    4.  Click **Save**.
        

#### Creating a Tax Type for Nondeductible Tax {#procedure_4637311190}

1.  Go to _Setup > Accounting > Taxes > Tax Types > New_.
    
2.  If you are using OneWorld, click the nexus that you are creating a tax control account for.
    
3.  Enter a name for the tax type, for example **Nondeductible VAT**.
    
4.  Enter a description for this tax type.
    
5.  In the **Asset/Purchase Tax Account** column, select the tax control account that you created.
    
6.  Click **Save**.
    

#### Creating a Tax Code for the Nondeductible Portion of the VAT {#procedure_N1823013}

1.  Enter a name for the tax code, for example **Nondeductible Tax Code**.
    
2.  Enter a description for the tax code, for example **60% nondeductible**.
    
3.  Enter a rate that represents the nondeductible portion, for example **60%**.
    
4.  Select the subsidiaries that you want this tax code to be available to.
    
5.  In the **Tax Agency** field, make sure the correct tax agency is selected.
    
6.  In the **Tax Type** field, select **Nondeductible VAT**.
    
7.  In the **Purchase Tax Account** field, select **Nondeductible VAT on Purchases**.
    
8.  In the **Available on** field, select **Purchase Transactions**.
    
9.  Check the **Nondeductible** box.
    
10.  Click **Save**.
     

#### Creating a Tax Code for the Reclaimable Portion of the VAT {#procedure_N1823115}

1.  Enter a name for the tax code, for example **40% Reclaimable VAT**.
    
2.  Enter a description for the tax code, for example **40% reclaimable**.
    
3.  Enter the VAT rate that should be applied to purchases, for example **21%** (the standard rate for purchases).
    
4.  In the **Tax Agency** field, make sure the correct tax agency is selected.
    
5.  In the **Tax Type** field, select **VAT**.
    
6.  In the **Purchase Tax Account** field, select **VAT on Purchases**.
    
7.  In the **Available on** field, select **Purchase Transactions**.
    
8.  In the **Nondeductible Rate Derived From** field, select the tax code that represents the nondeductible portion. For example, in the previous procedure, the tax code for the nondeductible portion of the VAT is called **Nondeductible Tax Code (60%)**.
    
9.  In the **Nondeductible Expense Account** field, select the expense account that the nondeductible tax should be posted to, for example **Miscellaneous Expense**.
    
    The selected expense account is the default value for the expense account column on the transaction. You can change this setting before saving the transaction.
    
10.  Click **Save**.
     

Important:

If you are using customized transaction forms for Vendor Bill, Vendor Credit, Expense Report, and Write Check, you must set the following custom tax transaction fields to show on your custom forms, otherwise the nondeductible feature won't work.

-   Custom Transaction Form > Screen Fields > Tax Reporting:
    
    -   **Nondeductible Tax Adjusted**
        
    -   **Nondeductible Adjustment Journal**
        
-   Custom Transaction Form > Screen Fields > Expenses:
    
    **Expense Account**
    
-   Custom Transaction Form > Screen Fields > Items:
    
    **Expense Account**
    

For information about displaying custom fields on transaction forms, see [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html).

## Configuring the Supplementary Tax Calculation Plug-in {#bridgehead_4639631439}

#### To Configure the Supplementary Tax Calculation Plug-in: {#procedure_4637312058}

1.  Go to _Customization > Plug-ins > Plug-in Implementations_.
    
2.  On the Plug-In Implementations page, click the **View** link next to Supplementary Tax Calculation, and then click **Configure**.
    
3.  On the Custom GL Lines: Configuration page, set the values for the following fields:
    
    -   **Transaction Type** - Set the values to **Bill**, **Bill Credit**, **Check**, and **Expense Report**.
        
    -   **Subsidiary** (for OneWorld accounts) - Set the value to the applicable subsidiaries, or check the **All** box below the field.
        
    -   **Accounting Book** (for Multi-Book Accounting) - Set the value to **Primary Accounting Book** only.
        
    
    If you have multiple Custom GL Lines plug-in implementations in your account, you need to configure the Supplementary Tax Calculation plug-in implementation for a unique set of transaction types, subsidiaries, and accounting books.
    
4.  Click **Save**.
    
5.  Go to _Customization > Plug-ins > Manage Plug-ins_.
    
6.  Check the **Supplementary Tax Calculation** box.
    
7.  Click **Save**.
    

Note:

Supplementary Tax Calculation isn't available for Canada and United States. Refer to the [Canada Help Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4198261632.html) and [U.S. Help Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4198378704.html) for details.

### Related Topics

-   [Recording Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822590.html)
-   [Applying Nondeductible Input Tax on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1823395.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
