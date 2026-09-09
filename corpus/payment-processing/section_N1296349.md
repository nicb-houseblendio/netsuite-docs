---
id: "section_N1296349"
type: "section"
title: "Customer Deposits"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Deposits"
parent: "preface_4739476790"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html"
anchors: ["section_N1296579"]
sha256: "7f428c81ac0b7a8581549da552ca6386c7f0c97bda75772af167a3b42d381dbc"
---

When a customer makes an advance payment for an order or project, you can record the funds received as a customer deposit. These payments go into your general ledger as a liability until you deliver the goods or services, and they don't affect the customer's accounts receivable balance.

When the order is filled, the deposit is applied against the invoice and the liability is canceled out.

To record customer deposits and apply them to invoices, you must use the Accounts Receivable (A/R) feature. To enable A/R, go to _Setup > Company > Enable Features (Administrator)_, and click the **Accounting** subtab. Check the **A/R** box and click **Save**.

With the A/R feature enabled, the Customer Deposit general ledger account is generated along with the first Customer Deposit record. Even if you do not have a permission to create accounts, you will still be listed in the system notes as the Customer Deposit account creator. The Customer Deposit account tracks each deposit as an Other Current Liability.

Record prepayments from customers by going to _Customers > Accounts Receivable > Record Customer Deposits_. Then, you can track funds the customer has paid until the goods or services are delivered. For more information, see [Recording a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296669.html).

You can view a customer record and click the Financial subtab to see if the customer has any unapplied deposits recorded. The Customer Deposit Balance field displays the total amount of unapplied deposits for the customer.

When you have entered a customer deposit, you can generate a payment receipt for the customer. For more information, see [Payment Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293235.html).

You can apply a deposit against an invoice in one of the following ways:

-   Go to _Customers > Accounts Receivable > Accept Customer Payments > Deposits_ > Deposits.
    
-   View a customer deposit record and click the **Apply** button.
    

NetSuite tracks the date when each deposit is applied to a customer invoice. For more information, see [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html). If you use the Consolidated Payments feature, any deposits made by a customer or its subcustomers can be applied to any of the open invoices in the customer hierarchy. For more information, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).

If needed, you can refund a customer deposit using the customer refund form. For more information, see [Issue Refunds for Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300211.html).

## Customer Deposits Workflow Chart {#section_N1296579}

![Block diagram showing the 3 steps in the Customer Deposits workflow (as listed under Related Topics).](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/customerdeposit.png)

### Related Topics:

-   [Recording a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296669.html)
-   [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html)
-   [Issue Refunds for Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300211.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
