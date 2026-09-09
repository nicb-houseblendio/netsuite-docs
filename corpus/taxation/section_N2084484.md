---
id: "section_N2084484"
type: "section"
title: "Setting Up Withholding Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Setting Up Withholding Tax > Setting Up Withholding Tax Codes"
parent: "section_N2079716"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html"
anchors: ["bridgehead_N2084496", "procedure_N2084506", "bridgehead_N2084806", "procedure_N2084820", "bridgehead_N2084860", "procedure_N2084874", "procedure_N2084918"]
sha256: "4c49d441de824814ec7d3deeaa5e3f7693d2b9b310cc3a5a10349f2c7be4b039"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

Tax codes are used to calculate tax on transactions.

Note:

The Withholding Tax SuiteApp supports up to 400 withholding tax codes per nexus. If you go over this limit, you'll get an error on your transaction. To fix it, inactivate all unused withholding tax codes. For information about inactivating tax codes, see [Inactivating or Deleting Withholding Tax Codes](#bridgehead_N2084860).

## Creating Withholding Tax Codes {#bridgehead_N2084496}

#### To create a withholding tax code: {#procedure_N2084506}

1.  Setup > Withholding Tax > Tax Codes.
    
2.  Click **New**.
    
3.  Click the nexus that you're creating a tax code for.
    
4.  Provide values for the following fields:
    
    1.  **Tax Code** - Enter a name for the tax code.
        
    2.  **Description** - Enter a description for the tax code.
        
    3.  **Rate** - Enter the appropriate withholding tax rate as a percentage. Example: 8%. This percentage will be calculated when you select this withholding tax code in bills or payments.
        
    4.  **Effective From** - Enter the first date this withholding tax code is effective.
        
    5.  **Valid Until** - Enter the latest date this withholding tax code is effective.
        
    6.  **Percentage of Base** - If the withholding tax should be applied to a percentage of the tax base, specify the percentage.
        
    7.  **Tax Agency** - Select the government agency this tax is paid to. You can set up a vendor as a tax agency by selecting Tax Agency in the Category field of the vendor record.
        
    8.  **Withholding Tax Type** - Select the tax type of this withholding tax code.
        
    9.  **Available On** - Select the type of transactions this withholding tax code can be applied to.
        
    10.  **Subsidiaries** - Select the subsidiaries that this withholding tax code should be available in. In the Subsidiaries field, colons separate Parents (on the left) from their Children (on the right). To select multiple subsidiaries, hold down the Ctrl key on your keyboard while clicking each subsidiary.
         
    11.  **Include Children** - Check this box to make this tax code available to children of the selected subsidiaries.
         
5.  Click **Save**. The next step to set up tax groups. See [Setting Up Withholding Tax Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085135.html).
    

## Editing Withholding Tax Codes {#bridgehead_N2084806}

You can change a tax code anytime. For example, if a tax rate changes, manually update the Rate field on the tax code record.

#### To edit an existing withholding tax code: {#procedure_N2084820}

1.  Go to Setup > Withholding Tax > Tax Codes.
    
2.  Click **Edit** next to the code you want to update.
    
3.  On the Tax Code page, make necessary changes.
    
4.  Click **Save**.
    

## Inactivating or Deleting Withholding Tax Codes {#bridgehead_N2084860}

If you don't use a tax code and don't want it displayed in your lists, you can inactivate or delete it.

#### To inactivate a withholding tax code: {#procedure_N2084874}

1.  Go to Setup > Withholding Tax > Tax Codes.
    
2.  Click **Edit** next to the code you want to inactivate.
    
3.  On the Tax Code page, check the **Inactive** box.
    
4.  Click **Save**.
    

After you save, this withholding tax code can't be selected in transactions, reports, or records.

#### To delete a withholding tax code: {#procedure_N2084918}

1.  Go to Setup > Withholding Tax > Tax Codes.
    
2.  Click **Edit** next to the withholding tax code record you want to delete.
    
3.  Click **Delete**.
    
4.  Click **OK** to confirm deletion of the withholding tax code record.
    

That tax code won't appear in the Withholding Tax Codes list and can't be selected for transactions, reports, or records.

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Setting Up Withholding Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html)
-   [Setting Up Withholding Tax Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html)
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
