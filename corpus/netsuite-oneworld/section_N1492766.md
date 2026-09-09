---
id: "section_N1492766"
type: "section"
title: "Managing Intercompany Inventory Transfers - Arm's Length"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Managing Intercompany Inventory Transfers - Arm's Length"
parent: "chapter_N1486105"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html"
anchors: ["bridgehead_N1492930"]
sha256: "48475882ba0d9b355290c0b698e74bf4074df4c021e1a3464bc5e5bda51b0964"
---

The Automated Intercompany Management feature lets you manage and coordinate arm's length intercompany inventory transfers including intercompany drop ship orders. With this feature you can:

-   Automate the end-to-end intercompany inventory workflow. Use intercompany inventory purchase and sales orders, intercompany item fulfillments and receipts, and inventory sales invoices and vendor bills.
    
-   Use intercompany auto-elimination to automatically revalue the period-end inventory and Cost of Goods Sold (COGS) balances.
    
    Important:
    
    If you are doing arm's-length intercompany inventory transfers, the **Eliminate Intercompany Transactions** box on the COGS account must not be checked. Keep this box checked for other transfer orders that are not arm's-length.
    
-   Automatically process intercompany elimination entries for intercompany inventory.
    
-   Use intercompany inventory transfer and sales activity reports for a detailed audit trail.
    

Automated Intercompany Management supports month end elimination for arm's length and non-arm's length intercompany inventory transfers.

-   Create intercompany purchase orders and sales orders to manage intercompany arm's length inventory transfers, returns, and intercompany inventory drop shipments. See:
    
    -   [Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493092.html)
        
    -   [Intercompany Inventory Returns - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493277.html)
        
    -   [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html)
        
-   For non-arm's length intercompany inventory transfers, create an intercompany transfer order. See [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html).
    
-   Enter advanced intercompany journal entries for other adjustments to inventory accounts. See [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html) and [Enter Intercompany Transactions for Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501665.html).
    

## Key Points for Intercompany Inventory Transfers {#bridgehead_N1492930}

-   For arm's length intercompany inventory transfers, returns, and drop shipments, the item rate or transfer price must be the same on all transactions.
    
-   You can't modify the originating transaction (purchase order or vendor return authorization) when you generate the intercompany sales order or return authorization.
    
-   For arm's length intercompany inventory transfers, disable the **Use Item Cost as Transfer Cost** preference on the Accounting Preferences page on the Order Management subtab. You can find the Accounting Preferences page at _Setup > Accounting > Preferences > Accounting Preferences_.
    
-   The currency for all transactions created for intercompany inventory transfers and drop shipments is always the base currency of the purchase order. The base currency of the purchase order eliminates the need for foreign currency revaluation for the transactions at period end close.
    
-   Ownership of the item transfers from the source subsidiary to the destination subsidiary when the order is fulfilled.
    
-   The quantity received can't be greater than the quantity shipped.
    
-   There is a one-to-one relationship between the intercompany purchase order and the intercompany sales order. There is a one-to-one relationship between the intercompany vendor return authorization and intercompany return authorization.
    
-   You can't generate multiple sales orders for one intercompany purchase order. You can't generate one sales order for multiple intercompany purchase orders.
    
-   You must generate an intercompany sales order using the Manage Intercompany Sales Orders page for an order with an intercompany vendor and an inventory item. You can't manually create an intercompany sales order.
    
-   You must generate an intercompany return authorization for a return authorization with an intercompany vendor and an inventory item. Use the Manage Intercompany Return Authorization page to do this. You can't manually create an intercompany return authorization.
    
    The return process for an intercompany inventory transfer reverses the original transfer transaction. It originates when the subsidiary that purchased the item (the original destination subsidiary) creates a vendor return authorization for the original purchase order. The original source subsidiary (the subsidiary that sold the item) can't create a credit memo to initiate the return of an intercompany inventory transfer. Instead, **the source subsidiary automatically generates a return authorization for the vendor return authorization**. Then, each subsidiary completes their part of the return process. **NetSuite doesn't process changes made to any line.**
    

Note:

For arm's length intercompany inventory transfers, intercompany clearing accounts are not returned to zero when you eliminate intercompany transactions at period end close. Reporting at the subsidiary level displays the intercompany clearing account with an accumulated balance.

### Related Topics:

-   [Intercompany Inventory Transfer Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493711.html)
-   [Intercompany Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498276.html)
-   [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html)
-   [Defining Intercompany Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158989474458.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)
-   [Intercompany Sales and Billing Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492389.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)
-   [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html)
-   [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html)
-   [Working with Elimination Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502129.html)
-   [Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1486105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
