---
id: "section_N2087711"
type: "section"
title: "Withholding Taxes on Payment Acceptance"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Recording Withholding Taxes on Transactions as a Seller > Withholding Taxes on Payment Acceptance"
parent: "section_N2087219"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087711.html"
anchors: ["procedure_N2087724", "bridgehead_3704211177"]
sha256: "2abe01a7e87cd6c4c69b9a5efa99d681bc6fb24f6451935188307c9a570c06a6"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

#### To record withholding taxes on acceptance of a customer payment: {#procedure_N2087724}

1.  Go to _Transactions > Customers > Accept Customer Payments_.
    
2.  On the Payment form, select a customer that you want to accept payment from.
    
    The Payment page displays a list of all open invoices.
    
3.  Check the boxes in the **Apply** column next to the invoices that the customer payment should be applied to. Or click **Pay All** to apply the customer payment to all the invoices.
    
    Note:
    
    When you accept a payment from a customer, NetSuite calculates and shows the total tax withheld by the customer from the selected invoices in the **WHT Tax Amount** field.
    
4.  Enter payment amounts, net of withholding tax, in the **Payment** column.
    
    Note:
    
    If you want to see the amount of tax withheld by the customer from each invoice, customize the payment sublist on the **Apply** tab to display the withholding tax amount and total amount, including withholding tax for each invoice. See [Displaying the Withholding Tax Amount and Total Amount Columns on the Payment Page](#bridgehead_3704211177).
    
5.  **To apply a partial payment for an invoice**, enter the payment amount (net of withholding tax) in the **Payment** column of the invoice. The system calculates the withholding tax amount (or the gross amount still including the withholding tax).
    
6.  **To apply a discount on a payment**, enter an amount in the **Disc. Taken** column of the invoice. The system recalculates and the amount in the **Payment** column changes to factor in the cash discount.
    
    Note:
    
    Currently cash discounts only affect the final cash payment and aren't included when computing the withholding tax amount.
    
7.  Click **Save**. The withholding tax amounts are automatically posted to the appropriate general ledger accounts.
    
    -   NetSuite creates a credit memo for each invoice paid to record the effect of withholding tax on customer payments. Posting withholding tax amounts might take a few minutes to complete and only works for up to 1000 invoice records at a time. When accepting a payment, keep the number of open invoices to 1000 or fewer for NetSuite to create a credit memo.
        
        Note:
        
        The payment record can't be edited while the posting of withholding tax is ongoing.
        
    -   To see all associated credit records, click the **Withholding Tax** tab. This tab is only available on the parent payment record. The credit records are also associated with the parent payment record.
        
    -   In the More Actions menu, click **GL Impact** to view the GL Impact page for this transaction.
        

## Displaying the Withholding Tax Amount and Total Amount Columns on the Payment Page {#bridgehead_3704211177}

You can customize the payment sublist on the Apply tab of the Payment page to show the withholding tax amount and total amount, including withholding tax for each invoice.

Important:

Users who want to see these columns need to customize the payment sublist in their own account. These columns will only show values in Create and Edit mode. After you complete this step, the columns will appear every time you open the Payment page.

#### To show the Withholding Tax Amount and Total Amount columns:

1.  On the Payment page, go to the **Apply** subtab, and click **Customize**.
    
2.  On the Customize Sublist page, under Additional Columns, select the **Tax Withheld** and **Total Amount** fields.
    
3.  Click **Save**.
    
    The **Tax Withheld** and **Total Amount** columns will now show up in the sublist next to the payment amount.
    
    Note:
    
    If there are more than 100 unpaid bills on the page, you should clear the Apply box next to the bill you want to pay. Check the Apply box again to show the payment amount net of the withholding tax.
    

### Related Topics

-   [Withholding Taxes on Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087402.html)
-   [Withholding Taxes on Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088149.html)
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
