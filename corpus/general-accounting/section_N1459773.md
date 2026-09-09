---
id: "section_N1459773"
type: "section"
title: "Sales Transaction GL Impact"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > General Ledger Impact of Transactions > Sales Transaction GL Impact"
parent: "chapter_N1459499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459773.html"
anchors: ["bridgehead_N1459793", "bridgehead_N1459817", "bridgehead_N1459997", "bridgehead_N1460166", "bridgehead_N1460335"]
sha256: "758facbf169314ba5077329bde37e36a9abe85390615aa4e92ffb38ccdeb5e8e"
---

Sales transactions are entered to process sales you make and can affect your general ledger. These transactions are used to record and fulfill orders as well as bill customers for orders they have received. As sales transactions are entered, NetSuite records the value of items shipped to customers and the prices charged for them.

## Sales Orders {#bridgehead_N1459793}

Entering sales orders enables you to track the items you need to fulfill and ship to customers. Sales orders, however, are non-posting transactions. They **don't** post an amount to your ledger accounts.

Enter sales orders at _Transactions > Sales > Enter Sales Orders_.

After you fulfill a sales order, the costs and asset values of the items post to your ledger.

## Order Fulfillments {#bridgehead_N1459817}

Fulfilling a sales order ships items to a customer to complete a sale. When you fulfill an order, you pull the items from inventory, package them, and send them to your customer.

After you physically fulfill an order, record an item fulfillment in NetSuite to specify which parts of an order you fulfilled. For example, Maple Street School buys copy paper from you to use in their office. Yesterday, they placed an order for three cases of paper. This morning, you fulfilled the order by getting three cases out of inventory, boxing them, and delivering them to the school. Now you need to record the fulfillment in NetSuite.

When you record a fulfillment, it posts to the journal accounts affected by the fulfillment. Because you're removing items of value from your inventory, fulfilling items lowers the total value of your assets on hand. That is why a fulfillment posts a decrease to an asset account.

The amount of the decrease that posts is based on your cost for the item. For example, if you paid $10 for each of the three cases, the value of your assets on hand decreases by $30. This posts as a decrease in the Inventory Asset account. Fulfilling items also increases the total amount you have spent on items sold, which is tracked in the Cost of Goods Sold (COGS) account. You paid $10 for each of the three cases, so this posts as a $30 increase to your COGS account.

These journal lines are posted by this fulfillment:

| Account | Debit | Credit |
| --- | --- | --- |
| Cost of Goods Sold (COGS) | $30 |  |
| Inventory Asset |  | $30 |

Record your item fulfillments at _Transactions > Sales > Fulfill Orders_.

After an order is fulfilled, bill the customer that received the order. Customers can be billed using cash sales, invoices, or statement charges.

## Cash Sales {#bridgehead_N1459997}

Cash sales should be used to bill customers only if you receive assured payment at the time of the sale in the form of credit card, check, or cash. If you provide terms for your customers and let them pay within a certain period, issue invoices and track how much each customer owes you. For example, you enter a cash sale for three cases of copy paper at $25 each. The total of $75 is paid upon receipt in cash. When you record a cash sale, the cash sale posts to the journal accounts affected by the sale. Accepting the cash from your customer increases the total amount of money you have yet to deposit in the bank. The cash sale posts this as $75 added to the Undeposited Funds account. Accepting the cash from your customer also increases the total amount of funds you have received as income. The cash sale posts this as $75 added to the Sales Income account.

These journal lines are posted by this cash sale:

| Account | Debit | Credit |
| --- | --- | --- |
| Undeposited Funds | $75 |  |
| Sales Income |  | $75 |

Record cash sales at _Transactions > Sales > Enter Cash Sales_.

## Invoices {#bridgehead_N1460166}

Invoices record income you expect to receive in the future for goods or services that you have provided. For example, you enter an invoice for three cases of copy paper at $25 each, totaling $75 due. When you record an invoice, it posts to the journal accounts affected by the invoice. The invoice increases the total amount of funds you need to collect as payments from customers. The invoice posts this as $75 added to the Accounts Receivable account. The invoice also increases the total amount of funds you have received as income. The invoice posts this as $75 added to the total amount in the Sales Income account.

These journal lines are posted by this invoice:

| Account | Debit | Credit |
| --- | --- | --- |
| Accounts Receivable (AR) | $75 |  |
| Sales Income |  | $75 |

Invoice your orders at _Transactions > Sales > Bill Sales Orders_ or at _Transactions > Sales > Create Invoices_.

## Statement Charges {#bridgehead_N1460335}

Statement charges are similar to invoices because they track payments you expect from customers. Use statement charges instead of invoices when you want to enter several charges that accumulate before you send a billing statement to the customer. For example, a landscaping company offers weekly lawn service to its customers. Each weekly service incurs a $50 charge. A $50 statement charge is entered each week that the lawn service is performed. Then, one time each month a statement is sent to the customer showing the total due for services performed.

Statement charges increase expected receivables and increase income like invoices do. These journal lines are posted by this statement charge:

| Account | Debit | Credit |
| --- | --- | --- |
| Accounts Receivable (AR) | $200 |  |
| Sales Income |  | $200 |

Record Statement Charges at _Transactions > Sales > Create Statement Charges_.

### Additional Topics

-   [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html)
-   [SuiteGL Features Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4326823275.html)

### Related Topics

-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [GL Impact Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481077.html)
-   [Customer Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1460914.html)
-   [Vendor/Purchase Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1461991.html)
-   [Cost of Goods Sold (COGS) GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1464868.html)
-   [Bank Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1465926.html)
-   [General Ledger Tracking in Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556628.html)
-   [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
