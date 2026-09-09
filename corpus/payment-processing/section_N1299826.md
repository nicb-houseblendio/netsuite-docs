---
id: "section_N1299826"
type: "section"
title: "Applying a Customer Deposit"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Deposits > Applying a Customer Deposit"
parent: "section_N1296349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html"
anchors: ["procedure_N1299849", "procedure_N1299971"]
sha256: "6d8bbface851985ed4baa9b1d210c607e3cd3f2eefa90158b3a80c832ef4c514"
---

You can apply a customer deposit against an invoice when the order is complete. Deposits are applied by creating a Deposit Application transaction.

Deposits can be applied against an invoice either from a customer deposit record or on a customer payment form.

#### Apply a deposit from a customer deposit record: {#procedure_N1299849}

1.  Go to _Customers > Accounts Receivable > Record Customer Deposits > List_.
    
2.  Click **View** next to the deposit you want to apply.
    
3.  On the Customer Deposit page, click **Apply**.
    
    The Deposit Application form opens with the customer information and To Apply amount auto-filled.
    
    A list of open invoices for that customer appears. If you use the **Multiple Currencies** feature, these invoices are filtered to show only those in the same currency as the deposit. For more information, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    
4.  Verify or enter the date for this Deposit Application.
    
5.  Select a posting period for this transaction.
    
6.  The **Application Of** field shows a link to the customer deposit being applied.
    
7.  The **Deposit Date** field shows the date the pre-payment was originally deposited.
    
8.  Enter a memo to identify this application transaction.
    
9.  Select a department , class or location as necessary.
    
10.  Check the **Apply** box next to the invoices you want to apply the deposit against.
     
     You can apply up to the total amount of the deposit.
     
11.  Click **Save**.
     

Now, the customer deposit is applied against the invoices you selected and their balance due is decreased by the appropriate amount.

#### Apply a deposit on a customer payment form: {#procedure_N1299971}

1.  Go to _Customers > Accounts Receivable > Accept Customer Payments > List_.
    
2.  Select the customer or project.
    
    If you use the **Consolidated Payments** feature, choose a top-level customer to apply any deposit in the customer-subcustomer hierarchy to any of the open invoices in the hierarchy. For more information, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).
    
3.  If you use the **Multiple Currencies** feature, select the currency of the invoices you want to apply the deposit to. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    
    Selecting a currency filters the list of invoices, credits, and deposits.
    
4.  Click the **Apply** subtab.
    
    A list of deposits, or pre-payments, appears on the **Deposits** subtab.
    
5.  Click the **Deposits** subtab to apply a customer pre-payment to an invoice.
    
    -   Check the box in the **Apply** column next to each customer deposit you want to apply.
        
    -   Clear the box in the **Apply** column next to each customer deposit you are not applying.
        
    -   Click **Mark All** to apply all existing customer deposits.
        
6.  Click the **Invoices** subtab.
    
    You can control the bills this deposit is applied to by:
    
    -   checking the box in the **Apply** column next to each invoice you want to record a payment on.
        
    -   clearing the box in the **Apply** column next to each invoice you are not recording a payment on.
        
    
    As payments are applied, you can see the amounts change in the **To Apply**, **Applied**, and **Unapplied** fields in the header.
    
7.  Click **Save**.
    
    The customer deposit is now applied.
    

NetSuite tracks the dates that deposits are applied to customer invoices.

To track a deposit application, go to the _Customers > Accounts Receivable > Record Customer Deposits > List_ . Click View next to the customer deposit to open the record. On the deposit, click the Applied To subtab to view the dates the deposit was applied and amounts applied.

### Related Topics:

-   [Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html)
-   [Customer Deposits Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html#section_N1296579)
-   [Recording a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296669.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
