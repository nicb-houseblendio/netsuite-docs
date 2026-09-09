---
id: "section_N1461991"
type: "section"
title: "Vendor/Purchase Transaction GL Impact"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > General Ledger Impact of Transactions > Vendor/Purchase Transaction GL Impact"
parent: "chapter_N1459499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1461991.html"
anchors: ["bridgehead_N1462014", "bridgehead_N1462033", "bridgehead_N1462228", "bridgehead_N1462397", "bridgehead_N1462566", "procedure_0824114745"]
sha256: "9565de108e26b16faa3be6f9c69c3d8070b04e4f656593e7dbb32cb846e53302"
---

Purchase transactions you enter in NetSuite include purchase orders, item receipts, vendor bills, vendor payments, and vendor credits.

As you enter these transactions, NetSuite records the costs and value of items. These transaction forms appear on the Transactions tab under the Sales Transaction heading when you're logged in using your Administrator role.

## Purchase Orders {#bridgehead_N1462014}

Entering purchase orders enables you to track the items you expect to receive from vendors and the costs associated with those purchases. Purchase orders, however, are non-posting transactions. They don't post an amount to your ledger accounts.

Record purchase orders at _Transactions > Purchases > Enter Purchase Orders_.

When you receive the purchase order, the costs and asset values of the items post to your ledger.

## Item Receipts {#bridgehead_N1462033}

As shipments arrive at your business, match them against open purchase orders to receive them into inventory. Record an item receipt to detail the items you're receiving into your inventory. For example, the Jones Paper Company ships you 10 cases of paper at a purchase price of $10 each. After you verify that the shipment contains all 10 cases, you record that you received them into your inventory. When you record an item receipt, it posts to the journal accounts affected by the receipt.

Receiving items increases the total value of your assets on hand. The receipt posts this as $100 added to the Inventory Asset account. Receiving items also increases the total amount owed to your vendor. The item receipt posts a $100 increase in the total amount of the Accrued Purchase account.

These journal lines are posted by the receipt:

| Account | Debit | Credit |
| --- | --- | --- |
| Inventory Asset | $100 |  |
| Accrued Purchase |  | $100 |

Record item receipts at _Transactions > Purchases > Receive Orders_.

If you use the Advanced Receiving feature, item receipts can post to other ledger accounts. For detailed information about the Advanced Receiving feature and tracking Cost of Goods Sold (COGS), see [LIFO/FIFO Inventory Costing and Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html).

## Vendor Bills {#bridgehead_N1462228}

Entering vendor bills enables you to record invoices you receive from vendors. Then, you can pay bills from the payable list as they're due. By recording vendor bills rather than writing a check to the vendor, you can track how much money your business owes at any point during the billing cycle. For example, you enter a bill from the Jones Paper Company showing $100 due for 10 cases of paper. When you record a bill, the bill posts to the journal accounts affected by the bill.

Billing items decreases the total amount you must schedule for payment to a vendor. The bill posts this as a $100 decrease from the account Accrued Purchase. Billing items also increases the money you're due to pay out. The bill posts this as a $100 increase in the Accounts Payable account.

These journal lines are posted by the bill:

| Account | Debit | Credit |
| --- | --- | --- |
| Accrued Purchase | $100 |  |
| Accounts Payable (AP) |  | $100 |

Record vendor bills at _Transactions > Payables > Enter Bills_.

## Vendor Payments {#bridgehead_N1462397}

Enter vendor payments to record when you pay a vendor bill. The payment records the payment date and the amount paid. By tracking payments you make to vendors, you know how much money you owe to specific vendors. For example, you pay the $100 bill from Jones Paper Company. When you record a vendor payment, the payment posts to the journal accounts affected by the payment.

Paying bills reduces the total amount of money you owe to vendors. The vendor payment posts a $100 decrease of the amount in the Accounts Payable account. The bill payment also decreases the total amount of money in the bank account you pay from. The vendor payment posts a $100 decrease of the total amount of funds in the Checking account.

These journal lines are posted by the payment:

| Account | Debit | Credit |
| --- | --- | --- |
| Accounts Payable (AP) | $100 |  |
| Checking |  | $100 |

Record a vendor payment at _Transactions > Payables > Pay Bills_ or _Transactions > Payables > Pay Single Vendor_.

## Vendor Credits {#bridgehead_N1462566}

Enter a vendor credit to record credit from a vendor that you can apply to your payable account. Vendors may credit your account if you return merchandise to them or negotiate a discount after receiving an invoice. For example, after you paid the bill to Jones Paper Company, you discover that one case of paper you received is damaged. You send the paper back and they fax you a credit memo for $10. You record the $10 credit so you can apply it against another Jones bill the next time you make a payment.

When you enter a vendor credit, the credit posts to the journal accounts affected by the credit. Crediting items decreases the total amount of money you're due to pay out to the vendor. The credit posts a $10 decrease of the amount in the Accounts Payable account. Vendor credit decreases the total value of your inventory. The vendor credit posts a $10 decrease of the total amount in the Inventory Asset account.

These journal lines are posted by the credit:

| Account | Debit | Credit |
| --- | --- | --- |
| Accounts Payable (AP) | $10 |  |
| Inventory Asset |  | $10 |

There are two ways to enter a vendor credit:

-   Manually create a credit that isn't necessarily associated with an existing bill.
    
    To manually enter a vendor credit, go to _Transactions> Payables > Enter Vendor Credits_.
    
-   Create a credit from an original vendor bill.
    

#### To create a credit from an original vendor bill: {#procedure_0824114745}

1.  Go to _Lists > Relationships > Vendors_.
    
2.  Click the **Vendor Dashboard** icon next to the **View**.
    
3.  In the Transaction section of the Vendor Dashboard Links portlet, hover over **Enter Bills** and click **List**.
    
4.  Click **View** next to the account you want to create a credit from.
    
5.  Click **Credit**.
    
6.  Fill in the Bill Credit form.
    
7.  Click **Save**.
    

### Additional Topics

-   [Purchasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2399286.html)
-   [Vendor Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2381615.html)
-   [Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2386193.html)
-   [Vendor Credits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2391960.html)
-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)
-   [SuiteGL Features Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4326823275.html)

### Related Topics

-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [GL Impact Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481077.html)
-   [Sales Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459773.html)
-   [Customer Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1460914.html)
-   [Cost of Goods Sold (COGS) GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1464868.html)
-   [Bank Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1465926.html)
-   [General Ledger Tracking in Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556628.html)
-   [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
