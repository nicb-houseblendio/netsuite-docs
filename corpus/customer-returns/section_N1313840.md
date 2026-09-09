---
id: "section_N1313840"
type: "section"
title: "Refunding an Open Balance"
branch: "customer-returns"
category: "order-management"
breadcrumb: "Order Management > Customer Returns > Customer Credits and Refunds > Customer Refunds > Refunding an Open Balance"
parent: "section_4417991286"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313840.html"
anchors: ["procedure_N1313871"]
sha256: "0d5bafdcdb1f239b097e35b6d09c3ed7d43b953101647f56358c44f93bdd1104"
---

Refunding an open balance refund gives money back to a customer who has overpaid or is due a refund. In NetSuite, you can pay a customer refund by issuing a check or by crediting a customer's credit card account.

For example, a customer sends you a check to pay an invoice. You apply a discount to this invoice while entering the payment. The difference between the discounted total and the payment is an unapplied credit to the customer's account.

This customer prefers to receive money back rather than having a credit applied to future invoices. You need to issue a customer refund to reimburse this customer.

#### To refund an open balance: {#procedure_N1313871}

1.  Go to _Transactions > Customers > Issue Customer Refund (Administrator)_.
    
2.  Under Primary Information:
    
    1.  Select the customer whose balance you are refunding.
        
        The current customer balance is shown in the **Balance** field.
        
        If the customer has a negative balance, the transactions responsible for that balance appear on the **Credits** subtab.
        
    2.  In the **Account** field, select the bank account you are using for this refund.
        
    3.  Check the **To Be Printed** box if you want to print a check for this refund.
        
        If you are refunding this open balance with a check, the next consecutive check number appears.
        
    4.  If you use the **Multi-Currency Customers** feature, select the currency of the credits or deposits you want to refund. The currency selected in the **Currency** field filters the list of credits and deposits on the **Apply** subtab.
        
        If you do not use this feature, the currency for this customer shows in the **Currency** field.
        
        For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
        
        The current exchange rate for this currency is shown in the **Exchange Rate** field. You can edit the exchange rate for this transaction only, or you can update the currency record with the exchange rate you enter here.
        
    5.  The **Refund Amount** field shows the total amount for this refund.
        
    6.  In the **Date** field, enter the date for this refund.
        
    7.  In the **Posting Period** field, select the period this transaction should post in.
        
    8.  Enter an optional memo to describe this refund. For example, you may want to include the original transaction number on the refund.
        
3.  Under Classification, select the department, class, or location you want to apply to this transaction.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
4.  Click the **Apply** subtab, and on the **Credits** subtab, check the box in the **Apply** column next to each transaction that caused the overpayment you are refunding.
    
5.  Click the **Payee Address** subtab, and verify your customer's address. You can select another address if available, or create a custom address for the particular Customer Refund.
    
6.  Enter the refund method details:
    
    1.  Click the **Refund Method** subtab.
        
    2.  In the **Refund Method** field, select the customer's original payment method.
        
        You must issue the refund in the same form of payment.
        
    3.  If you are crediting the customer's credit card account, enter the credit card information.
        
    4.  If you have a NetSuite enabled merchant account, the check the **Process Credit Card** box to refund the customer's credit card when you save this transaction.
        
    5.  If you do not have a NetSuite enable merchant account, process the refund then check the **Credit Card Approved** box.
        
7.  When you have finished, click **Save**.
    

If you refunded your customer in the form of a check and checked the To Be Printed box, go to _Transactions > Management > Print Checks and Forms (Administrator)_ to print it.

Note:

For details about Refunding a Credit Card with Verisign, please read [FAQ: Accounting & ERP](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3906699.html).

### Related Topics:

-   [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html)
-   [Issuing a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311510.html)
-   [Crediting an Authorized Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1312244.html)
-   [Applying a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1312521.html)
-   [Printing a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313142.html)
-   [Refunding an Authorized Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313511.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
