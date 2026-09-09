---
id: "section_N2086435"
type: "section"
title: "Withholding Taxes on Bill Payments"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Applying Withholding Taxes on Transactions as a Buyer > Withholding Taxes on Bill Payments"
parent: "section_N2085924"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086435.html"
anchors: ["procedure_N2086448", "bridgehead_3704166931"]
sha256: "181babb8f8e1b7af4fe778593aebd17bfb207194c65b61db285d369a67d9f55b"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

#### To record withholding tax on bill payments: {#procedure_N2086448}

1.  To pay multiple vendors, go to Transactions > Payables > Pay Bills. To pay a single vendor, go to Transactions > Payables > Pay Single Vendor.
    
2.  On the Bill Payment page, select the bank account you want to use to pay these bills.
    
3.  Select a posting period.
    
4.  The Bill Payment page displays all your open bills. Check the **Apply** box next to the bills you want to pay.
    
    When paying a single vendor, NetSuite calculates and shows the total amount to be withheld from the selected payments.
    
    When paying bills from multiple vendors, NetSuite doesn't show the amount to be withheld but still deducts the appropriate withholding tax on posting of the payments. You can enter a date in the **Start Date** and **End Date** fields to limit the transactions that appear in the list.
    
5.  For each item to be paid, enter the payment amount net of withholding tax.
    
    Note:
    
    When paying a single vendor, if you want to see the amount of tax to be withheld from each bill, you can customize the payment sublist on the **Apply** tab to show the withholding tax amount and total amount, including withholding tax for each bill. See [Displaying the Withholding Tax Amount and Total Amount Columns on the Bill Payment Page](#bridgehead_3704166931).
    
6.  **To apply a partial payment for a bill**, enter the payment amount (net of withholding tax) in the **Payment** column of the bill. The system calculates the withholding tax amount to show the total amount due, including withholding tax.
    
7.  **To apply a discount on a payment**, enter an amount in the **Disc. Taken** column of the bill. The system recalculates, and the amount in the **Payment** column changes to account for the cash discount.
    
    Note:
    
    Currently, cash discounts only affect the final cash payment, and aren't included when computing the withholding tax amount.
    
8.  Click **Save**. When you save the bill payment, NetSuite automatically deducts the withholding tax amounts from the payment.
    
    -   When paying a single vendor, the amount to be withheld is shown in the **WH Tax Amount** field.
        
    -   When paying bills from different vendors, the calculated withholding tax amount isn't shown but is posted after payment processing is completed.
        
    -   Posting of the withholding tax amounts might take a few minutes to complete. NetSuite posts them to the right general ledger accounts and creates a bill credit memo for each bill paid. Take note that NetSuite can only process up to 1000 bill records. If you're paying a vendor, you must only have up to 1000 open bills for NetSuite to create a bill credit memo.
        
        Note:
        
        The payment record can't be edited while the posting of withholding tax is ongoing.
        
    -   To see all associated credit records, click the **Withholding Tax** tab. This tab is only available on the parent payment record. The credit records are also associated with the parent payment record.
        
    -   In the More Actions menu, click **GL Impact** to view the GL Impact page for this transaction.
        

## Displaying the Withholding Tax Amount and Total Amount Columns on the Bill Payment Page {#bridgehead_3704166931}

When paying a single vendor, if you want to see the amount of tax to be withheld from each bill, customize the payment sublist on the Apply tab to show the withholding tax amount and total amount, including withholding tax for each bill.

Important:

Each user who wants to see these columns needs to customize the payment sublist in their own account. After you complete this step, the columns appear every time the Pay Single Vendor page is displayed.

#### To customize the payment sublist of a bill payment to show the Withholding Tax Amount and Total Amount columns:

1.  On the **Apply** subtab, click **Customize**.
    
2.  On Customize Sublist page, under Additional Columns, select the **Tax Withheld** and **Total Amount** fields. Click **Save**.
    
    The **Tax Withheld** and **Total Amount** columns will now show up in the sublist next to the payment amount.
    
    Note:
    
    If there are more than 100 unpaid bills on the page, you should clear the Apply box next to the bill you want to pay, and then check the box again, to show the payment amount net of withholding tax.
    

### Related Topics

-   [Withholding Taxes on Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086130.html)
-   [Withholding Taxes on Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086925.html)
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
