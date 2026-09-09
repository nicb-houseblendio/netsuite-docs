---
id: "section_N2086925"
type: "section"
title: "Withholding Taxes on Checks"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Applying Withholding Taxes on Transactions as a Buyer > Withholding Taxes on Checks"
parent: "section_N2085924"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086925.html"
anchors: ["procedure_N2086938"]
sha256: "a11de8b8231062f6e73a0124e8f825b6156db4c452142e117cd7c77786fb513a"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

#### To apply withholding taxes on a check: {#procedure_N2086938}

1.  Go to _Transactions > Bank > Write Check_.
    
2.  Select an account.
    
3.  Select the payee for this check. If the payee is a vendor from a nexus where withholding tax is used, the system reloads the form to display the withholding tax objects.
    
4.  Enter expenses or items for this check.
    
    1.  **To apply withholding tax to the total of the bill**, do the following:
        
        -   On the **Withholding Tax** tab under Expenses and Items, set the **Applies To** field to **Total Amount**.
            
        -   In the **Tax Code** field, select the appropriate withholding tax code. You can also select a tax code in the **Tax Code** column of the Expenses and Items list.
            
    2.  **To apply withholding tax to individual items**, do the following:
        
        -   On the **Withholding Tax** tab under Expenses and Items, set the **Applies To** field to **Individual Line Items**.
            
        -   On the **Expenses and Items** subtab, check the **Apply WH Tax?** box for each line item that you want to apply withholding tax to. In the **Withholding Tax Code** column, select the appropriate withholding tax code that will be applied to the item (if not already selected).
            
5.  After entering line items, review the information about the **Withholding Tax** tab under Expenses and Items to make sure the values are correct in the **Base Amount** and **Tax Amount** fields.
    
6.  Enter other details required for this transaction.
    
7.  Click **Save**. The withholding tax amounts are automatically posted to the appropriate general ledger accounts. In the More Actions menu, click **GL Impact** to view the GL Impact page for this transaction.
    

### Related Topics

-   [Withholding Taxes on Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086130.html)
-   [Withholding Taxes on Bill Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086435.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
