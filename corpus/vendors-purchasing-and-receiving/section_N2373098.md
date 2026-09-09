---
id: "section_N2373098"
type: "section"
title: "Vendor Bill Variance Journals"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Variances > Vendor Bill Variance Journals"
parent: "section_N2371184"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373098.html"
anchors: []
sha256: "94053644165613691238e43daa2bca470017be26a6af0370d442f75f78f41a8b"
---

On journals that post vendor bill variances, note the following. Journal line details show the accounts being debited and credited by the entry to clear the Accrued Purchases account.

-   **Journal accounts**
    
    The accounts that journal lines post to are determined by the accounts selected on item records. For information about these accounts, read about variance accounts in [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
-   **Journal amounts**
    
    The amounts on journal lines are the amounts calculated from the vendor bills and receipts associated with the purchase order. These amounts are calculated as described below:
    
    Three kinds of variances can be generated:
    
    -   **Bill Price Variance** - The variance associated with price changes between the time you receive an item and the time the vendor bills you.
        
        Bill Price Variance = VB Qty \* ((VB Val / VB Qty) - (IR Val / IR Qty)) \* ((VB Value \* VB Average FX)/VB Val)
        
    -   **Bill Quantity Variance** - The variance associated with any quantity differences between the item receipt and the vendor bill.
        
        Bill Quantity Variance = (VB Qty - IR Qty)\*(IR Val / IR Qty)
        
    -   **Bill Exchange Rate Variance** - A variance associated with exchange rate changes. These changes occur between the time you receive an item and the time the vendor bills you.
        
        Exchange Rate Variance = VB Qty \* (IR Val / IR Qty) \* (((VB Val \* VB Average FX) / VB Val) - (IR Val \* IR Average FX) / IR Val)
        

When the Match Bill to Receipts method is not used and multiple receipt lines are posted against a purchase order line, note the following. The receipt quantities, receipt amounts, and receipt exchange rates used for variance calculations are as follows:

-   Receipt Quantity = The sum of quantities on receipts linked to the purchase order line.
    
-   Receipt Price = The sum of amounts on receipts linked to the purchase order line.
    
    In addition, the sum of quantities on receipts linked to the purchase order line.
    
-   Receipt Exchange Rate = The sum of foreign currency amounts on receipts linked to the purchase order line.
    
    In addition, the sum of base currency amounts on receipts linked to the purchase order line.
    

When the Match Bill to Receipts method is not used, note the following. The vendor bill quantities, vendor bill amounts and vendor bill exchange rates for variance calculations are as follows:

-   Bill Quantity = The sum of quantities on bills linked to the purchase order line.
    
-   Bill Price = The sum of amounts on bills linked to the purchase order line.
    
    In addition, the sum of quantities on bills linked to the purchase order line.
    
-   Bill Exchange Rate = The sum of foreign currency amounts on bills linked to the purchase order line.
    
    In addition, the sum of base currency amounts on bills linked to the purchase order line.
    

When the Match Bill to Receipts method is used and multiple receipt lines are linked to a vendor bill line, note the following. The quantities, amounts, and exchange rates used for variance calculations are as follows:

-   Receipt Quantity = The sum of quantities on receipts linked to the vendor bill line.
    
-   Receipt Price = The sum of amounts on receipts linked to the vendor bill line.
    
    In addition, the sum of quantities on receipts linked to the vendor bill line.
    
-   Receipt Exchange Rate = The sum of foreign currency amounts on receipts linked to the vendor bill line.
    
    In addition, the sum of base currency amounts on receipts linked to the vendor bill line.
    

After these calculations complete, NetSuite posts the following entries:

-   DR Accrued Purchases
    
-   CR Exchange Rate Variance
    
-   CR Bill Quantity Variances
    
-   CR Vendor Bill Price Variances
    

Important:

After the variances on the journal entry are created and posted, associated purchase orders, receipts, and vendor bills transactions can"t be changed.

The variance journal entries must be voided or deleted to allow changes to associated transactions. Also, the accounting period must be open for the entries being considered.

### Additional Information

-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)

### Related Topics

-   [Posting Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2372745.html)
-   [Mass Updates for Variance Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373402.html)
-   [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
