---
id: "section_N1493711"
type: "section"
title: "Intercompany Inventory Transfer Examples"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Managing Intercompany Inventory Transfers - Arm's Length > Intercompany Inventory Transfer Examples"
parent: "section_N1492766"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html"
anchors: ["bridgehead_N1493770", "bridgehead_N1496683", "bridgehead_N1497553"]
sha256: "0b0e050473a3aad25f034948608b5cc0a6f0098991a2d273426ac3beb9ce3865"
---

-   [Arm's Length Intercompany Inventory Transfer Example](#bridgehead_N1493770)
    
-   [Arm's Length Intercompany Inventory Return Example](#bridgehead_N1496683)
    
-   [Intercompany Drop Ship Example](#bridgehead_N1497553)
    

## Arm's Length Intercompany Inventory Transfer Example {#bridgehead_N1493770}

This scenario illustrates an intercompany inventory transfer between two subsidiaries, U.K. and EU.

-   The EU subsidiary is the destination subsidiary and submits a purchase order for inventory item with transfer price of EUR 200. The base currency of the EU subsidiary is EUR.
    
-   The U.K. subsidiary is the source subsidiary and creates a corresponding sales order throught the Manage Intercompany Sales Orders page. The inventory item is accessible by both subsidiaries. In the U.K. subsidiary, the Cost of Goods Sold (COGS) amount for the item is GBP 100.
    
-   The U.K. subsidiary (source) fulfills the order and ships the item.
    
-   The EU subsidiary (destination) receives the item into inventory. On the Item Receipt, the receiving standard cost is EUR 160.
    
-   The EU subsidiary records a vendor bill.
    
-   The U.K. subsidiary creates a sales invoice.
    

The following table presents the general ledger impact for each of the posting transactions involved in the inventory transfer.

Note:

In this example, the general ledger impact for COGS and Inventory lines post in the currency of the source subsidiary (GBP). All of the transactions for the transfer are in the currency of the destination subsidiary (EUR).

**However, the currency that impacts the GL is the currency used in the transaction. This currency is from source subsidiary.**

| Subsidiary | Account | Debit | Credit |
| --- | --- | --- | --- |
| **Item Fulfillment** |
| U.K. | Cost of Goods Sold (COGS) | GBP 100 |  |
| U.K. | Inventory |  | GBP 100 |
| EU | Inventory In Transit | EUR 200 |  |
| EU | Intercompany Clearing |  | EUR 200 |
| **Item Receipt** |
| EU | Purchase Price Variance | EUR 40 |  |
| EU | Inventory | EUR 160 |  |
| EU | Inventory In Transit |  | EUR 200 |
| EU | Intercompany Clearing | EUR 200 |  |
| EU | Accrued Purchases |  | EUR 200 |
| **Sales Invoice** |
| U.K. | Intercompany A/R | EUR 200 |  |
| U.K. | Intercompany Revenue |  | EUR 200 |
| **Vendor Bill** |
| EU | Accrued Purchases | EUR 200 |  |
| EU | Intercompany A/P |  | EUR 200 |

For more information about arm's length inventory transfers, see [Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493092.html).

## Arm's Length Intercompany Inventory Return Example {#bridgehead_N1496683}

In this scenario, the EU subsidiary returns the item from the previous example back to the U.K. subsidiary. The return is a complete reversal of the accounting impact of the original transfer.

-   The EU subsidiary creates a vendor return authorization to initiate the return. The vendor return authorization must be created from the original purchase order and be linked to it. It must be in the same currency as the original intercompany purchase order and sales order pair.
    
-   The U.K. subsidiary creates the return authorization through the Manage Intercompany Return Authorizations page.
    
-   The EU subsidiary returns the item and records an item fulfillment.
    
-   The U.K. subsidiary receives the item and records an item receipt. The U.K. subsidiary restock the item or discard it as an expense.
    
-   The EU subsidiary records a vendor credit.
    
-   The U.K. subsidiary issues a credit memo.
    

The following table presents the general ledger impact for each of the posting transactions involved in the inventory return.

Note:

The general ledger impact for Cost of Goods Sold (COGS) and inventory lines post in the currency of the source subsidiary (GRP). All of the transactions for the transfer are in the currency of the destination subsidiary (EUR).

| Subsidiary | Account | Debit | Credit |
| --- | --- | --- | --- |
| **Item Fulfillment** |
| EU | Inventory |  | EUR 200 |
| EU | Inventory In Transit | EUR 200 |  |
| EU | Intercompany Clearing |  | EUR 200 |
| EU | Purchases Returned Not Credited | EUR 200 |  |
| **Item Receipt** |
| U.K. | Cost of Goods Sold (COGS) |  | GBP 100 |
| U.K. | Inventory (Expense if received as scrap) | GBP 100 |  |
| EU | Inventory In Transit |  | EUR 200 |
| EU | Intercompany Clearing | EUR 200 |  |
| **Vendor Credit** |
| EU | Purchases Returned Not Credited |  | EUR 200 |
| EU | Intercompany A/P | EUR 200 |  |
| **Credit Memo** |
| U.K. | Intercompany A/R |  | EUR 200 |
| U.K. | Intercompany Revenue | EUR 200 |  |

For more information about intercompany inventory returns, see [Intercompany Inventory Returns - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493277.html).

## Intercompany Drop Ship Example {#bridgehead_N1497553}

This scenario illustrates an intercompany drop ship order involving two subsidiaries, U.K. and EU.

-   The EU subsidiary is the sales subsidiary selling an item to Customer that is to be shipped from a warehouse in the U.K. subsidiary. The base currency of the EU subsidiary is EUR. The EU subsidiary creates a sales order in the amount of EUR 200 and identifies the U.K. subsidiary as the vendor for the transaction.
    
-   The EU subsidiary submits a purchase order for inventory item with transfer price of EUR 200.
    
-   The U.K. subsidiary is the warehouse subsidiary and creates a corresponding intercompany sales order through the Manage Intercompany Sales Orders page. The inventory item is accessible by both subsidiaries. In the U.K. subsidiary the Cost of Goods Sold (COGS) amount for the item is GBP 100.
    
-   The U.K. subsidiary fulfills the order and ships the order directly to Customer.
    
-   The U.K. subsidiary creates a sales invoice to bill the EU subsidiary.
    
-   The EU subsidiary marks the dummy fulfillment for the intercompany purchase order as Marked Shipped.
    
-   The EU subsidiary creates a vendor bill from the intercompany purchase order to bill the U.K. subsidiary.
    

The following table presents the general ledger impact for each of the transactions involved in the intercompany drop shipment.

Note:

The general ledger impact for COGS and Inventory lines post in the currency of the sales subsidiary (GRP). All of the transactions for the transfer are in the currency of the destination subsidiary (EUR).

| Subsidiary | Account | Debit | Credit |
| --- | --- | --- | --- |
| **External Item Fulfillment** |
| U.K. | Cost of Goods Sold (COGS) | GBP 100 |  |
| U.K. | Inventory |  | GBP 100 |
| **Dummy Item Fulfillment** |
| Non-posting |
| **Sales Invoice** |
| U.K. | Intercompany A/R | EUR 200 |  |
| U.K. | Intercompany Revenue |  | EUR 200 |
| **Vendor Bill** |
| EU | Inventory Dropship Expense | EUR 200 |  |
| EU | Intercompany A/P |  | EUR 200 |
| **External Sales Invoice** |
| EU | Accounts Receivable | EUR 200 |  |
| EU | Revenue |  | EUR 200 |

For more information about an intercompany drop ship order, see [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html).

### Related Topics:

-   [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html)
-   [Intercompany Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498276.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
