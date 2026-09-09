---
id: "section_N2088149"
type: "section"
title: "Withholding Taxes on Cash Sales"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Recording Withholding Taxes on Transactions as a Seller > Withholding Taxes on Cash Sales"
parent: "section_N2087219"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088149.html"
anchors: ["procedure_N2088162"]
sha256: "051d5ecc0d9b053ccdbb86a58ae4d533b5921780e50fb786b6b32b8d2261f970"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

#### To record withholding taxes on a cash sale: {#procedure_N2088162}

1.  Go to _Transactions > Sales > Enter Cash Sales_.
    
2.  Select the customer for this cash sale. If the customer is from a nexus where withholding tax is used, the system reloads the form to display the withholding tax objects.
    
3.  Enter line items.
    
    1.  **To apply withholding tax to the total of the cash sale**, do the following:
        
        -   On the **Withholding Tax** tab under Items, set the **Applies To** field to **Total Amount**.
            
        -   In the **Tax Code** field, select the appropriate withholding tax code. You can also select a tax code in the **Tax Code** column of the Items list.
            
    2.  **To apply withholding tax to individual items**, do the following:
        
        -   On the **Withholding Tax** tab under Items, set the **Applies To** field to **Individual Line Items**.
            
        -   On the **Items** subtab, check the **Apply WH Tax?** box for each line item that you want to apply withholding tax to. In the **Withholding Tax Code** column, select the appropriate withholding tax code that will be applied to the item (if not already selected).
            
    3.  **To apply withholding tax to transaction discounts**, the withholding tax point must be set to **On Payment**. Withholding tax won't apply to transaction discounts when the withholding tax point is set to **On Accrual**. The tax point is the point in time when withholding tax is recorded. For more information about setting up the tax point, see [Setting Up Withholding Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html).
        
4.  After entering line items, review the information about the **Withholding Tax** tab under Expenses and Items to make sure the values are correct in the **Base Amount** and **Tax Amount** fields.
    
5.  Enter other details required for this transaction.
    
6.  Click **Save**. The withholding tax amounts are automatically posted to the appropriate general ledger accounts. In the More Actions menu, click **GL Impact** to view the GL Impact page for this transaction.
    

### Related Topics

-   [Withholding Taxes on Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087402.html)
-   [Withholding Taxes on Payment Acceptance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087711.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
