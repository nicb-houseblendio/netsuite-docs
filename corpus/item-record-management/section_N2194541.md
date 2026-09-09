---
id: "section_N2194541"
type: "section"
title: "LIFO/FIFO Inventory Costing and Advanced Receiving"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > LIFO/FIFO Inventory Costing and Advanced Receiving"
parent: "chapter_N2191369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html"
anchors: ["bridgehead_N2194557", "bridgehead_N2194718"]
sha256: "da2d334803d18b5a6ecff521ff63fac06c87f60e32b88599547af1c52f370c8b"
---

NetSuite tracks inventory costing differently based on the Advanced Receiving feature.

## LIFO/FIFO Costing With Advanced Receiving {#bridgehead_N2194557}

If you use Advanced Receiving, LIFO/FIFO costing happens at the time of item receipt. Inventory costing is determined by the amounts entered on purchase orders.

The following transactions may affect inventory costing:

-   Create Invoice
    
-   Enter Cash Sale
    
-   Write Checks
    
-   Use Credit Cards
    
-   Enter Purchase Orders (determines inventory cost)
    
-   Item Receipt (determines inventory costing date)
    
-   Issue Credit Memo and Refund Cash Sale
    
    -   affects inventory costing the same way an item receipt does
        
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        
-   Enter Vendor Credits
    
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        
-   Adjust Inventory
    
    -   affect inventory costing the way purchases and sales do
        
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        

## LIFO/FIFO Costing Without Advanced Receiving {#bridgehead_N2194718}

If you don't use Advanced Receiving, inventory costing happens when you enter the bill. Inventory cost is determined by amounts entered on bills for inventory items. Inventory costing can't be tracked or calculated until a bill is entered.

The following transactions may affect inventory costing:

-   Create Invoices
    
-   Enter Cash Sale
    
-   Write Checks
    
-   Use Credit Cards
    
-   Enter Bills
    
-   Issue Credit Memo and Refund Cash Sales
    
    -   affects inventory costing the same way a purchase does
        
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        
-   Enter Vendor Credits
    
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        
-   Adjust Inventory
    
    -   affects inventory costing the same way purchases and sales do
        
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        

### Related Topics

-   [Setting Inventory Costing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html)
-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html)
-   [Selecting a Default Cost of Goods Sold (COGS) Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2192814.html)
-   [Inventory Costing and Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194190.html)
-   [System Cost of Goods Sold Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html)
-   [Viewing Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197076.html)
-   [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)
-   [Troubleshoot Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4447393386.html)
-   [Cost Accounting Status on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199228.html)
-   [Item Return Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html)
-   [Group Average Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
