---
id: "section_N2193441"
type: "section"
title: "Inventory Reporting After Changing the Costing Method"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Costing Methods > Setting a Default Inventory Costing Method > Inventory Reporting After Changing the Costing Method"
parent: "section_4345703007"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2193441.html"
anchors: ["bridgehead_N2193482", "bridgehead_N2193709"]
sha256: "83c855e6afb97b5d7c3ad68b5c4cb09f46abdf297b92db0bcb08befb86e01b69"
---

You can select the type of inventory costing method your business uses. The cost of your inventory includes your items' purchase prices and any other costs you incur to get them. The costing method determines how you handle the costs of buying the same items at different prices over time. Your inventory reports reflect the costing method you choose. Average costing is the default costing method.

NetSuite records inventory costs at different times depending on whether you use the Advanced Receiving feature. For a procedure to enable this feature, see [Setting a Default Inventory Costing Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703007.html).

## LIFO/FIFO Costing if You Don't Use Advanced Receiving {#bridgehead_N2193482}

-   Costing happens when you enter the bill
    
-   The amounts you enter on bills for inventory items determine inventory costing
    
-   Inventory costing doesn't exist until you enter a bill
    
-   If a purchase order is still open when a period closes, you can choose to:
    
    -   Reopen the period and change the purchase order amounts to match the bill
        
    -   Leave the discrepancy because it has no impact on accounting
        
-   Transactions that might affect inventory costing:
    
    -   Create Invoices
        
    -   Enter Cash Sale
        
    -   Write Checks
        
    -   Use Credit Cards
        
    -   Enter Bills
        
    -   Issue Credit Memo and Refund Cash Sales
        
        -   affects inventory costing the same way a purchase does
            
        -   most recent value used for LIFO
            
        -   oldest value used for FIFO
            
        -   quantities returned are added back to inventory available for sale
            
    -   Enter Vendor Credits
        
        -   most recent value used for LIFO
            
        -   oldest value used for FIFO
            
        -   quantities credited decrease the quantity of inventory available for sales
            
    -   Adjust Inventory
        
        -   affects inventory costing the same way purchases and sales do
            
        -   most recent value used for LIFO
            
        -   oldest value used for FIFO
            
        -   quantity increases add inventory available for sale
            
        -   quantity decreases lower inventory available for sale
            

## LIFO/FIFO Costing if You Use Advanced Receiving {#bridgehead_N2193709}

-   Costing happens during item receipt
    
-   The amounts you enter on purchase orders for inventory items determine inventory costing, but dates depend on item receipts
    
-   Inventory costing doesn't exist until you enter an item receipt
    
-   If a purchase order is still open when a period closes, you can choose to:
    
    -   Reopen the period, delete the item receipt, change the purchase order amounts to match the bill, and then recreate the item receipt
        
    -   Create a journal entry to post the inventory costing variance in the new period
        
    -   Enter the bill with variances and accept reporting discrepancies
        
        For example, if the bill price is higher than the purchase order price, inventory costing will be understated.
        
-   Transactions that might affect inventory costing:
    
    -   Create Invoice
        
    -   Enter Cash Sale
        
    -   Write Checks
        
    -   Use Credit Cards
        
    -   Enter Purchase Orders - this determines the inventory costing cost
        
    -   Item Receipt - this determines the inventory costing date
        
    -   Issue Credit Memo and Refund Cash Sale
        
        -   affects inventory costing the same way a purchase order does
            
        -   most recent value used for LIFO
            
        -   oldest value used for FIFO
            
        -   quantities returned are added to inventory available for sale
            
    -   Enter Vendor Credits:
        
        -   most recent value used for LIFO
            
        -   oldest value used for FIFO
            
        -   quantities credited decrease the inventory available for sale
            
    -   Adjust Inventory
        
    -   affects inventory costing the way purchases and sales do
        
    -   most recent value used for LIFO
        
    -   oldest value used for FIFO
        
    -   quantity increases add inventory available for sale
        
    -   quantity decreases lower inventory available for sale
        

### Related Topics

-   [Changing Your Costing Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_160650437174.html)
-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
