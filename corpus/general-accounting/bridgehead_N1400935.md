---
id: "bridgehead_N1400935"
type: "bridgehead"
title: "Currency on Vendor Transactions"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Assigning Currencies to Entities > Vendors and Multiple Currencies > Currency on Vendor Transactions"
parent: "section_N1400742"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400935.html"
anchors: ["bridgehead_N1400984", "bridgehead_N1401058", "bridgehead_N1401074"]
sha256: "f64b09ad0ffd3c7cbade584f2ffebe8ab23674afef33dccd94224fd83f16648a"
---

When you enter a vendor transaction, such as a purchase order, the vendor's primary currency is the value in the Currency field by default. You can select a different transaction currency before you save the transaction. The currencies available for a vendor transaction are previously set up on the vendor record. For more information, see [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html).

After a transaction has been saved, you can't change the currency. If you need to use a different currency, you must delete the transaction and create a new one. You make a copy of the transaction and change the currency on the copy before you delete the original.

If you change the currency during new transaction creation, NetSuite tries to convert the prices on the transaction to the new currency. If you entered a custom price for a line item and then changed the currency, NetSuite can't convert the price. For the logic used to convert prices derived from item records to a different currency, see [Item Purchase Prices and Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1401098.html).

When vendors log in to the Vendor Center, they can see purchase requests and purchase orders in the currency in which the transactions were entered. Billable time entered through the Vendor Center uses the vendor's primary currency.

The Approve Bills transaction converts currency amounts on unapproved purchase orders and vendor bills to your company's base currency for approval.

See the following sections for additional information:

-   [Transaction Workflows](#bridgehead_N1400984)
    
-   [Vendor Payments](#bridgehead_N1401058)
    
-   [Order Items Transactions](#bridgehead_N1401074)
    

## Transaction Workflows {#bridgehead_N1400984}

When you convert a purchase transaction to another transaction in the purchase process, **the currency from the original transaction is maintained and can't be changed**.

This includes the following workflows:

-   Purchase request to purchase order
    
-   Purchase order to item receipt
    
-   Purchase order to vendor bill including purchase orders billed through the Bill Purchase Orders page
    
-   Vendor bill to vendor payment
    
-   Vendor return authorizations to vendor return item fulfillment
    

For example, if you create a purchase request using the euro, the resulting purchase order, item receipt, and vendor bill all use the euro.

Memorized purchase order transactions use the same currency as the original transaction. The cost of items on the generated purchase orders reflect this currency.

Drop-ship or special orders are purchased from an item's preferred vendor. The resulting purchase orders are in the preferred vendors' primary currency. The sales transactions can use any of your customer's transaction currencies.

## Vendor Payments {#bridgehead_N1401058}

When you record a payment made to a vendor, the default currency is the vendor's primary currency. You can, however, choose any of the vendor's transaction currencies. The currency selection filters the lists of vendors bills, credits, and deposits to match the currency you chose.

If you pay bills through the Pay Bills page, you can include payments in any number of vendor transaction currencies. Payment must be made in the same currency as the purchase order.

## Order Items Transactions {#bridgehead_N1401074}

The Order Items page displays all items with the purchase price of the items' preferred vendors. If you use this page and show items with no preferred vendor, you must use the vendor's primary currency when you select a vendor.

### Related Topics

-   [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html)
-   [Item Purchase Prices and Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1401098.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
