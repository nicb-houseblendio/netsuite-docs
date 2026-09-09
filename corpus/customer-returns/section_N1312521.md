---
id: "section_N1312521"
type: "section"
title: "Applying a Customer Credit Memo"
branch: "customer-returns"
category: "order-management"
breadcrumb: "Order Management > Customer Returns > Customer Credits and Refunds > Customer Credits > Applying a Customer Credit Memo"
parent: "section_4417991103"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1312521.html"
anchors: ["procedure_N1312599", "procedure_N1312699", "procedure_N1312897"]
sha256: "6252bbbb3258c2c6e79a7cc5f0614afee115acec9d82e3999026e36d2af9abf0"
---

You can apply a credit memo to decrease the amount a customer owes you. When you apply a credit memo against an open invoice or cash sale, the amount of the credit is deducted from the total amount due.

Note:

If you create a standalone credit memo and apply it to one or more invoice lines, in a transaction saved search the CreatedFrom field references that invoice. However, the credit memo transaction CreatedFrom field is blank because it wasn't created directly from an invoice.

You can apply a credit memo in the following ways:

-   [Apply a Credit Memo on the Credit Transaction](#procedure_N1312599)
    
-   [Apply a Credit Memo on a Customer Payment](#procedure_N1312699)
    
-   [Apply a Credit Memo on an Open Invoice](#procedure_N1312897)
    

#### Apply a Credit Memo on the Credit Transaction {#procedure_N1312599}

1.  Go to _Transactions > Customers > Issue Credit Memos > List (Administrator)_.
    
2.  Click **Edit** next to the memo you want to apply.
    
3.  On the **Items** subtab, check the **Auto Apply** box next to the Unapplied field if you want NetSuite to apply the credit amount to the oldest invoices or cash sales due.
    
4.  Click the **Apply** subtab to apply the credit toward a specific invoice or cash sale.
    
5.  Check the **Apply** box next to the invoices or cash sales you want the credit applied to.
    
    If you use the **Multiple Currencies** feature, only invoices or cash sales in the currency of the memo are shown on the **Apply** subtab.
    
    For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    
6.  Click **Save**.
    

Now, when you include the credited invoice or cash sale on a customer payment, the balance due reflects the credit amount.

You can also apply credit memos when you enter a customer payment.

When you enter a customer payment, you can also apply open credit memos for that customer. This is useful when a customer remits a payment amount that is based on both invoices and credits to their account.

For example, your customer ACME Inc. makes a monthly payment based on their statement. This month, their statement shows invoice #888 for $100 and credit memo #999 issued for $25. ACME Inc. remits a $75 payment. You can create one transaction that applies both the $25 credit memo and the $75 payment to invoice #888.

#### Apply a Credit Memo on a Customer Payment {#procedure_N1312699}

1.  Go to _Transactions > Customers > Accept Customer Payments > List (Administrator)_.
    
2.  Click Edit next to the payment where you want to apply the credit.
    
    To create a new payment click New Transaction.
    
3.  Fill in the necessary information for this payment. For more information, see [Applying a Payment on the Customer Payment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288824.html).
    
4.  On the **Apply** subtab, click the **Credits** subtab.
    
    1.  Check the box in the **Apply** column next to each credit memo you want to apply.
        
    2.  Clear the box in the **Apply** column next to each credit memo you are not applying.
        
    3.  Click **Mark All** to apply all existing credits.
        
    
    Note:
    
    If you check the Auto Apply box, NetSuite applies this credit amount to the oldest outstanding invoices, but does not auto-apply existing credits or deposits.
    
5.  Click the **Invoices** subtab to view the invoices being credited.
    
    You can change the bills that credits are applied to by:
    
    1.  checking the box in the **Apply** column next to each invoice you are applying credit to.
        
    2.  clearing the box in the **Apply** column next to each invoice you are not applying credit to.
        
    
    As credits are applied, you can see the amounts change in the To Apply, Applied, and Unapplied amounts in the header.
    
6.  Click **Save**.
    

The following procedure explains how to create a new credit memo and apply it directly from an invoice. To apply an **existing** credit memo to an open invoice, first you must click Accept Payment on the invoice page, and then follow the steps in [Apply a Credit Memo on a Customer Payment](#procedure_N1312699).

Note:

To apply a credit memo on an open invoice, the account fields on both the credit memo and the invoice need to have the same value.

#### Apply a Credit Memo on an Open Invoice {#procedure_N1312897}

1.  Go to _Transactions > Sales > Create Invoices > List (Administrator)_.
    
2.  Click **View** next to the invoice you want to credit.
    
3.  Click **Credit**.
    
4.  Fill in the necessary information for the **Credit Memo**. For details, read [Issuing a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311510.html).
    

After you have applied a credit memo, you can review how it was applied in the following ways:

-   **From a Credit** - Go to _Transactions > Customers > Issue Credit Memos > List (Administrator)_ > List. On the Credit memos page, click View next to the credit. The Apply subtab on the credit memo shows which bills were credited.
    
-   **From a Payment** - Go to _Transactions > Customers > Accept Customer Payments > List (Administrator)_. On the Payments page, click View next to the payment. The Credits Applied subtab on the payment shows which credits were applied.
    

### Related Topics:

-   [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html)
-   [Issuing a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311510.html)
-   [Crediting an Authorized Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1312244.html)
-   [Printing a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313142.html)
-   [Refunding an Authorized Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313511.html)
-   [Refunding an Open Balance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313840.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
