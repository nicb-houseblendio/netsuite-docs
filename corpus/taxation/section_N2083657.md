---
id: "section_N2083657"
type: "section"
title: "Setting Up Withholding Tax Preferences"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Setting Up Withholding Tax > Setting Up Withholding Tax Preferences"
parent: "section_N2079716"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html"
anchors: ["procedure_N2083695"]
sha256: "477e92926da4b0678ad0801da03cfdd26d2a41be0ef386119c799baa55117e2b"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

Withholding tax preferences enable you to set rules for the following:

-   Make withholding tax codes available on purchases, sales, or both
    
-   Specify whether to post withholding tax at the time of payment or at the time of invoice
    
-   Specifying whether tax codes apply to each line item in a transaction, or to the sum of the transaction
    

#### To set up withholding tax preferences for each nexus: {#procedure_N2083695}

1.  Go to Setup > Withholding Tax > Set Up Withholding Tax.
    
2.  Provide values for the following fields:
    
    1.  **Nexus** - Select the nexus that this withholding tax setup applies to.
        
    2.  **Enable Tax Lookup on Transactions** - Check this box to automatically select the default withholding tax code of the item or entity on transactions. You can change this on a transaction.
        
    3.  **Auto Apply Withholding Tax** - Check this box to automatically select Yes in the **Apply WH Tax?** column per line on transactions. You can change this on a transaction.
        
        Note:
        
        You can include or exclude certain lines of a transaction when calculating the withholding tax base amount.
        
        NetSuite doesn't apply withholding tax to the following line items:
        
        -   Description item type
            
        -   Subtotal item type
            
        -   Group item type
            
        -   End of Group line (the amount of the group item)
            
    4.  **Available on Purchases** - Check this box to make withholding tax codes available on purchase transaction forms such as Check payments, Purchase Orders, Bills, and Bill payments.
        
        1.  **Disable Withholding Tax in Purchase Orders** - Check this box to disable withholding tax in purchase orders.
            
            Note:
            
            When withholding tax is disabled in POs, the **Apply WH Tax?** column isn't automatically set to **Yes** on a bill created from a PO, even if Auto Apply Withholding Tax was enabled in the tax setup. You can still check the **Apply WH Tax?** box for each line item you want to apply withholding tax to.
            
        2.  **Tax Point** - Set when to record withholding tax as a buyer. You can:
            
            -   Select **On Accrual** to post withholding tax when you create the bill.
                
            -   Select **On Payment** to post withholding tax at the time of payment (write check/bill payment).
                
            
            The withholding tax amounts are posted to the general ledger accounts automatically. To view the GL Impact page for the transaction on a transaction record, go to the More Actions menu and click **GL Impact**.
            
        3.  **Applies To** - Specify whether the selection of withholding tax codes apply to the entire sum of the transaction, or should be defined individually per line item. You can change this on a transaction.
            
    5.  **Available on Sales** - Check this box to make withholding tax codes available on sales transaction forms such as Cash Sales, Sales Orders, Invoices, and Invoice Payments.
        
        1.  **Disable Withholding Tax in Sales Orders** - Check this box to disable withholding tax in sales orders.
            
            Note:
            
            When withholding tax is disabled in SOs, the **Apply WH Tax?** column isn't automatically set to **Yes** on an invoice created from an SO, even if Auto Apply Withholding Tax was enabled in the tax setup. You can check the **Apply WH Tax?** box for each line item you want to apply withholding tax to.
            
        2.  **Tax Point** - Set when to record withholding tax as a seller. You can:
            
            -   Select **On Accrual** to post withholding tax when you create the invoice.
                
            -   Select **On Payment** to post withholding tax at the time of payment (cash sale/payment acceptance).
                
            
            The withholding tax amounts are posted to the general ledger accounts automatically. To view the GL Impact page for the transaction on a transaction record, go to the More Actions menu and click **GL Impact**.
            
            Note:
            
            Header discounts aren't supported when withholding tax is set to record on accrual for sales transactions. To calculate withholding tax correctly for invoices with header discounts, set the tax point to **On Payment**.
            
        3.  **Applies To** - Specify whether withholding tax codes apply to the entire sum of the transaction, or should be defined individually per line item. You can change this on a transaction.
            
3.  Click **Save**. The next step is to set up withholding tax types. For more information, see [Setting Up Withholding Tax Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html).
    

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Setting Up Withholding Tax Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html)
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
