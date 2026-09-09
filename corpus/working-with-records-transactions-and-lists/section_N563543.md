---
id: "section_N563543"
type: "section"
title: "Voiding, Deleting, or Closing Transactions"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Voiding, Deleting, or Closing Transactions"
parent: "chapter_N545359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html"
anchors: ["bridgehead_4241871944", "bridgehead_4241873225", "bridgehead_N563722"]
sha256: "796ee8d939ec0c93c1d34a6ac02cbd4cfb2655d355f9f251c0661d995f66e300"
---

You may need to change a transaction you've entered if it has errors or you don't intend to complete it. The following sections explain the differences between voiding, deleting, and closing transactions:

-   [Voiding Transactions](#bridgehead_4241871944)
    
-   [Deleting Transactions](#bridgehead_4241873225)
    
-   [Closing Line Items and Transactions](#bridgehead_N563722)
    

Important:

Before you delete or void a posting transaction, check to ensure that the transaction isn't part of a match on the Reconcile Account Statement page. You shouldn't delete transactions that have been reconciled. For more information, see _Viewing Submitted Transactions_.

## Voiding Transactions {#bridgehead_4241871944}

Voiding a transaction sets its total and all its line items to 0 but doesn't remove it from the system. This is the preferred way to cancel an existing transaction because the audit trail is preserved. After you void a transaction, you can't make changes that have general ledger impact to the original transaction, including changing the posting period.

If you void a transaction that was created to close another transaction, the original transaction is reopened. For example, if an invoice was created to bill a sales order, voiding the invoice reopens the sales order and sets the order's status to pending billing. Then you must invoice the order again. Another example is a bill payment that has been applied to a bill. If you void the bill payment, the bill is reopened. Another payment must be entered against the bill.

#### To void a transaction:

1.  Open the transaction for editing.
    
2.  Click Void.
    
    If the preference to void transactions with a reversing journal entry has been enabled, only certain types of transactions can be voided. For more information, see [Void Transactions Using Reversing Journals Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469460.html).
    

Voided sales orders don't show on the Transactions subtab of customer records. To view voided sales orders, go to _Transactions > Sales > Enter Sales Orders > List_.

Additional help is available for some transaction types as follows:

-   For information specific to check transactions, see [Voiding a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3951602420.html).
    
-   For information specific to credit cards, see [Voiding Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1570067.html).
    

## Deleting Transactions {#bridgehead_4241873225}

Important:

If the Use Deletion Reason feature is enabled in your account, you must provide a reason for deleting transaction records. For more information about the feature, see [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html).

You may want to remove a transaction from the system entirely. For example, after entering a transaction you may realize it contains many errors. You can delete it and reenter the transaction.

To delete a transaction, open the transaction you want to delete and click **Edit**. In the Actions menu, click **Delete**.

The Delete option appears only when both of the following conditions are met:

-   The Void Transactions Using Reversing Journals preference is not set. For more information, see [Void Transactions Using Reversing Journals Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469460.html).
    
-   Your role has Full level of access to that transaction type. For more information, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).
    

Note:

You can't delete a transaction if:

-   The transaction is linked to other transactions. For example, you can't delete an invoice that has been paid and that has an associated customer payment transaction. However, you can close linked transactions. For information about closing transactions, see [Closing Line Items and Transactions](#bridgehead_N563722).
    
-   The transaction is in a closed accounting period. To edit or delete a transaction in a closed period, you need to reopen the closed period. See [Reopening a Closed Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html).
    

You can also delete a transaction from the transaction List page when inline editing is enabled and you have the required permission. To delete a transaction from the transaction List page, hover over the New column and click Delete Record from the menu that appears. For more information about inline editing, see [Using Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html).

NetSuite does not retain the details of a deleted transaction. However, the audit trail includes a record that the transaction was deleted.

## Closing Line Items and Transactions {#bridgehead_N563722}

You can manually close transaction line items when you don't intend to fulfill or receive open items on the order. For example, you sell 10 items to a customer and have already fulfilled five of them. Then you discontinue the item and can't fulfill the remaining five. If you close the line manually instead of changing the quantity, you retain a record of how many were ordered originally.

#### To close a line item on a transaction:

1.  Click **Edit** on the transaction.
    
2.  Click the line you want to close, check the box in the Closed column and click **Done**.
    
3.  Click **Save**.
    

Note:

You must bill the sales order before you manually close the line. When all lines on a sales order are fulfilled or closed manually, the sales order is removed from the billing and receiving queues.

When you view sales orders, purchase orders, and return authorizations, click the **Close** or **Close Remaining** button to close the entire transaction. This action checks the Closed box for all lines on the transaction and changes the status of the transaction to Closed. You can reopen a closed transaction by clearing the Closed box for all lines on the transaction.

For specific information about sales orders, see [Closing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698204292.html).

### Related Topics

-   [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html)
-   [Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546079.html)
-   [Entering Transaction Line Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550610.html)
-   [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)
-   [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html)
-   [Tips for Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551712.html)
-   [Finding Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560124.html)
-   [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html)
-   [Preferred Transaction Delivery on Customer and Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N558109.html)
-   [Transaction Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569351.html)
-   [Transaction Detail Workbook Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156465780853.html)
-   [Limits for Display of Transaction Lists and Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569641.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
