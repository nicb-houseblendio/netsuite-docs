---
id: "section_N2085135"
type: "section"
title: "Setting Up Withholding Tax Groups"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Setting Up Withholding Tax > Setting Up Withholding Tax Groups"
parent: "section_N2079716"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085135.html"
anchors: ["procedure_N2085175"]
sha256: "47342015d06aa310f7cc8bfe852df50025965ede61d38cc0ed1c3f667fc0778c"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

Tax codes you can apply to a transaction can be combined to create a Withholding Tax Group. You can create a group of tax codes from different withholding tax types if they have the same applicable withholding tax base and tax nexus. For example, net amount tax codes can be grouped together from the same nexus, even if they have different tax types. The Withholding Tax Base field shows the tax base for the tax group.

#### To create a withholding tax group: {#procedure_N2085175}

1.  Setup > Withholding Tax > Tax Groups.
    
2.  Click **New**.
    
3.  Click the nexus that you're creating a tax group for.
    
4.  Provide values for the following fields:
    
    1.  **Name** - Enter a name for the tax group. You select this name on transactions.
        
    2.  **Description** - Enter a description for the tax group.
        
    3.  **Rate** - The system automatically displays the sum of the rates of the tax codes in this tax group. This sum takes into account the percentage base that applies to the tax codes.
        
    4.  **Subsidiaries** - Select the subsidiaries that this withholding tax group should be available to. In the **Subsidiaries** field, colons separate parents (on the left) from their children (on the right). To select multiple subsidiaries, hold down the Ctrl key on your keyboard while clicking each subsidiary.
        
    5.  **Include Children** - Check this box to make this tax group available to children of the selected subsidiaries.
        
    6.  **Withholding Tax Type** - Select the withholding tax type of the tax group you're creating. You can create a new tax type at Setup > Withholding Tax > Tax Types > New.
        
    7.  **Available On** - Select which transaction types the withholding tax group applies to.
        
5.  Add the tax codes that you want to include in this tax group.
    
    1.  In the **Tax Code** column, select a tax code. The list only shows tax codes for this nexus with the same withholding tax base and nexus.
        
    2.  In the **Basis** column, enter the basis for the selected tax code. The default value is 100, which represents the full rate. For example, with a 10% tax rate and a basis of 100, 10% is added to the tax group rate. If the basis is 50, only 5% is added.
        
    3.  To add more tax codes, click **Add** and repeat the steps.
        
6.  Click **Save**. The next step is to set default withholding tax codes on item, customer, and vendor records. For more information, see [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html).
    
    Note:
    
    If you edit a tax code that's part of a group, the system will warn you that changes you make will also affect the behavior of the tax group it belongs to.
    

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Setting Up Withholding Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html)
-   [Setting Up Withholding Tax Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html)
-   [Setting Up Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
