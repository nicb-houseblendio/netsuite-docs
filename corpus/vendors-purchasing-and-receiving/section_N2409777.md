---
id: "section_N2409777"
type: "section"
title: "Purchase Order History Report"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order History Report"
parent: "chapter_N2399286"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2409777.html"
anchors: []
sha256: "3b8a5fb4e9e36ed82599304aaef74b3eee2927d37f9a3c4f76aea0e3102b2902"
---

The Purchase Order History report details purchase orders you have entered and helps you assess transactions and items associated with them. You can see how much you have authorized for purchase and at what price. You can also see how many you have received, and how much you have been billed for items.

To view the Purchase Order History report, go to _Reports > Purchases > Purchase Order History_.

To filter the data on the report, see [Filtering Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N742381.html).

The Purchase Order History report can help you spot discrepancies between amounts ordered and billed or between rates on orders and bills. This can help you reconcile your accounts by gathering data about orders and bills for comparison.

On the Purchase Order History report, the Receipt Minus Bill Amount column displays posting lines from inventory items on transactions.

-   Receipts have a positive value in this column.
    
-   Vendor bills have a negative value in this column.
    

If the Receipt Minus Bill Amount is not balanced, this could indicate a problem in the workflow for that order that must be reconciled. Keeping track of these discrepancies for orders can help you verify that vendors bill you the correct amount.

For example, purchase order #1001 shows 5 widgets ordered. The receipt against the purchase order shows 5 widgets received, but the associated bill shows the vendor charged you for 10 widgets. Because the bill amount is higher than the order amount, the Receipt Minus Bill Amount is not balanced for that order. The Purchase Order History report helps you identify such a discrepancy.

If the Receipt Minus Bill Amount is not balanced, it is may be due to one of the following three causes:

1.  The quantity on the order and the quantity on the bill do not match.
    
    This might indicate that you have been billed for an incorrect quantity.
    
    For example, purchase order #1001 shows 5 widgets ordered. The receipt against the purchase order shows 5 widgets received, but the associated bill shows the vendor charged you for 10 widgets.
    
    Verify that quantities match in the Qty column.
    
2.  The purchase price on the order and the price on the vendor bill do not match.
    
    This might indicate you have been billed at the wrong rate by the vendor.
    
    For example, purchase order #1001 shows 5 widgets ordered at $5 each. The associated bill shows the vendor charged you $10 per widget.
    
    Verify that billing rates are correct in the Rate column.
    
3.  The currency exchange rate on the order is no longer current when you enter the receipt.
    
    Currency rate fluctuations can cause discrepancies in the cost of an item. This means that even if quantities and prices are entered correctly, the amounts can be inaccurate.
    
    For example when you entered the purchase order, the exchange rate was 1.0. Later, when you enter the receipt, the current exchange rate is 1.25. If you do not use the current rate on the receipt, it may cause a discrepancy.
    
    Compare rates in the Rate column to identify exchange rate issues.
    
    Note:
    
    You can set the Default Receiving Exchange Rate preference to determine how rates are handled. For more information, see [Exchange Rates on Item Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415572.html).
    

For discrepancies you find that can't be corrected by updating a quantity or rate, create a journal entry to resolve the issue. For details on creating journal entries, see [Manual Journal Entry Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469070.html).

### Related Topics

-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)
-   [Purchase Order Approval Workflow SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2398841.html)
-   [Accounting for Received Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408991.html)
-   [Drop Shipment and Special Order Purchases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2409296.html)
-   [Centralized Purchasing and Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161122386910.html)
-   [Purchasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2399286.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
