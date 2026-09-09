---
id: "section_N2218627"
type: "section"
title: "Scanning Bar Codes"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Bar Codes and Item Labels > Scanning Bar Codes"
parent: "chapter_N2215205"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2218627.html"
anchors: ["procedure_N2218658", "procedure_N2218752"]
sha256: "e9ed0a9425271e43ecda0d7e4fc3c825d20c8234d5e78f31a40fa2cd7f26e28b"
---

When you've printed transactions with bar codes or item labels with bar codes, you can scan these bar codes to enter them in transactions.

Scanning a bar code enters a number as if it were typed on the keyboard. For example, you can scan an item label bar code to add the item to a sales order. You can scan a sales order bar code to add the sales order to a queue to be fulfilled.

To scan bar codes properly, you must use popup windows rather than lists.

#### To use popup windows:

1.  Go to Home > Set Preferences.
    
2.  Set **Maximum Size of Drop Downs** to 0.
    
3.  Click **Save**.
    

#### To scan items and add them to a transaction: {#procedure_N2218658}

1.  When you're editing a transaction, such as a sales order or a transfer order, click the **Item** field to place the cursor there.
    
    On some transactions, click the **Select Item Number** field to place the cursor there.
    
2.  Scan the bar code on the item label of the item you want to add to the transaction.
    
    The item number and description are added automatically to the transaction.
    
3.  Press the **Enter** key after you scan each item.
    
    Some scanner software can be programmed to automatically press the Enter key after each scan. Check the manual for your scanner hardware for more information.
    
4.  Repeat steps from 1 to 3 for each item you want to add to the transaction.
    
5.  Verify that the items you scanned appear on the transaction.
    
6.  Click **Save**.
    

#### To scan transactions to add them to a queue: {#procedure_N2218752}

1.  When you're editing a page to add transactions, click the **Select Order Number** field to place the cursor there.
    
    For example, on the Fulfil Orders page, click the **Orders** subtab. Place the cursor in the **Select Order Number** field. The Fulfil Orders page is located at _Transactions > Sales > Fulfill Orders_.
    
2.  Choose **All** in filter fields.
    
    For example, on the Fulfill Orders page, in the **Customer** field, select **All** to show all open orders.
    
    Important:
    
    Don't leave this field blank or you cannot scan bar codes.
    
3.  Scan the bar code on transactions you want to add to the queue.
    
4.  Press the **Enter** key after each item you scan.
    
    Some scanner software can be programmed to automatically press the Enter key after each scan. Check the manual for your scanner hardware for more information.
    
5.  Repeat steps from 2 to 4 for each transaction you want to add to the queue.
    
6.  Verify that the transactions you scanned are marked to be processed.
    
7.  Click **Submit** to process the checked transactions.
    

### Related Topics

-   [Using Code 128 Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292085605.html)
-   [Enabling the Bar Coding and Item Labels Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292087805.html)
-   [Printing Bar Code and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2215536.html)
-   [Processing Orders Using Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N561778.html)
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N562976.html)
-   [Bar Codes and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
