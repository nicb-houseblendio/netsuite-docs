---
id: "section_N2084141"
type: "section"
title: "Setting Up Withholding Tax Types"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Setting Up Withholding Tax > Setting Up Withholding Tax Types"
parent: "section_N2079716"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html"
anchors: ["procedure_N2084153"]
sha256: "cb341c609bf83ffa0aa1efd421af6230687b109305189737e812706dc6b7bfc0"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

A withholding tax type determines where withholding tax is tracked in the chart of accounts. You need to specify the tax control accounts where NetSuite should post collected or paid tax. You also need to set the tax type's tax base. The tax base determines if withholding tax should be applied to the line item net amount, gross amount, or the tax amount (VAT).

#### To create a withholding tax type for a nexus: {#procedure_N2084153}

1.  Go to Setup > Withholding Tax > Tax Types.
    
2.  Click **New**.
    
3.  Provide values for the following fields:
    
    1.  **Name** - Enter a name for this withholding tax type.
        
    2.  **Description** - Enter a description for the withholding tax type.
        
    3.  **Nexus** - Select the nexus that this withholding tax type applies to.
        
    4.  **Withholding Tax Base** - Select the tax base. Specify if withholding tax applies to the line item net amount, gross amount, or tax amount (VAT/GST or sales tax).
        
        Warning:
        
        The Pay Tax Liability functionality in NetSuite can't pick up withholding tax amounts posted to an account that isn't a tax control account. The Tax Account field on the Tax Liability Check only shows tax control accounts you created at Setup > Accounting > Tax Control Accounts. For more information, see [Creating a Tax Control Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812423.html).
        
    5.  **Liability/Purchase Tax Account**\- Select the account where NetSuite posts tax withheld on purchase transactions.
        
    6.  **Asset/Sales Tax Account**\- Select the account where NetSuite posts tax withheld on sales transactions.
        
4.  Click **Save**. The next step is to set up withholding tax codes. See [Setting Up Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html).
    

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Setting Up Withholding Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html)
-   [Setting Up Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html)
-   [Setting Up Withholding Tax Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085135.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
