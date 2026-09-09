---
id: "section_N1460914"
type: "section"
title: "Customer Transaction GL Impact"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > General Ledger Impact of Transactions > Customer Transaction GL Impact"
parent: "chapter_N1459499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1460914.html"
anchors: ["bridgehead_N1460933", "bridgehead_N1461102", "bridgehead_N1461275", "bridgehead_N1461290", "bridgehead_N1461467", "bridgehead_N1461640", "bridgehead_N1461655", "bridgehead_N1461674", "bridgehead_N1461701"]
sha256: "9f058d10944238fb1dcdc83eaf555df7729c26a29199e724cfccbc215e55cff8"
---

After customers are billed, you must process payments you receive. Customer transactions you enter in NetSuite include customer payments and deposits, return authorizations, receipts of item returns, credit memos, and customer refunds. As you enter customer transactions, NetSuite records the effects with journal entries in the general ledger.

## Customer Payments {#bridgehead_N1460933}

Enter customer payments to record payments you receive from customers. By recording payments, you can track how much money customers owe you. For example, Maple Street School has a $75 invoice due. They send you a check and you record the $75 payment. When you record a payment, it posts to the journal accounts affected by the payment. Recording a payment increases the total amount of funds you have yet to deposit in the bank. The payment posts this as $75 added to the Undeposited Funds account. Recording a payment also decreases the total amount of funds you expect to receive from customers. The payment posts this as $75 reduced from the Accounts Receivable account.

These journal lines are posted by the payment:

| Account | Debit | Credit |
| --- | --- | --- |
| Undeposited Funds | $75 |  |
| Accounts Receivable |  | $75 |

Record customer payments at _Transactions > Customers > Accept Customer Payments_.

## Customer Deposits {#bridgehead_N1461102}

Sometimes a customer pays a deposit or pre-payment before an order is complete. Record this payment as a deposit that can later be applied on the invoice for the order. Then, the total amount due is decreased by the amount of the deposit. For example, Maple Street School wants to buy new computers for their library. After they place the order, they pay a $1,000 deposit. When you record the customer deposit, the payment posts to the journal accounts affected by the deposit. Recording a deposit increases the total funds you're holding to apply to invoices later. The deposit posts this as a $1,000 increase in the Customer Deposits account. The deposit also increases the total amount of money due to be deposited in your bank account. The deposit posts this as a $1,000 increase in the Undeposited Funds account.

These journal lines are posted by the deposit:

| Account | Debit | Credit |
| --- | --- | --- |
| Undeposited Funds | $1,000 |  |
| Customer Deposits |  | $1,000 |

Record customer deposits at _Transactions > Customers > Record Customer Deposits_.

## Return Authorizations {#bridgehead_N1461275}

Customers that want to return an item for a refund or credit can be issued a return authorization. A return authorization enables you to track items you expect to be returned, but isn't a posting transaction. Items on return authorizations have no accounting impact until you receive those items back into inventory. When you receive the items back into your inventory, the costs and asset values of the items post to your ledger.

## Return Receipts {#bridgehead_N1461290}

When your warehouse gets an authorized return from a customer, you need to record that you have received it. Then, you can track which items you have already received and which ones you expect to receive later. For example, Maple Street School returns a keyboard they previously purchased. Your warehouse manager puts the keyboard back in stock to sell again later, and you record that the keyboard is added back into inventory.

When you receive a return, it posts to the journal accounts affected by the receipt. Because you're adding items of value to your inventory, receiving items increases the total value of your assets on hand. A return receipt posts an increase to an asset account. The amount of the increase that posts is based on the amount you paid for the item. You originally paid $10 for the keyboard, so the value of your assets on hand increases by $10. This posts as an increase in the Inventory Asset account. Receiving a return also decreases the total amount you have spent on items sold, which is tracked in the Cost of Goods Sold (COGS) account. You paid $10 for the keyboard, so this posts as a $10 decrease from the total amount in the COGS account.

These journal lines are posted by the deposit:

| Account | Debit | Credit |
| --- | --- | --- |
| Inventory Asset | $10 |  |
| Cost of Goods Sold (COGS) |  | $10 |

Record return receipts at _Transactions > Customers > Receive Returned Order_.

When a return has been received, you can issue a refund or credit to the customer.

## Credit Memos {#bridgehead_N1461467}

A credit memo decreases the amount a customer owes you. You can use a credit memo to reverse a charge billed to a customer. For example, last week you billed Maple Street School for 10 keyboards at $20 each. Upon realizing they had one keyboard too many, the school returned the extra keyboard. When the returned keyboard is received, you issue a credit memo to decrease the total amount the school owes. Issuing a credit memo posts to the journal accounts affected by the credit memo.

Because crediting an item reduces the amount you expect this customer to pay, it reduces the total funds you're expecting to receive. This posts as a $20 decrease to the Accounts Receivable account. Crediting the item decreases the total amount of your income from sales. This posts as a $20 decrease to the Sales Income account.

These journal lines are posted by the credit memo:

| Account | Debit | Credit |
| --- | --- | --- |
| Sales Income | $20 |  |
| Accounts Receivable (AR) |  | $20 |

Issue Credit Memos at _Transactions > Customers > Issue Credit Memos_.

When a credit memo has been issued, you can issue the customer a refund.

## Customer Refunds {#bridgehead_N1461640}

Customer refunds give money back to the customer in the amount that they originally paid. Refunds are often made using checks but may also credit the customer's credit card. You can refund money to customers by generating a refund from a credit memo or by generating an individual refund.

## Refunding from a Credit Memo {#bridgehead_N1461655}

For customers that are billed with invoices instead of cash sales, refund returns by first generating a credit memo and then clicking Refund on the credit memo. When you click Refund, a customer refund opens in the amount credited on the credit memo. For example, Maple Street School wants to be refunded the amount showing on the credit memo you issued for the returned keyboard. To process the refund, view the credit memo and click the Refund button.

Refund from a credit memo by going to _Transactions > Customers > Issue Credit Memos > List_ and clicking View next to the credit memo.

## Refunding a Cash Sale {#bridgehead_N1461674}

If you originally entered a cash sale and now need to refund money to a customer, enter an individual cash refund. A cash sale refund is a transaction that gives money back to a customer who paid for goods or services at the time of the sale using cash, a check, or a credit card.

Cash refunds are not generated from a credit memo, but instead issue a payment to the customer in the amount you enter on the cash refund. For example, a teacher at Maple Street School purchased three staplers for the classroom. The teacher bought the staplers with cash and you entered a cash sale. Later, the teacher realized that only two staplers were needed and returned one of them. To refund the money for the stapler, you enter a cash refund.

Enter a cash refund at _Transactions > Customers > Refund Cash Sales_.

| Account | Debit | Credit |
| --- | --- | --- |
| Sales Income | $20 |  |
| Checking Account (or Undeposited Funds Account) |  | $20 |

## Refund Journal Entries {#bridgehead_N1461701}

Refunding a return posts to the journal accounts affected by the refund.

Refunding a sale decreases the income generated from the original sale. When you refund the sale, the amount of income generated by the sale posts as a decrease to your sales income account. Refunding a sale takes money out of your checking account in the amount of the refund. This posts as a decrease to your checking account.

These journal lines are posted by the refund:

| Account | Debit | Credit |
| --- | --- | --- |
| Sales Income | $20 |  |
| Checking Account |  | $20 |

Refund a return at _Transactions > Customers > Refund Returns_.

### Additional Topics

-   [SuiteGL Features Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4326823275.html)

### Related Topics

-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [GL Impact Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481077.html)
-   [Sales Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459773.html)
-   [Vendor/Purchase Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1461991.html)
-   [Cost of Goods Sold (COGS) GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1464868.html)
-   [Bank Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1465926.html)
-   [General Ledger Tracking in Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556628.html)
-   [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
