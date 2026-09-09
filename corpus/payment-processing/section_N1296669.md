---
id: "section_N1296669"
type: "section"
title: "Recording a Customer Deposit"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Deposits > Recording a Customer Deposit"
parent: "section_N1296349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296669.html"
anchors: ["bridgehead_N1296730", "procedure_N1296740", "bridgehead_1500286017", "bridgehead_N1296976"]
sha256: "6abb0398c6f8ae65666dbca2e0afc671ee59d554f1410329579dfb057c748ecd"
---

Record a customer deposit when a customer makes an advance payment for an order or project. A customer deposit record tracks funds the customer has paid until the goods or services are delivered.

These payments are recorded in your general ledger as a liability until the goods or services are delivered and don't affect the customer's accounts receivable balance.

There are two ways to record a customer deposit:

-   [Creating a Deposit on the Customer Deposit Page](#bridgehead_N1296730)
    
-   [Customer Deposit Status](#bridgehead_1500286017)
    
-   [Creating a Deposit From the Sales Order](#bridgehead_N1296976)
    

## Creating a Deposit on the Customer Deposit Page {#bridgehead_N1296730}

#### To record a customer deposit: {#procedure_N1296740}

1.  Go to _Customers > Accounts Receivable > Record Customer Deposits_.
    
2.  Under Primary Information:
    
    1.  Select the customer making the payment. If you are using projects, select the appropriate project name.
        
        Important:
        
        After you save this form, the selection in this field cannot be changed.
        
    2.  In the **Payment Amount** field, enter the currency amount the customer is paying.
        
    3.  Select the account to deposit the funds to:
        
        -   If you select a bank account in the **Account** field, the funds post to that account directly.
            
        -   If you select **Undep. Funds**, the funds post to the Undeposited Funds account and appear in your deposit list.
            
    4.  Under Classification, select a department, class, and location you want to associate with this order.
        
        Note:
        
        If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        
    5.  On the **Payment Method** subtab, enter the payment information for this deposit.
        
        For more information, see [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html).
        
3.  On the **Relationships** subtab, the primary contact for the customer is selected automatically. To edit information for this contact, click the contact's name.
    
4.  On the **Communication** subtab, attach events, tasks, and phone calls for this transaction. For more information, see [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html).
    
5.  Click **Save**.
    

When you record a customer deposit, you can generate a payment receipt for the customer. For more information, see [Payment Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293235.html).

As soon as an order is completed, you can apply a deposit to the invoice. For more information, see [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html).

## Customer Deposit Status {#bridgehead_1500286017}

When you save a customer deposit, one of the following status will be applied to it:

-   **Unapproved payment** - this status means that the deposit has not been successful. Possible reasons for this status include insufficient funds in the account, or the card used for the payment is reported lost or stolen.
    
-   **Not deposited** - this is a successful status, the deposit is being processed but the funds have not yet been deposited.
    
-   **Deposited** - this status is applied when the funds have been deposited.
    

The status of the deposit is visible at the top of the Customer Deposit record next to the deposit number.

![Location of the deposit status on the Customer Deposit record.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/SA_CustomerDepositStatus.png)

## Creating a Deposit From the Sales Order {#bridgehead_N1296976}

You can accept deposits directly from the sales orders they are to be applied to.

Sales orders created with a Sales Order-Invoice transaction form (or orders that use other forms but do not have terms or a payment method specified) have a Create Deposit button that enables you to record a deposit immediately upon saving a new sales order.

![Example of a sales order with location of the Create Deposit button highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/CustomerDeposit_CreateDepositButton.png)

Deposits created this way are linked to the originating sales order and cannot be applied to other invoices. A read-only Sales Order field on the deposit shows the linked transaction.

When you invoice this originating sales order, the reserved deposit is automatically applied.

Note:

You can only use this button for sales orders that have not been billed.

You can apply multiple deposits to a single order. If the deposit total exceeds the order amount, the excess deposit amount is not linked to the original order and can be applied to any invoice.

### Related Topics:

-   [Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html)
-   [Customer Deposits Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html#section_N1296579)
-   [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
